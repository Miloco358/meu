<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Amizades que Evoluem</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            background-color: #f5f5f5;
            color: #333;
        }
        
        header {
            background-color: #ff6b6b;
            color: white;
            text-align: center;
            padding: 2rem 0;
        }
        
        .container {
            max-width: 800px;
            margin: 2rem auto;
            padding: 0 20px;
        }
        
        .pricing {
            background-color: white;
            border-radius: 8px;
            padding: 2rem;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            margin-bottom: 2rem;
        }
        
        .pricing h2 {
            color: #ff6b6b;
            text-align: center;
        }
        
        .price {
            font-size: 2.5rem;
            text-align: center;
            margin: 1rem 0;
            color: #333;
        }
        
        .features {
            list-style-type: none;
            padding: 0;
        }
        
        .features li {
            padding: 8px 0;
            border-bottom: 1px solid #eee;
        }
        
        .features li:last-child {
            border-bottom: none;
        }
        
        .cta-button {
            display: block;
            width: 100%;
            padding: 12px;
            background-color: #ff6b6b;
            color: white;
            text-align: center;
            text-decoration: none;
            border-radius: 4px;
            font-weight: bold;
            margin-top: 1rem;
            transition: background-color 0.3s;
        }
        
        .cta-button:hover {
            background-color: #ff5252;
        }
        
        .testimonials {
            background-color: white;
            border-radius: 8px;
            padding: 2rem;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }
        
        footer {
            text-align: center;
            padding: 2rem 0;
            background-color: #333;
            color: white;
        }
    </style>
</head>
<body>
    <header>
        <h1>Amizades que Evoluem</h1>
        <p>Conheça pessoas incríveis que podem se tornar mais que amigos</p>
    </header>
    
    <div class="container">
        <div class="pricing">
            <h2>Plano Premium</h2>
            <div class="price">R$150/mês</div>
            <ul class="features">
                <li>✔ Perfil destacado na plataforma</li>
                <li>✔ Acesso a eventos exclusivos</li>
                <li>✔ Compatibilidade com seus interesses</li>
                <li>✔ Mensagens ilimitadas</li>
                <li>✔ Acompanhamento personalizado</li>
            </ul>
            <a href="#signup" class="cta-button">Assinar Agora</a>
        </div>
        
        <div class="testimonials">
            <h2>Histórias de Sucesso</h2>
            <p>"Conheci minha melhor amiga através dessa plataforma e hoje estamos noivos!" - Ana C.</p>
            <p>"Valeu cada centavo investido. Em 3 meses conheci alguém especial." - João P.</p>
        </div>
        
        <div id="signup" style="margin-top: 3rem;">
            <h2>Cadastre-se</h2>
            <form id="signupForm">
                <div style="margin-bottom: 1rem;">
                    <label for="name">Nome:</label>
                    <input type="text" id="name" name="name" required style="width: 100%; padding: 8px;">
                </div>
                
                <div style="margin-bottom: 1rem;">
                    <label for="email">Email:</label>
                    <input type="email" id="email" name="email" required style="width: 100%; padding: 8px;">
                </div>
                
                <div style="margin-bottom: 1rem;">
                    <label for="interests">Interesses:</label>
                    <textarea id="interests" name="interests" style="width: 100%; padding: 8px;" rows="4"></textarea>
                </div>
                
                <button type="submit" class="cta-button">Enviar Cadastro</button>
            </form>
        </div>
    </div>
    
    <footer>
        <p>© 2023 Amizades que Evoluem. Todos os direitos reservados.</p>
    </footer>
    
    <script>
        document.getElementById('signupForm').addEventListener('submit', function(e) {
            e.preventDefault();
            
            // Captura os dados do formulário
            const name = document.getElementById('name').value;
            const email = document.getElementById('email').value;
            
            // Aqui você normalmente enviaria para um servidor
            // Por enquanto, vamos apenas mostrar uma mensagem
            alert(`Obrigado, ${name}! Seu cadastro foi recebido. Enviaremos detalhes de pagamento para ${email} em breve.`);
            
            // Limpa o formulário
            document.getElementById('signupForm').reset();
        });
    </script>
</body>
</html>
