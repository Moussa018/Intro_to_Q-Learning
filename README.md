#  Q-Learning Algorithm

## Description
Ce projet implémente l’algorithme **Q-Learning**, une technique d’apprentissage par renforcement .  
L’objectif est de permettre à un agent d’apprendre une stratégie optimale en interagissant avec un environnement.

---

##  Principe
Le Q-Learning est un algorithme **model-free**, ce qui signifie qu’il ne nécessite pas de modèle de l’environnement.

Il repose sur une fonction appelée **Q-table** :
## Q(s, a)
- **s** : état (state)  
- **a** : action (action)  
- **Q(s,a)** : valeur estimée de l’action dans cet état  

###  Mise à jour

==> Q(s,a) = Q(s,a) + α [ r + γ max Q(s',a') - Q(s,a) ]

- **α (alpha)** : taux d’apprentissage  
- **γ (gamma)** : facteur de réduction  
- **r** : récompense  
- **s'** : nouvel état  

---

##  Fonctionnement
1. Initialiser la Q-table  
2. Observer l’état courant  
3. Choisir une action (exploration vs exploitation)  
4. Recevoir une récompense  
5. Mettre à jour la Q-table  
6. Répéter jusqu’à convergence  

---

##  Exécution
```bash
jupyter notebook Qlearning.ipynb



