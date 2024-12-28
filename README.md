
# ⚡📲 Affichage de la Home Page d'une application web dédiée aux Simpsons 

## 1. Description
Ce projet est un exercice pratique en **HTML/CSS**.
**Flexbox** est utilisé pour une disposition dynamique des éléments du contenu principal.
Le projet utilise des conventions de **Responsive Design** pour une accessibilité sur tous supports.

---

## 2. Fonctionnalités
- Affichage d'un **Menu Burger** pour les résolutions d'écran inférieures à 900px en largueur.
Ce menu contextuel encapsule la barre de navigation et la déploie à la verticale.
Cette fonctionnalité a été conçue en usant uniquement d'éléments HTML et CSS, sans utilisation de JavaScript :

1. **HTML**

```<nav>
    <label for="burger">☰</label>
    <input type="checkbox" id="burger">
        <div class="burger_content">
            <a href="#">ACCUEIL</a>
            <a href="#">LE FILM</a>
            <a href="#">PERSONNAGES</a>
            <a href="#">HISTOIRE</a>
            <a href="#">MATT GROENING</a>
        </div>
</nav>
```

2. **CSS**

```label, #burger {
    display: none;
}

@media screen and (max-width: 900px) {
    .burger_content {
        display: none;
    }

    label {
        display: inline-block;
        font-size: 250%;
        cursor: pointer;
    }

    #burger:checked + .burger_content {
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    .burger_content a {
        margin: 7.5px;
        width: fit-content;
    }
}
```

---

## 3. Installation 

1. Accédez directement au projet via [ce lien](https://xylo87.github.io/Exos-Simpsons/)

2. Clonez ce projet depuis GitHub :
```bash
   git clone https://github.com/Xylo87/Exos-Simpsons.git
   cd Exos-Simpsons
```

## 4. Utilisation

Le Menu Burger est déployable en tant que **Checkbox** par un simple clic sur l'icône, si la résolution de l'écran est inférieure à 900px.

## 5. Auteur
Projet réalisé par Théo Arbogast (aka Xylo87).
N'hésitez pas à ouvrir une issue ou à me contacter pour toute suggestion ou question.