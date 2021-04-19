# Cours sur le formulaire pour les réseaux
## Comment faire un formulaire web
Ce dépôt sert à apprendre à gérer les propriétés html, css et le langage js

Exemple de code html :

```html
<h1>
            <strong>insight</strong> 
             <p>PSG - Formulaire - Inscription</p>
        </h1>
    </header>
    <main>
        <section>
            <h2>Inscrivez vous</h2>
            <a href="#" title="Accéder à votre espace" class="connect">Accéder ici</a>
        </section>
        <p class="warning">Warning</p>
        <div class="form" role="form">
            <form action="" method="get">
                <label for="nom">Votre nom</label>
                <input type="text" name="nom" id="nom" placeholder="Votre nom" aria-required="true" autofocus>
                <label for="prenom">Votre prenom</label>
                <input type="text" name="prenom" id="prenom" placeholder="Votre prenom" aria-required="true">
                <label for="email">Votre email</label>
                <input type="email" name="email" id="email" placeholder="Votre email" aria-required="true">
                <label for="mdp">Votre mot de passe</label>
                <input type="password" name="mdp" id="mdp" placeholder="Votre mot de passe" aria-required="true">
                <input type="submit" value="Envoyer votre inscription">
```
### Exemple de code CSS

```css
@import url('https://fonts.googleapis.com/css?family=Dosis:300,400,500,600');
/* reset */
html{
    font-size: 62.5%;
    margin: 0;
    scroll-behavior: smooth;
}
body{
    font: 1.6rem 'Dosis', sans-serif;
    margin: 0;
}
h1,h2,h3,p,ul,ol{
    margin: 0;
    font-weight: 300;
    padding: 0;
    list-style: none;
    text-align: center;
}
a{
    text-decoration: none;
    color: #222;
}
*{
    box-sizing: border-box;
}
```
### Exemple de code js

```js
document.addEventListener("DOMContentLoaded",()=>{
    console.log("hello")
    let btn, form, warning, connect, btn_form, traitement
    btn = document.querySelector(".connect")
    form = document.querySelector(".form")
    warning = document.querySelector(".warning")
    btn_form = document.getElementsByTagName("input")[4]
    console.log(btn_form)
    /* affectation de valeur et de type */
    console.log(btn.innerText)
