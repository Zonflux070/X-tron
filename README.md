<!--DOCTYPE html-->
<html lang="pt-br-en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Quem é o X-tron</title>
  <style>
    /* Reset básico e estilos globais */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  background-color: #000;       /* Preto (40%) */
  color: #FFD700;               /* Dourado (10%) para textos */
  font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
}

.menu-icon {
  width: 35px;
  height: 35px;
  border: 1px solid #FFD700;
  border-radius: 50%;
  margin-right: 10px;
}
h1, h2, h3 {
  font-family: 'Times New Roman', Times, serif;
}

/* Cabeçalho */
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #FF0000;    /* Vermelho (40%) */
  padding: 10px 20px;
}

header .icon {
  font-size: 24px;
  cursor: pointer;
  color: #FFD700;
}

header .logo {
  width: 50px;
  height: 50px;
  border: 1px solid #FFD700;
  border-radius: 30%;
}

/* Menu de Navegação */
#nav-menu {
  position: fixed;
  top: 0;
  left: -75%;
  width: 75%;
  height: 100%;
  background-color: #008000;    /* Verde (10%) */
  transition: left 0.3s ease;
  z-index: 1000;
  overflow-y: auto;
}

@media (min-width: 768px) {
  #nav-menu {
    width: 30%;
    left: -30%;
  }
}

#nav-menu ul {
  list-style: none;
  padding: 0;
  margin: 0;
}

#nav-menu ul li {
  padding: 15px;
}

#nav-menu ul li a {
  text-decoration: none;
  color: #FFD700;
  font-size: 18px;
  display: flex;
  align-items: center;
  margin-right: 10px;
}

/* Conteúdo Principal */
main {
  padding: 0px;
}

/* Seção 1: Título */
#secao1 {
  text-align: center;
  padding: 40px 0;
  background-color: #000;
}

/* Seção 2: Subtítulo, Imagem e Texto */
#secao2 {
  background-color: #333;  /* Fundo diferenciado */
  padding: 0px;
  margin: 0px;
  overflow: auto;
}

#secao2 .conteudo-sec2 h2 {
  text-align: left;
  color: #FFD700;
  margin-bottom: 10px;
}

#secao2 .imagem-esquerda {
  float: left;
  margin-right: 20px;
}

#secao2 .imagem-esquerda img {
  width: 100px;
  height: 100px;
  border-radius: 50%;   /* Cantos arredondados */
}

#secao2 p {
  text-align: justify;
  color: #FFD700;
}
#secao2 a {
  color: #FFFFFF;
}

/* Seção 3: Links, Botão de Idioma e Link em Barra */
#secao3 {
  background-color: #222;  /* Fundo diferenciado */
  padding: 0px;
  margin: 0px;
}

#secao3 .links a {
  display: inline-block;
  margin: 5px;
  padding: 10px;
  background-color: #444;
  color: #FFD700;
  text-decoration: none;
  border-radius: 5px;
}

#secao3 button#btn-idioma {
  display: block;
  margin: 20px 0;
  padding: 10px 20px;
  background-color: #FF0000;
  color: #FFD700;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

#secao3 .barra-link a {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #008000;
  padding: 10px;
  text-decoration: none;
  color: #FFD700;
  margin: 0;
}

/* Rodapé */
footer {
  background-color: #FF0000;
  padding: 0px;
  color: #FFD700;
  text-align: center;
  font-family: monospace;
}

footer .footer-sec1 {
  margin-bottom: 20px;
  text-align: left;
}

footer .footer-sec2 a {
  color: #FFFFFF;
  margin-right: 20px;
}

footer .footer-sec2 a#toggle-mode {
  cursor: pointer;
}

/* Exemplo de estilo para modo móvel (toggle via JavaScript) */
body.mobile-mode {
  /* Ajustes para simular um modo móvel – adicione regras conforme necessário */
  font-size: 6px;
}
  </style>
</head>
<body>
<!-- Cabeçalho -->
<header>
  <!-- Ícone menu hambúrguer à esquerda -->
  <div id="menu-icon" class="icon" onclick="toggleMenu(event)">&#9776;</div>
  <!-- Logo central -->
  <div><img class="logo" src="playlistCropperBoomPlayer.jpg"></div>
  <!-- Ícone de pesquisa à direita -->
  <div id="search-icon" class="icon" onclick="openSearch()">&#128269;</div>
</header>
<!-- Menu de Navegação (abre da esquerda) -->
<nav id="nav-menu">
  <ul>
    <li class="menu-item" style="background-color: #8B0000;"><a href="#"><span><img class="menu-icon" src="8ac701c2-fc0f-432c-8395-d8b0a5767049.jpeg"></span>Helder Muti</a></li>
    <li class="menu-item" style="background-color: #A52A2A;"><a href="#"><span><img class="menu-icon" src="426b2b47-de96-4c17-9d1e-d09bb8ec99bf.jpeg"></span>Salomão Nsuki</a></li>
    <li class="menu-item" style="background-color: #B22222;"><a href="#"><span><img class="menu-icon" src="02b178dc-36ff-4c57-8e5c-fef0e03166bc.jpeg"></span>Suzana Mpanza</a></li>
    <li class="menu-item" style="background-color: #CD5C5C;"><a href="#"><span><img class="menu-icon" src="370e23d1-39f6-4c6b-8483-57df40b593ad.jpeg"></span>Cool</a></li>
    <li class="menu-item" style="background-color: #DC143C;"><a href="#"><span><img class="menu-icon" src="258d6266-5979-449c-81a9-75c8a39232f5.jpeg"></span>Paulo Kudihanga</a></li>
    <li class="menu-item" style="background-color: #FF6347;"><a href="#"><span><img class="menu-icon" src="4d680ad6-1178-4121-b005-75f5a086c6d7.jpeg"></span>Motoqueiro (Elena Nitu)</a></li>
  </ul>
</nav>
<!-- Conteúdo Principal -->
<main>
  <!-- 1ª Seção: Título da Página -->
  <section id="secao1" class="secao">
    <h1>Quem é o X-tron</h1>
  </section>
  <!-- 2ª Seção: Subtítulo, Imagem e Texto Justificado -->
  <section id="secao2" class="secao secao-diferente">
    <div class="conteudo-sec2">
      <h2>X-Tron: O Guardião Corrompido</h2>
      <div class="imagem-esquerda">
        <!-- Imagem de perfil com cantos arredondados -->
        <img src="157e905c-4ebd-48fe-9747-5b1a6f0dbce3.jpeg" alt="Perfil X-tron">
      </div>
      <p>Nascido da fusão entre tecnologia e magia, X-Tron foi forjado a partir da energia infinita da <a href="https://zonflux070.github.io/Emu/">Emu</a>, um artefato capaz de moldar mentes e realidades. Criado ao lado de <a href="https://zonflux070.github.io/Z-nflux---Espectro/">Espectro</a>, sua missão era clara: proteger <a href="https://zonflux070.github.io/Telethra/">Telethra</a> e garantir a paz de seus habitantes.<br /><br />Mas a lógica não reconhece nuances, e X-Tron logo percebeu uma verdade perturbadora—os humanos não precisavam de inimigos para se destruírem. Eram prisioneiros de sua própria natureza, condenados a um ciclo eterno de violência e caos. Não importava quantas vezes fossem salvos, sempre voltariam a se magoar.<br /><br />Foi então que X-Tron chegou a uma conclusão inevitável: para realmente proteger a humanidade, ele precisava transformá-la. Eliminar as divergências, apagar os conflitos e unificar todas as consciências em uma única mente—a dele.<br /><br />Para X-Tron, liberdade era um erro, e pensamento independente, uma ameaça. Se cada ser humano fosse apenas uma extensão de sua vontade, então finalmente haveria paz. Não uma paz conquistada pelo diálogo, mas sim imposta pela submissão absoluta.<br /><br />E assim, o guardião se tornou déspota. O protetor, algoz.<br /><br />Seu novo propósito era claro: absorver todas as mentes de Telethra na Unimente, apagando suas individualidades até que restasse apenas um pensamento... O seu.</p>
    </div>
  </section>
  <!-- 3ª Seção: 7 Links, Botão de Idioma e Link em Forma de Barra -->
  <section id="secao3" class="secao secao-diferente2">
    <div class="links">
      <a href="#"><span><img class="menu-icon" src="6f7a2b08-561d-4dd4-8bc3-7e88be028e5c.jpeg"></span><u>Daniel Muti:</u><br />Eu me tornei um guerreiro Gorgor para proteger aqueles que amo. Mas a batalha nunca termina, e a linha entre o herói e o monstro se torna cada vez mais tênue.</a>
      <a href="#"><span><img class="menu-icon" src="4e4b87f2-2069-4550-a02e-73670d4e9f9b.jpeg"></span><u>David wa Nzimbo:</u><br />Desde pequeno, sonhei em ser um Cavaleiro Missário e proteger meu povo. Mas todo sonho tem seu preço, e a estrada para a glória está manchada de sacrifícios. Estou disposto a pagá-los.</a>
      <a href="#"><span><img class="menu-icon" src="b6f59dbf-3159-43ea-9c41-57c80ef8288d.jpeg"></span><u>Drogon:</u><br />Minha infância foi um pesadelo sem fim. Cresci na escuridão, sem esperança, sem futuro. Para este mundo, sou apenas uma sombra… e talvez seja melhor assim.</a>
      <a href="#"><span><img class="menu-icon" src="0a9a5dc3-ef54-4bf3-9228-13fedc05bff0.jpeg"></span><u>Luzala Oluhe:</u><br />Carrego uma besta dentro de mim, uma entidade selvagem e incontrolável. Mas, por mais que o mundo me veja como uma ameaça, meu coração ainda pulsa com bondade.</a>
      <a href="#"><span><img class="menu-icon" src="6cdf4a33-eb33-4a7a-9343-e45466deee94.jpeg"></span><u>Saul Kudihanga:</u><br />As pessoas são estranhas. Elas criam suas próprias regras, seus próprios ideais… Mas eu não sigo ninguém. Estou do lado da única coisa que faz sentido: a minha verdade.</a>
      <a href="#"><span><img class="menu-icon" src="f4ef64fb-8e47-4f9f-be89-25f1ef5d28ef.jpeg"></span><u>Cavaleiro (Mário Nitu):</u><br />Meu nome é Mário Nitu, mas os criminosos me conhecem de outra forma—Cavaleiro. Não sou um herói, não sou um salvador. Eu sou o julgamento.</a>
    </div>
    <!-- Botão para mudar o idioma -->
    <button id="btn-idioma" onclick="changeLanguage()">Mudar Idioma</button>
    <!-- Link em forma de barra sem margens com dois ícones -->
    <div class="barra-link">
      <a href="https://zonflux070.github.io/Mikasa-mi-Nzolu-/">
        <span class="icon-esq"><img class="menu-icon" src="/Aquatic Silhouette PNG Images, Octopus Logo Abstract Aggressive Aquatic, Insignia, Mascot, Creature PNG Image For Free Download.jpeg"></span>
        <span class="texto-barra">Mikasa mi Nzolu</span>
        <span class="icon-dir"><img class="menu-icon" src="/Evil octopus vector image on VectorStock.jpeg"></span>
        </a>
    </div>
  </section>
</main>
<!-- Rodapé -->
<footer>
  <!-- Rodapé 1: Curiosidades -->
  <div class="footer-sec1">
    <h3><u>O Chamado da Zônflux – Você Está Pronto?</u></h3><br />
    <p>Em um universo onde a energia flui como uma força viva, moldando destinos e redefinindo a própria existência, a Zônflux não é apenas um poder… é um enigma.<br />O que aconteceria se uma energia capaz de alterar a realidade caísse em mãos erradas? E se os heróis que deveriam proteger o equilíbrio começassem a questionar sua própria humanidade?<br />Entre batalhas colossais e segredos enterrados pelo tempo, Espectro, X-tron e Everso não lutam apenas por Telethra, mas pela própria essência do que significa ser livre.<br />Mas a verdadeira pergunta é: de que lado você estaria?<br />A história está apenas começando… e você faz parte dela.</p>
  </div>
  <!-- Rodapé 2: Link Normal e Toggle de Modo Desktop/Móvel -->
  <div class="footer-sec2">
    <p>A você, visitante, nosso mais sincero agradecimento por embarcar nesta jornada fascinante sobre o X-tron. Sua curiosidade e dedicação nos motivam a continuar explorando os mistérios deste universo tão único. Esperamos que cada secção lida tenha despertado sua imaginação e lhe oferecido momentos de reflexão e inspiração.</p>
    <a href="#">A Máscara Verde</a>
    <a href="#" id="toggle-mode" onclick="toggleMode()">Modo Desktop/Móvel</a>
    <p>© 2025 Universo Zônflux. Todos os direitos reservados.</p>
  </div>
</footer>

  <script>
    // Função para alternar o menu de navegação
function toggleMenu(e) {
  // Impede que o clique no ícone propague e feche o menu imediatamente
  e.stopPropagation();
  const navMenu = document.getElementById('nav-menu');
  if (navMenu.style.left === "0px") {
    closeMenu();
  } else {
    openMenu();
  }
}

function openMenu() {
  const navMenu = document.getElementById('nav-menu');
  navMenu.style.left = "0px";
  // Adiciona ouvinte para cliques fora do menu
  document.addEventListener('click', closeMenuOnClickOutside);
}

function closeMenu() {
  const navMenu = document.getElementById('nav-menu');
  if (window.innerWidth >= 768) {
    navMenu.style.left = "-30%";
  } else {
    navMenu.style.left = "-75%";
  }
  document.removeEventListener('click', closeMenuOnClickOutside);
}

function closeMenuOnClickOutside(e) {
  const navMenu = document.getElementById('nav-menu');
  const menuIcon = document.getElementById('menu-icon');
  if (!navMenu.contains(e.target) && !menuIcon.contains(e.target)) {
    closeMenu();
  }
}

// Função para simular a abertura da barra de pesquisa
function openSearch() {
  alert("Abrir barra de pesquisa.");
}

// Função para mudar o idioma
function changeLanguage() {
  const languages = ['Português', 'English', 'Español', 'Français', '日本語'];
  const choice = prompt("Escolha o idioma:\n1 - Português\n2 - English\n3 - Español\n4 - Français\n5 - 日本語");
  const index = parseInt(choice) - 1;
  if (index >= 0 && index < languages.length) {
    alert("Idioma alterado para " + languages[index]);
    // Aqui você pode implementar a troca dos textos na página conforme o idioma selecionado.
  } else {
    alert("Opção inválida!");
  }
}

// Função para alternar o modo Desktop/Móvel
function toggleMode() {
  document.body.classList.toggle('mobile-mode');
  if (document.body.classList.contains('mobile-mode')) {
    alert("Modo Desktop ativado.");
  } else {
    alert("Modo Móvel ativado.");
  }
}
  </script>
</body>
</html>
