# Créattion d'un horloge en HTML/CSS et JS
## Le HTML

on crée trois div différentes, pour chaque aiguille de l'horloe, à l'intérieur d'une div cadran elle meme dan une div horloge,

on donne le nom de classe Horloge, cadran et aiguille minutes, secondes ou heures

## La CSS

pour chaque classe, une classe ici aussi

#### pour avoir les aiguilles qui tournes sur un axe et pas sur leurs centres:

on utilise cette propriété: 
```css
transform-origin: 100%;
```
*Autre* proporiété intéréssante:

```css
transform: rotate(90deg);
```
elle permet de remettre les aiguilles droites, c'est pour cet angle d'ailleurs qu'on a utilisé le plus 90 dans le code js suivant:
```js
 const secondesdegres = ((sec / 60) * 360) + 90;
 ```

 ## le Js

il y a déjà des méthodes get() pour les minutes etc, donc va les utiliser pour avoir l'heure actuelle, 
*Après* cela, il faut transformer les minutes en angle, on le fait avec un simple calcul
on applique ensuite la fonction "rotate()" (de css) à toutes les aiguilles selon les degrès 
