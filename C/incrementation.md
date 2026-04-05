<span style="color: #3498db">2. directives du préprocesseur</span>

Les directives du préprocesseur sont exécutées avant la compilation. Elles permettent de préparer le code avant qu’il soit réellement compilé.

Principales directives :

* `#include` → inclure une bibliothèque

```c
#include <stdio.h>
```

* `#define` → définir une constante

```c
#define PI 3.14
```

* `#ifdef`, `#ifndef` → conditions de compilation

```c
#ifndef TEST
#define TEST
#endif
```

Ces directives sont essentielles car elles permettent d’ajouter des fonctionnalités externes ou de contrôler la compilation du programme.

---

<span style="color: #3498db">2. bibliothèques</span>

Les bibliothèques contiennent des fonctions déjà écrites que l’on peut réutiliser pour éviter de tout coder soi-même.

Exemples :

* `stdio.h` → entrée / sortie (`printf`, `scanf`)
* `stdlib.h` → gestion mémoire, conversions
* `math.h` → fonctions mathématiques

---

<span style="color: #3498db">3. incrémentation (utilisation des éléments du code)</span>

Ce que l’on appelle ici "incrémentation" correspond aux éléments nécessaires pour faire fonctionner un programme.

Exemple avec un "Hello World" :

```c
#include <stdio.h> // permet d'utiliser printf

int main() // fonction principale, point d'entrée du programme
{
    printf("hello world!\n"); // affiche le message
    return 0; // termine le programme
}
```

Explications :

* `#include <stdio.h>` → on inclut la bibliothèque pour pouvoir utiliser `printf`
* `int main()` → c’est la fonction principale, le programme commence ici
* `printf("hello world!\n");` → affiche du texte dans la console, il est important de mettre \n pour ne couper le texte et sauter la ligne
* `\n` → permet de faire un retour à la ligne pour une meilleure lisibilité
* `return 0;` → indique que le programme s’est terminé correctement