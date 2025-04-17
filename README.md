<!DOCTYPE html>
<html lang="pt-BR">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mario Bros Encanadores</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Press+Start+2P&family=Roboto:wght@400;700&display=swap" rel="stylesheet">
</head>

<body>
    <div class="mascara-formulario" onclick="esconderForm()"></div>

    <header class="header">
        <img src="./img/logo-header.png" alt="Logo do Mário Bros" class="logo-header">
        <nav>
            <a href="#" class="active">Home</a>
            <a href="#servicos">Nossos Serviços</a>
            <a href="#" onclick="mostrarForm()">Fale Conosco</a>
        </nav>
        <div class="menu-mobile" onclick="toggleMenu()">
            <i class="fas fa-bars"></i>
        </div>
    </header>

    <div class="caixa-mae">
        <div class="caixa-principal">
            <img src="./img/logo.png" alt="Logo do Mário Bros" class="logo-mario">
            <h1>Encanadores Mario & Luigi</h1>
            <p class="slogan">Resolvendo seus Problemas com Estilo!</p>
            <p class="descricao">Você já se encontrou em uma situação de emergência com encanamento? Torneiras que não param de pingar? Vazamentos inesperados? Não se preocupe! Os encanadores mais famosos do Reino dos Cogumelos estão aqui para ajudar!</p>

            <button onclick="mostrarForm()" class="btn-contato">
                <span>Entre em Contato</span>
                <i class="fas fa-chevron-right"></i>
            </button>
            
            <div class="destaques">
                <div class="destaque-item">
                    <i class="fas fa-check-circle"></i>
                    <span>Serviço Rápido</span>
                </div>
                <div class="destaque-item">
                    <i class="fas fa-star"></i>
                    <span>Garantia Total</span>
                </div>
                <div class="destaque-item">
                    <i class="fas fa-thumbs-up"></i>
                    <span>Preço Justo</span>
                </div>
            </div>
        </div>

        <div class="caixa-video">
            <video src="img/video.mp4" autoplay muted loop></video>
            <div class="mascara"></div>
        </div>
        
        <a href="https://wa.me/5527995303509?text=Ol%C3%A1%20quero%20ajuda%20dos%20irm%C3%A3os%20mario" class="link-whatsapp" target="_blank">
            <img src="./img/whatsapp.png" alt="link para o WhatsApp">
            <span>Fale Conosco</span>
        </a>
           
        <img src="./img/mario.png" alt="Mario e Luigi" class="imagem-mario-luigi">
        
        <form class="formulario-fale-conosco" onsubmit="enviarFormulario(event)">
            <h2>Fale Conosco</h2>
            <input placeholder="Seu Nome" type="text" required>
            <input placeholder="Seu Telefone" type="tel" required>
            <textarea placeholder="Digite seu problema aqui..." required></textarea>
            <button type="submit" class="btn-orcamento">
                <span>Pedir Orçamento</span>
                <i class="fas fa-paper-plane"></i>
            </button>
            <button type="button" class="btn-fechar" onclick="esconderForm()">
                <i class="fas fa-times"></i>
            </button>
        </form>
    </div>
    
    <section id="servicos" class="servicos">
        <h2>Nossos Serviços</h2>
        <div class="servicos-grid">
            <div class="servico-card">
                <div class="servico-icon">
                    <i class="fas fa-tools"></i>
                </div>
                <h3>Reparos Emergenciais</h3>
                <p>Consertamos vazamentos e problemas urgentes em tempo recorde!</p>
            </div>
            <div class="servico-card">
                <div class="servico-icon">
                    <i class="fas fa-faucet"></i>
                </div>
                <h3>Torneiras e Válvulas</h3>
                <p>Substituição e reparo em todos os tipos de torneiras e válvulas.</p>
            </div>
            <div class="servico-card">
                <div class="servico-icon">
                    <i class="fas fa-toilet"></i>
                </div>
                <h3>Vasos Sanitários</h3>
                <p>Conserto, substituição e instalação de vasos sanitários.</p>
            </div>
            <div class="servico-card">
                <div class="servico-icon">
                    <i class="fas fa-shower"></i>
                </div>
                <h3>Chuveiros e Banheiras</h3>
                <p>Instalação e manutenção de sistemas de chuveiro e banheira.</p>
            </div>
        </div>
    </section>
    
    <footer class="footer">
        <div class="footer-content">
            <img src="./img/logo.png" alt="Logo Mario Bros" class="footer-logo">
            <div class="footer-info">
                <p><i class="fas fa-phone"></i> (27) 99530-3509</p>
                <p><i class="fas fa-envelope"></i> contato@mariobrosencanadores.com</p>
                <p><i class="fas fa-map-marker-alt"></i> Reino dos Cogumelos, 123</p>
            </div>
            <div class="footer-social">
                <a href="#"><i class="fab fa-facebook"></i></a>
                <a href="#"><i class="fab fa-instagram"></i></a>
                <a href="#"><i class="fab fa-youtube"></i></a>
            </div>
        </div>
        <div class="footer-copyright">
            <p>&copy; 2023 Mario Bros Encanadores. Todos os direitos reservados.</p>
        </div>
    </footer>
    
    <script src="scripts.js"></script>
</body>
</html>
