# CSS

### ordre des sources : (priorité)
	1. style en ligne (style html)
	2. internes (style au sein du fichier html)
	3. externes (style fichier css externe)
	4. utilisateur ( préférences navigateur)
	
### ordre de spécificité : (priorité)
	1. sélecteurs de type (p, h1, etc) FAIBLE
	2. sélecteurs de classe (.ma-classe) MOYENNE
	3. sélecteurs d'id ELEVEE
	4. Styles en ligne PLUS HAUTE
	5. Enfin, les déclarateurs avec !important

### origine des styles:
	styles de l'auteur : celui du dev dans le CSS
	de l'user : dans son nav
	du nav : par défaut dans le nav

**Si deux règles de même niveau, alors c'est la dernière qui s'applique.**

## HERITAGE

## Propriété héritables :
	* Couleur de texte (color)
	* Polices (font-family, font-size, font-style, font-weight)
	* Hauteur de ligne (line-height)
	* Alignement du texte (text-align)
	* Visibilité (visibility)
	
## Propriétés non-héritables :
	* Margin
	* Padding
	* width & height
	* background
	* border

## Forcer ou annuler l'héritage :
	* inherit (force)
		* ex : p { border: 1px solid black; } span { color: inherit }
		* (hérite des borders du parent)
	* initial (annule l'héritage)
		* ex : p { color: red; } span { color: initiial }
		* (annule l'héritage de la couleur du parent)
	* unset (applique si héritée par défaut, sinon réinitialise la propriété à sa valeur par défaut)
		* ex : on a une prop button avec un certain style.
		* Si on add une classe à un autre button, on peut utiliser l'attribut unset pour qu'il réinitialise à son héritage par défaut de son parent.
