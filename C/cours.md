# <span style="color: #3498db">aprentissage du C</span>
### <span style="color: #3498db">instalation des prerequis</span>
- vs code commme ide https://code.visualstudio.com/Download

linux : installer le paquet **.deb** et extraire avec cette commande : **dpkg-deb -x nom_du_paquet.deb répertoire_destination**

rdv sur votre ide et ouvrir un terminal situé en haut a gauche a coté de la barre de recherche, tapé la commande suivant : **sudo apt install gcc**, puis pour voir si cela a correctement été installé vous pouvez faire **gcc --version**

### <span style="color: #3498db"> 1. les variables
les variable sont des contenant dans lequelle nous allons pouvoir stocké des donnée, 

il en existe plusieurs sorte, les voicie : 
Voici votre texte avec tous les éléments en gras maintenant en rouge :

Voici toutes les données formatées selon le modèle demandé :

- <span style="color: #e74c3c">char</span> pour des caractères signés de <span style="color: #e74c3c">1o</span> compris entre <span style="color: #e74c3c">-128 et 127</span>

- <span style="color: #e74c3c">unsigned char</span> pour des caractères non signés de <span style="color: #e74c3c">1o</span> compris entre <span style="color: #e74c3c">0 et 255</span>

- <span style="color: #e74c3c">short int</span> pour des entiers courts signés de <span style="color: #e74c3c">2o</span> compris entre <span style="color: #e74c3c">-32 768 et 32 767</span>

- <span style="color: #e74c3c">unsigned short int</span> pour des entiers courts non signés de <span style="color: #e74c3c">2o</span> compris entre <span style="color: #e74c3c">0 et 65 535
</span>

- <span style="color: #e74c3c">int</span> pour des entiers signés de <span style="color: #e74c3c">2o (16 bits) / 4o (32 bits)</span> compris entre <span style="color: #e74c3c">-32 768 à 32 767 (16 bits) / -2 147 483 648 à 2 147 483 647 (32 bits)</span>

- <span style="color: #e74c3c">unsigned int</span> pour des entiers non signés de <span style="color: #e74c3c">2o (16 bits) / 4o (32 bits)</span> compris entre <span style="color: #e74c3c">0 à 65 535 (16 bits) / 0 à 4 294 967 295 (32 bits)</span>

- <span style="color: #e74c3c">long int</span> pour des entiers longs signés de <span style="color: #e74c3c">4o</span> compris entre <span style="color: #e74c3c">-2 147 483 648 à 2 147 483 647</span>

- <span style="color: #e74c3c">unsigned long int</span> pour des entiers longs non signés de <span style="color: #e74c3c">4o</span> compris entre <span style="color: #e74c3c">0 à 4 294 967 295</span>

- <span style="color: #e74c3c">float</span> pour des nombres à virgule flottante simple précision de <span style="color: #e74c3c">4o</span> compris entre <span style="color: #e74c3c">≈ 3.4 × 10⁻³⁸ à 3.4 × 10³⁸</span>

- <span style="color: #e74c3c">double</span> pour des nombres à virgule flottante double précision de <span style="color: #e74c3c">8o</span> compris entre <span style="color: #e74c3c">≈ 1.7 × 10⁻³⁰⁸ à 1.7 × 10³⁰⁸</span>

- <span style="color: #e74c3c">long double</span> pour des nombres à virgule flottante précision étendue de <span style="color: #e74c3c">10o</span> compris entre <span style="color: #e74c3c">≈ 3.4 × 10⁻⁴⁹³² à 3</span>

pour indiquer le type de variable dans notre code nous allon devoir utiliser des "**%**", voici les "**%**" qui se refere a chaque variable : 

- %d : entier signé (type int)
- %i : entier signé (type int)
- %u : entier non signé (type unsigned int)
- %f : nombre à virgule flottante en simple précision (type float)
- %lf : nombre à virgule flottante en double précision (type double)
- %c : caractère unique (type char)
- %s : chaîne de caractères (tableau de char)
- %x : entier non signé en notation hexadécimale (type unsigned int)
- %p : pointeur (adresse mémoire)

### <span style="color: #3498db"> 2. les incrémentation 

ce que j'appelle les incrementation sont les élément qu'on va devoir appeller pour faire fonctionner notre code par exemple pour ecrire un "**hello world**"
nous devond ecrire :

#include <stdio.h>  //pour utiliser printf

int main()  //fonction main, execution première  
{   
    printf("hello world!\n");   //affiche le message    
    return 0;   //ici fait terminer le main     
}

ici nous appelons la bibliotheque stdio.h pour pouvoir utiliser le printf   
nous declarons aussi notre fonction principale,notre **main**, fonction principale de notre code     
dans le printf nous pouvons voir \n qui nous sert a sauter une ligne pour pouvoir lire clairement et ne pas avoir tous a la suite qui se colle en une seul ligne mais dans une forme de texte 
