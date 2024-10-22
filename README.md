// ==Script de Usuário==
// @nome Alura Destruidor
// @namespace https://cursos.alura.com.br/
// @versão 2024-09-23
// @description nuh uh eu não quero mais fazer Alura :sob:
// @autor wwwwwwwwwwwww
// @match https://cursos.alura.com.br/course/*/task/*
// @icon https://i.imgur.com/gP1LZq9.png
// @grant nenhum
// ==/Script do Usuário==

(função() {
    'usar estrito';
    const marca_d'água = document.querySelector('.formattedText');
    water_mark.innerHTML = 'sussy baka entre nós';

    deixe cookies = document.cookie;

    deixe atual_url = window.location.href;

    deixe next_lesson_button = document.getElementsByClassName("bootcamp-next-button")[0];

    se (botão_próxima_lição){
        deixe next_lesson_link = next_lesson_button.getAttribute('href');
        deixe partes = actual_url.split('/');
        deixe lessonName = partes[4];
        deixe lessonId = partes[6];
        console.log(`[DEBUG] Nome_da_lição: ${lessonName} ID_da_lição: ${lessonId} `);

        fetch(`https://cursos.alura.com.br/course/${lessonName}/task/${lessonId}/mark-video`, {
          método: 'POST',
          credenciais: 'incluir',
          cabeçalhos: {
             'Tipo de conteúdo': 'aplicativo/json',
             'Cookie': biscoitos
          }}).então(dados => {
          console.log("[DEBUG] Lição concluída!")
          })

        setTimeout(next_lesson_button.click(), 4000); // Modifica o tempo para 4 segundos
    } outro {
        alert("Botão Próxima Lição não encontrado :( tem certeza de que está na página correta?");
    }
})();
