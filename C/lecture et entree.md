<span style="color: #3498db">3. affichage et entrée</span>

En C, on utilise principalement deux fonctions pour interagir avec l’utilisateur : `printf` pour afficher et `scanf` pour lire une valeur.

---

**Afficher du texte ou des valeurs :**

```c
printf("Nombre : %d\n", a);
```

Explications :

* `printf` → fonction qui permet d’afficher du texte dans la console
* `"Nombre : %d\n"` → chaîne de caractères affichée
* `%d` → spécificateur de format, il indique que l’on va afficher un entier (`int`)
* `a` → variable dont la valeur sera affichée à la place de `%d`
* `\n` → retour à la ligne pour éviter que tout s’affiche sur une seule ligne

Exemple concret :
Si `a = 5`, alors le programme affichera :

```
Nombre : 5
```

On peut utiliser d’autres formats :

* `%f` → float (nombre à virgule)
* `%c` → caractère
* `%s` → chaîne de caractères

---

**Lire une valeur entrée par l’utilisateur :**

```c
scanf("%d", &a);
```

Explications :

* `scanf` → fonction qui permet de lire une valeur entrée au clavier
* `"%d"` → indique que l’on attend un entier (`int`)
* `&a` → adresse mémoire de la variable `a`

⚠️ **Le `&` est obligatoire** ici :
Il permet à `scanf` de savoir **où stocker la valeur en mémoire**.

Sans le `&`, le programme ne fonctionnera pas correctement (erreur ou comportement imprévisible).

---

**Exemple complet :**

```c
#include <stdio.h>

int main()
{
    int a;

    printf("Entrez un nombre : ");
    scanf("%d", &a);

    printf("Vous avez entré : %d\n", a);

    return 0;
}
```

Fonctionnement :

1. Le programme demande un nombre
2. L’utilisateur entre une valeur
3. Cette valeur est stockée dans `a`
4. Le programme affiche la valeur entrée

---

**À retenir :**

* `printf` → afficher
* `scanf` → lire
* `%d`, `%f`, `%c`, `%s` → types de données
* `&variable` → indispensable pour stocker une entrée utilisateur
