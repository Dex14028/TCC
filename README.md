<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>StamPro - Home</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    

    <style>
        :root {
            --bg-body: #EFF4FD; --bg-header: #BDCFFC; --bg-sidebar: #BDCFFC;
            --bg-card: #DEE6F8; --bg-btn: #BDCFFC; --text-main: #1A202C;
            --primary-blue: #4A90E2; --shadow: rgba(0,0,0,0.1);
        }
        body.dark-mode {
            --bg-body: #121212; --bg-header: #1F2937; --bg-sidebar: #1F2937;
            --bg-card: #374151; --bg-btn: #4A90E2; --text-main: #F3F4F6;
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Poppins', sans-serif; transition: 0.3s; }
        body { background-color: var(--bg-body); color: var(--text-main); height: 100vh; display: flex; flex-direction: column; overflow: hidden; }
        
        header { background-color: var(--bg-header); height: 70px; display: flex; align-items: center; justify-content: space-between; padding: 0 20px; z-index: 10; }
        
        .logo { font-weight: 800; font-size: 1.3rem; display: flex; align-items: center; gap: 10px; }
        .logo img { width: 40px; height: auto; border-radius: 5px; }

        .container { display: flex; flex: 1; height: calc(100vh - 70px); }
        .sidebar { width: 200px; background-color: var(--bg-sidebar); padding: 30px 20px; display: flex; flex-direction: column; justify-content: space-between; }
        
        /* Ajuste do grid para dar mais destaque à direita */
        .content { flex: 1; padding: 40px; position: relative; display: grid; grid-template-columns: 0.8fr 1.2fr; align-items: center; gap: 40px; }
        
        .top-buttons { position: absolute; top: 20px; right: 20px; display: flex; flex-direction: column; gap: 10px; z-index: 5; }
        .btn-link { 
            display: block; width: 180px; padding: 12px 0; background-color: var(--bg-btn); 
            color: var(--text-main); text-align: center; text-decoration: none; 
            border-radius: 20px; font-weight: 700; box-shadow: 2px 2px 5px var(--shadow);
        }
        .btn-link:hover { filter: brightness(1.1); transform: scale(1.05); }

        /* --- LOGO CENTRAL AMPLIADA --- */
        .big-logo-container { text-align: center; display: flex; flex-direction: column; align-items: center; }
        .big-logo-img { 
            width: 100%; 
            max-width: 500px; /* Tamanho consideravelmente maior */
            height: auto; 
            margin-bottom: -10px; /* Aproxima o texto da imagem */
            filter: drop-shadow(0px 10px 15px var(--shadow));
        }
        .big-logo { font-size: 5rem; font-weight: 900; line-height: 1; margin-top: 10px; }
        .big-logo span { color: var(--primary-blue); }
    </style>
</head>
<body>
    <header>
        <div class="logo">
            <img src="https://uploads.onecompiler.io/43s363kb2/44cbs86da/ema.png" alt="StamPro Logo" class="Imgp"> 
            StamPro
        </div>
        <button onclick="document.body.classList.toggle('dark-mode')" style="background:none; border:none; cursor:pointer; font-size:1.5rem; color:inherit;">
            <i class="fa-solid fa-moon"></i>
        </button>
    </header>

    <div class="container">
        <aside class="sidebar">
            <div>
                <p style="opacity: 0.7; font-size: 0.9rem;">MENU PRINCIPAL</p>
                <br>
                <a href="login.html" style="text-decoration:none; color:inherit; font-weight:bold; display: flex; align-items: center; gap: 10px;">
                    <i class="fa-solid fa-right-to-bracket"></i> Entrar
                </a>
            </div>
        </aside>

        <main class="content">
            <div class="top-buttons">
                <a href="login.html" class="btn-link">Entrar</a>
                <a href="cadastro.html" class="btn-link">Cadastrar</a>
            </div>

            <div style="background:var(--bg-card); padding:40px; border-radius:30px; box-shadow: 5px 5px 15px var(--shadow);">
                <h2 style="margin-bottom: 15px;">Bem-vindo!</h2>
                <p style="font-size: 1.1rem; line-height: 1.6;">O <strong>StamPro</strong> é a solução definitiva para sua gestão profissional, unindo rapidez e simplicidade em um só lugar.</p>
            </div>

            <div class="big-logo-container">
                <img src="https://uploads.onecompiler.io/43s363kb2/44cbs86da/ema.png" alt="Ilustração StamPro" class="big-logo-img">
                <h1 class="big-logo">Stam<span>Pro</span></h1>
            </div>
        </main>
    </div>
</body>
</html>
