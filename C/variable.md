# <span style="color: #3498db">aprentissage du C</span>

### <span style="color: #3498db">instalation des prerequis</span>

* VS Code comme IDE : [https://code.visualstudio.com/Download](https://code.visualstudio.com/Download)



**Windows :**
Télécharger l’exécutable, puis l’installer comme n’importe quelle application.

Ensuite, ouvrir votre IDE et lancer un terminal (en haut de l’interface).

---
**Linux :**
Installer le paquet **.deb**, puis extraire avec :

```bash
dpkg-deb -x nom_du_paquet.deb repertoire_destination
```

Installer le compilateur C :

```bash
sudo apt install gcc
```

Vérifier l’installation :

```bash
gcc --version
```

---

### <span style="color: #3498db">1. les variables</span>

Les variables sont des **conteneurs** qui permettent de stocker des données en mémoire pour les utiliser dans le programme.

Chaque variable possède :

* un **type** (nature de la donnée)
* un **nom**
* une **valeur**

---

**Types principaux :**

* <span style="color: #e74c3c">char</span> → caractère (1 octet)
  de <span style="color: #e74c3c">-128 à 127</span>

* <span style="color: #e74c3c">unsigned char</span> → caractère positif
  de <span style="color: #e74c3c">0 à 255</span>

* <span style="color: #e74c3c">short int</span> → entier court (2 octets)
  de <span style="color: #e74c3c">-32 768 à 32 767</span>

* <span style="color: #e74c3c">unsigned short int</span> → entier court positif
  de <span style="color: #e74c3c">0 à 65 535</span>

* <span style="color: #e74c3c">int</span> → entier (souvent 4 octets)
  de <span style="color: #e74c3c">-2 147 483 648 à 2 147 483 647</span>

* <span style="color: #e74c3c">unsigned int</span> → entier positif
  de <span style="color: #e74c3c">0 à 4 294 967 295</span>

* <span style="color: #e74c3c">long int</span> → entier long
  (souvent 4 ou 8 octets selon le système)

* <span style="color: #e74c3c">unsigned long int</span> → entier long positif

* <span style="color: #e74c3c">float</span> → nombre à virgule (précision simple, 4 octets)
  ≈ <span style="color: #e74c3c">3.4 × 10⁻³⁸ à 3.4 × 10³⁸</span>

* <span style="color: #e74c3c">double</span> → nombre à virgule (précision double, 8 octets)
  ≈ <span style="color: #e74c3c">1.7 × 10⁻³⁰⁸ à 1.7 × 10³⁰⁸</span>

* <span style="color: #e74c3c">long double</span> → précision étendue

---

**Déclaration d’une variable :**

```c
int age = 20;
float taille = 1.75;
char lettre = 'A';
```

---

### <span style="color: #3498db">formats d'affichage (printf)</span>

Pour afficher une variable avec `printf`, on utilise des **spécificateurs de format** (`%`).

* `%d` → entier signé (`int`)
* `%i` → entier signé (`int`)
* `%u` → entier non signé (`unsigned int`)
* `%f` → float
* `%lf` → double
* `%c` → caractère
* `%s` → chaîne de caractères
* `%x` → hexadécimal
* `%p` → adresse mémoire (pointeur)

---

**Exemple :**

```c
#include <stdio.h>

int main()
{
    int age = 20;
    float taille = 1.75;

    printf("Age : %d\n", age);
    printf("Taille : %f\n", taille);

    return 0;
}
```

---

**À retenir :**

* Une variable = une zone mémoire
* Le type détermine ce qu’on peut stocker
* Les `%` servent à afficher correctement les valeurs
* Le choix du type impacte la précision et la mémoire utilisée

---
