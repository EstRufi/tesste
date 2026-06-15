[index.html](https://github.com/user-attachments/files/28973434/index.html)[index.html](https://github.com/user-attachments/files/28973459/index.html)
<!DOCTYPE html>
<html lang="pt-br">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <script type="module" src="./js/app.js" defer></script>
    <title>Planeta Vegano</title>
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link rel="stylesheet" href="./css/reset.css">
    <link rel="stylesheet" href="./css/style.css">
</head>

<body>
    <header>
        <img src="./img/logo_planetaVerde.png" alt="Planeta Verde com uma planta no meio">
        <nav class="header">
            <img src="./img/Search.svg" alt="Foto de uma lupa">
            <input type="text" placeholder="Pesquise Produtos veganos aqui">
        </nav>
    </header>
    <main>
        <section>
            <ul id="carrossel">

            </ul>
        </section>

        <div class="listaButoes">
            <button class="bnt-categoria">Alimento</button>
            <button class="bnt-categoria">Cosméticos</button>
            <button class="bnt-categoria">Vestuário</button>
            <button class="bnt-categoria">Acessório</button>
            <button class="bnt-categoria">Higiene Pessoal</button>
            <button class="bnt-categoria">Limpeza</button>
        </div>
    </main>
    <footer>
        <nav class="footer">
            <img src="./img/logo_empresa.png" alt="Ant-Bug">

            <small>&copy;2026 -  ANT-BUG - Todos os direitos reservados</small>
        </nav>
        <div class="maisInformacao">
            <p>Mais informações</p>
            <div class="link">
                <a href="https://github.com/PyetroSouza/pi_ant-bug">
                    <p>GitHub</p>
                    <img src="./img/GitHub.png" alt="Logo do GitHub">
                </a>
            </div>

        </div>
    </footer>
</body>

</html>

[style.css](https://github.com/user-attachments/files/28973448/style.css):root{
    --fundo-verde: #659860;
    --cor-cards-bage: #f7f8f2;
    --verde-butao: #e2ece4;
    --houver-verde-escuro:#366b41;
    --bage-escuro: #E6E3DA; 
}

/* Header */

header{
    width: 100%;
    min-height: 150px;
    background-color: var(--cor-cards-bage);
    display: flex;
    padding: 20px;
    gap: 78px;
}

.header{
    display: flex;
    align-items: center;
    background-color: var(--bage-escuro);
    width: 60%;
    height: 40px;
    margin: auto;
    justify-content: left;
    border-radius: 10px;
}

.header img{
    width: 50px;
}

.header input{
    border: none;
    width: 100%;
    height: 100%;
    background-color: var(--bage-escuro);
    font-size: 25px;
    border-radius: 10px;
}

/* :focus serve para quando algo está ativado.
    e o outline: nome; serve para tirar o contorno visual de algo
*/
.header input:focus{
    outline: none;
}

/* Main */

main{
    width: 100%;
    background-color: var(--fundo-verde);
}

/* Carossel - main */
section{
    height: 260px;
    width: 100%;
    overflow: hidden;
    background-color: var(--verde-butao);
}

#carrossel{
    display: flex;
    gap: 30px;
    padding: 0;
    margin: 0;
}

.imageProduto{
    object-fit: cover;
    height: 260px;
    padding: 20px;
}

/* Buttoes - main */

.listaButoes{
    display: flex;
    justify-content: center;
    gap: 32px;
}

.bnt-categoria{
    height: 55px;
    width: 230px;
    background-color: var(--cor-cards-bage);
    border: none;
    border-radius: 213.5px;
    font-size: 30px;
    margin-top: 10px;
    margin-bottom: 50px;
}

.bnt-categoria:hover{
    background-color: var(--houver-verde-escuro);
    transition: 0.2s;
    color: #fafafa;
}

/* Footer */

footer{
    display: flex;
    height: 100%;
    background-color: var(--cor-cards-bage);
}

.footer{
    flex-direction: row;
    width: 60%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    font-size: 20px;
}

.footer img{
    width: 420px;
    height: 165px;
}

.maisInformacao{
    display: flex;
    flex-direction: column;
    width: 40%;
    background-color: #b31b1b;
    align-items: end;
    justify-content: center;
    padding-right: 100px;
    gap: 10px;
    text-align: center;
    font-size: 25px;
    
}

.link{
    background-color: var(--verde-butao);
    display: flex;  
    justify-content: center;
    padding: 1px;
    width: 150px;
    height: 65px;
    flex-direction: row;
    border-radius: 25px;
    font-size: 20px;
}

.link img{
    width: 60px;
    height: 57px;
}

a{
    display: flex;
    text-decoration: none;
    color: inherit;    
    align-items: center;
}

