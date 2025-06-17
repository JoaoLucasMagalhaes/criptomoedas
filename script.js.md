// Função para o botão "Voltar ao Topo"
window.onscroll = function() {scrollFunction()};

function scrollFunction() {
  let mybutton = document.getElementById("voltar-topo");
  if (document.body.scrollTop > 100 || document.documentElement.scrollTop > 100) {
    mybutton.style.display = "block";
    mybutton.style.opacity = "1";
  } else {
    mybutton.style.opacity = "0";
    // Adiciona um pequeno delay para a transição de opacidade antes de esconder
    setTimeout(function() {
        if (!(document.body.scrollTop > 100 || document.documentElement.scrollTop > 100)) {
            mybutton.style.display = "none";
        }
    }, 300); // 300ms, igual à duração da transição no CSS (se houver)
  }
}

// Quando o usuário clica no botão, rola para o topo do documento
function topFunction() {
  document.body.scrollTop = 0; // Para Safari
  document.documentElement.scrollTop = 0; // Para Chrome, Firefox, IE e Opera
}

// Adiciona o listener ao botão (se ele existir na página)
document.addEventListener('DOMContentLoaded', (event) => {
    let topButton = document.getElementById("voltar-topo");
    if (topButton) {
        topButton.addEventListener('click', topFunction);
    }
});