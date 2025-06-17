/* Estilos Gerais */
body {
    font-family: 'Arial', sans-serif;
    line-height: 1.6;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
    color: #333;
    display: flex;
    flex-direction: column;
    min-height: 100vh; /* Garante que o footer fique no final */
}

.container {
    width: 80%;
    margin: auto;
    overflow: hidden;
    padding: 0 20px;
    flex-grow: 1; /* Faz o conteúdo principal crescer e empurrar o footer para baixo */
}

/* Cabeçalho e Navegação */
header {
    background: #333;
    color: #fff;
    padding-top: 30px;
    min-height: 70px;
    border-bottom: #0779e4 3px solid;
}

header a {
    color: #fff;
    text-decoration: none;
    text-transform: uppercase;
    font-size: 16px;
}

header ul {
    padding: 0;
    list-style: none;
    text-align: center; /* Centraliza os itens da navegação */
}

header li {
    display: inline; /* Coloca os itens da navegação na mesma linha */
    padding: 0 20px 0 20px;
}

header #branding {
    text-align: center; /* Centraliza o título do site */
    margin-bottom: 10px; /* Espaço abaixo do título */
}

header #branding h1 {
    margin: 0;
    font-size: 24px;
}

header nav {
    margin-top:10px;
}

header .highlight, header .current a {
    color: #0779e4;
    font-weight: bold;
}

header a:hover {
    color: #ccc;
    font-weight: bold;
}

/* Seções de Conteúdo */
.educational-section {
    background-color: #fff;
    padding: 25px;
    margin-top: 20px;
    margin-bottom: 20px;
    border-radius: 8px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
}

.educational-section h1 {
    color: #0056b3; /* Azul escuro para títulos principais da seção */
    border-bottom: 2px solid #eee;
    padding-bottom: 10px;
    margin-top: 0;
}

.educational-section h2 {
    color: #007bff; /* Azul mais claro para subtítulos */
    margin-top: 20px;
}

.educational-section p, .educational-section ul {
    margin-bottom: 15px;
}

.educational-section ul {
    list-style-position: inside;
    padding-left: 0;
}

.educational-section li {
    margin-bottom: 8px;
}

.call-to-action {
    display: inline-block;
    background-color: #0779e4;
    color: #fff;
    padding: 10px 20px;
    text-decoration: none;
    border-radius: 5px;
    margin-top: 15px;
    transition: background-color 0.3s ease;
}

.call-to-action:hover {
    background-color: #0056b3;
}

/* Rodapé (Footer) */
footer {
    background-color: #222; /* Um pouco mais escuro que o header */
    color: #bbb;
    text-align: center;
    padding: 30px 20px; /* Aumentei o padding para mais espaço */
    margin-top: auto; /* Garante que ele seja empurrado para o final da página */
    font-size: 0.9em;
    border-top: #0779e4 3px solid;
}

footer p {
    margin: 8px 0;
}

footer nav {
    margin-top: 10px;
}

footer nav a {
    color: #07A0F0; /* Cor um pouco mais clara para os links do footer */
    text-decoration: none;
    margin: 0 10px;
    transition: color 0.3s ease;
}

footer nav a:hover {
    color: #fff;
    text-decoration: underline;
}

/* Botão "Voltar ao Topo" (opcional) */
#voltar-topo {
    display: none; /* Oculto por padrão */
    position: fixed;
    bottom: 20px;
    right: 30px;
    z-index: 99;
    border: none;
    outline: none;
    background-color: #0779e4;
    color: white;
    cursor: pointer;
    padding: 12px 15px;
    border-radius: 50%; /* Deixa redondo */
    font-size: 18px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.2);
    transition: background-color 0.3s ease, opacity 0.3s ease;
}

#voltar-topo:hover {
    background-color: #0056b3;
}

/* Responsividade Básica */
@media(max-width: 768px){
    header #branding,
    header nav,
    header nav ul,
    header nav li {
        float: none;
        text-align: center;
        width: 100%;
    }

    header {
        padding-bottom: 20px;
    }

    .container {
        width: 95%;
        padding: 0 10px;
    }
}