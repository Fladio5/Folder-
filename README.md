# Folder-
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Plano de Acompanhamento de Saúde</title>
    <style>
        :root {
            --verde: #A8D8B9;
            --coral: #FF9E80;
            --bege: #F5F0E6;
            --branco: #F9F9F9;
            --cinza: #555555;
        }
        
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }
        
        body {
            font-family: 'Raleway', sans-serif;
            background: #f0f0f0;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            padding: 20px;
        }
        
        .folder-container {
            width: 100%;
            max-width: 800px;
            background: white;
            box-shadow: 0 5px 30px rgba(0,0,0,0.15);
            border-radius: 8px;
            overflow: hidden;
        }
        
        .print-button {
            display: block;
            width: 100%;
            padding: 15px;
            background: var(--verde);
            color: white;
            text-align: center;
            font-weight: bold;
            cursor: pointer;
            border: none;
            font-size: 18px;
            transition: all 0.3s;
        }
        
        .print-button:hover {
            background: #8bc2a5;
        }
        
        .folder {
            display: flex;
            flex-wrap: wrap;
        }
        
        .panel {
            width: 50%;
            min-height: 400px;
            padding: 30px;
            position: relative;
        }
        
        /* Painel 1: Capa */
        .panel-1 {
            background: var(--bege);
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            background-image: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="100" height="100" viewBox="0 0 100 100"><rect width="100" height="100" fill="none" stroke="%23A8D8B980" stroke-width="0.5"/></svg>');
        }
        
        .panel-1 h1 {
            font-family: 'Montserrat', sans-serif;
            font-size: 28px;
            color: var(--coral);
            margin-bottom: 15px;
            line-height: 1.3;
        }
        
        .panel-1 p {
            font-size: 18px;
            color: var(--cinza);
            max-width: 90%;
            margin-bottom: 10px;
        }
        
        .quote {
            font-style: italic;
            margin-top: 20px;
            color: var(--cinza);
            font-size: 16px;
        }
        
        /* Painel 2: Mensagem */
        .panel-2 {
            background: linear-gradient(to bottom, var(--coral), var(--branco));
            display: flex;
            flex-direction: column;
            justify-content: center;
        }
        
        .panel-2 h2 {
            font-family: 'Montserrat', sans-serif;
            color: white;
            font-size: 24px;
            margin-bottom: 20px;
        }
        
        .panel-2 p {
            color: white;
            margin-bottom: 15px;
            line-height: 1.6;
        }
        
        .highlight {
            background-color: var(--verde);
            padding: 10px 20px;
            border-radius: 30px;
            display: inline-block;
            margin-top: 15px;
            font-weight: bold;
            color: #333;
        }
        
        /* Painel 3: Benefícios */
        .panel-3 {
            background: var(--branco);
        }
        
        .panel-3 h2 {
            font-family: 'Montserrat', sans-serif;
            color: var(--coral);
            font-size: 24px;
            margin-bottom: 25px;
        }
        
        .benefits-list {
            list-style: none;
        }
        
        .benefits-list li {
            margin-bottom: 15px;
            padding-left: 35px;
            position: relative;
            line-height: 1.5;
        }
        
        .benefits-list li:before {
            content: "✓";
            color: var(--coral);
            font-size: 22px;
            position: absolute;
            left: 0;
            top: -2px;
        }
        
        /* Painel 4: Contato */
        .panel-4 {
            background: var(--bege);
            display: flex;
            flex-direction: column;
            justify-content: flex-end;
        }
        
        .contact-info {
            text-align: right;
        }
        
        .contact-info h2 {
            font-family: 'Montserrat', sans-serif;
            color: var(--coral);
            font-size: 24px;
            margin-bottom: 15px;
        }
        
        .contact-info p {
            margin-bottom: 8px;
            color: var(--cinza);
        }
        
        .contact-number {
            font-size: 20px;
            font-weight: bold;
            margin: 15px 0;
            color: #333;
        }
        
        /* Media Query para impressão */
        @media print {
            body {
                background: white;
                padding: 0;
            }
            
            .print-button {
                display: none;
            }
            
            .folder-container {
                box-shadow: none;
                border-radius: 0;
                max-width: 100%;
            }
        }
        
        @media (max-width: 768px) {
            .panel {
                width: 100%;
                min-height: 300px;
            }
        }
    </style>
</head>
<body>
    <div class="folder-container">
        <button class="print-button" onclick="window.print()">IMPRIMIR FOLDER</button>
        
        <div class="folder">
            <!-- Painel 1: Capa -->
            <div class="panel panel-1">
                <h1>Sua jornada para uma saúde plena começa aqui</h1>
                <p>Parabéns por escolher um cuidado que valoriza você</p>
                <p class="quote">"Cada passo importa. Estamos juntos nessa caminhada."</p>
            </div>
            
            <!-- Painel 2: Mensagem -->
            <div class="panel panel-2">
                <h2>Querido(a) paciente,</h2>
                <p>Bem-vindo(a) ao plano de acompanhamento que entende suas necessidades únicas. Esta não é apenas uma assistência médica, mas um compromisso genuíno com seu bem-estar integral.</p>
                <div class="highlight">Sua coragem em investir em si mesmo(a) merece celebração!</div>
            </div>
            
            <!-- Painel 3: Benefícios -->
            <div class="panel panel-3">
                <h2>Seu plano inclui:</h2>
                <ul class="benefits-list">
                    <li><strong>10 consultas médicas/ano</strong> + Bioimpedância em todas as consultas</li>
                    <li><strong>4 sessões com nutricionista/ano</strong>: Alimentação como aliada</li>
                    <li><strong>6 encontros com psicólogo/ano</strong>: Cuidando da mente</li>
                    <li><strong>Acompanhamento semanal via WhatsApp</strong>: Suporte contínuo</li>
                    <li><strong>Contato direto com a médica</strong>: (21) 97251-6275 (dúvidas)</li>
                    <li><strong>Plano de saúde personalizado</strong>: Feito sob medida para você</li>
                </ul>
                <div class="highlight">Tudo para que você se sinta seguro(a) em cada etapa</div>
            </div>
            
            <!-- Painel 4: Contato -->
            <div class="panel panel-4">
                <div class="contact-info">
                    <h2>Estamos aqui para você</h2>
                    <p>Dra. [Seu Nome]</p>
                    <p>Especialista em Medicina Preventiva</p>
                    <div class="contact-number">📱 (21) 97251-6275</div>
                    <p>✉️ email@clinica.com</p>
                    <p class="quote">"Sua saúde é uma história que escrevemos juntos, com respeito e escuta."</p>
                </div>
            </div>
        </div>
    </div>

    <!-- Fontes do Google -->
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@700&family=Raleway:wght@400;500;600&display=swap" rel="stylesheet">
    
    <script>
        // Configurações de impressão otimizadas
        document.querySelector('.print-button').addEventListener('click', function() {
            window.print();
        });
    </script>
</body>
</html>
