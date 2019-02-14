# To do :bookmark_tabs:

### To do é um aplicativo do tipo lista onde o usuário pode colocar as coisas em que ele tem para fazer no dia, na semana ou no mês.

To do é feito com **JavaScript**, **Jquery**, **HTML** e **CSS** com sincronização online usando **Firebase**.

**Portanto ele roda:**

| Plataforma                   | Estado        |
| -------------                | ------------- |
| Online (usando github pages) | em construção |
| Localmente (usando Electron) | em construção |
| Mobile (usando Ionic)        | em construção |


* A construção foi feita usando como base o livro *JavaScript and JQuery: Interactive Front-End Web Development* do autor *Jon Duckett* (Que livro awesome!) e seus exemplos. Mais especificamente os **capítulos 5, 6 e 7.**

### Imagens do projeto :)

https://github.com/wesley-cantarino/to_do/blob/master/images/img1.png

https://github.com/wesley-cantarino/to_do/blob/master/images/img2.png

https://github.com/wesley-cantarino/to_do/blob/master/images/img3.png

<hr>

## Como usar modo online com seu database?

1. Github:
    * Fazer fork desse repositório.
    * Em settings -> Github Pages -> Source -> master branch -> click em save. Depois disso seu site deve ser algo do tipo: https://<seu_nome>.github.io/to_do/

2. Firebase:
    * Acesse página do firebase e click em go to console.
    * Crie um novo projeto.
    * Procure por *"Adicionar o Firebase ao seu aplicativo da Web"* e copie o script.

3. De volta para github:
    * Procure por *js/firebase/config.js*
    * Cole o script e escoda seu ID. Deixe da seguinte forma:
    ```JavaScript
      // Initialize Firebase
      var config = {
        apiKey: "AIzaSyB9eE0NrFFrHVvrhsoDGhENGdiV91hNdrE",
        authDomain: id + ".firebaseapp.com",
        databaseURL: "https://" + id + ".firebaseio.com",
        projectId: id,
        storageBucket: "",
        messagingSenderId: "394049252253"
      };
      firebase.initializeApp(config);
    ```
4. Sua página online:
    * Acesse sua página, digite seu ID na caixa de texto no inicio da página de pode atualizar a página.

    * Aperte em *"DOWN"* para sincronizar com seu database e em *"UP"* para enviar para seu database.
