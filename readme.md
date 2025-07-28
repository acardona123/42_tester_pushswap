# Pushswap Tester

## 📌 Description
Outils d'aide à la correction du projet Pushswap de 42:
 1. `moyenne.sh` pour calculer le nombre de coups moyen d'un Pushswap lors du tri d'un nombre donné d'entiers (bornés)
 2. `randomizer.sh` pour obtenir une liste d'entiers bornés mélangée de manière aléatoire.


## ⚙️ Installation et Utilisation
Les deux scripts peuvent être utilisés indépendamment.

### Génération de liste
`randomizer.sh` peut être exécuté n'importe où avec le format suivant:
```bash
	bash randomizer.sh <born_min> <born_max>
 ```

> **Example:**
> `bash randomizer.sh 1 10`
> -> sortie possible: `1 5 10 4 2 6 7 8 3 9` 

### Tester le coût moyen de l'algorithme
```bash
	git clone https://github.com/acardona123/42_tester_pushswap
	cd 42_tester_pushswap/
	cp <directory_contenant_push_swap>/push_swap .
	bash ./moyenne.sh <min_value> <max_value> <nombre_max_d_iteration>
```
**Arguments:**
- `min_value`: la borne inférieure des valeurs à trier
- `max_value`: la borne supérieure des valeurs à trier
- `nombre_max_d_iteration`: le nombre max d'opérations issues du push_swap pour `max_value - min_value + 1` par le sujet.
> Example:  
> `bash moyenne.sh 1 100 700`

> **Rappel:**  
> Selon le sujet, le nombre d'itérations maximum pour obtenir 100% sont:
> - 100 valeurs: 700
> - 500 valeurs: 5500