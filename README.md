# 🏦 Application Console – Système Bancaire en Kotlin



## 🎯 Description du projet

Cette application console simule un système bancaire simple développé en Kotlin.  
Elle permet à l’utilisateur de :

- Créer un type de compte (Débit, Crédit ou Checking)
- Consulter le solde
- Retirer de l’argent
- Déposer de l’argent
- Fermer l’application

Les entrées utilisateur sont simulées à l’aide de valeurs aléatoires.

---

## 🧠 Objectifs pédagogiques

À la fin de ce projet, il est possible de :

- Modéliser différents types de comptes bancaires
- Utiliser les structures de contrôle (`if`, `when`, `while`)
- Implémenter des fonctions avec paramètres et valeurs de retour
- Appliquer des règles métier différentes selon le type de compte
- Organiser le code en sections claires et structurées
- Tester le comportement du programme avec différents scénarios

---

## 🛠 Technologies utilisées

- Kotlin
- Kotlin Playground ou IntelliJ IDEA

---

## 🏗 Structure du projet

Le projet est divisé en trois parties principales :

### 1️⃣ Partie 1 — Création du compte

- Affichage d’un message d’accueil
- Choix du type de compte
- Validation de la sélection
- Confirmation du compte créé

  <img width="865" height="224" alt="image" src="https://github.com/user-attachments/assets/885e69e4-26a5-4d70-a10d-7451c41723f0" />


### 2️⃣ Partie 2 — Opérations bancaires

Fonctions implémentées :

- `withdraw(amount: Int)` → Retrait standard
- `debitWithdraw(amount: Int)` → Retrait sécurisé pour compte débit
- `deposit(amount: Int)` → Dépôt standard
- `creditDeposit(amount: Int)` → Gestion spécifique du compte crédit

Règles importantes :

- Compte Débit : impossible de retirer plus que le solde
- Compte Crédit : le solde représente une dette (valeur négative)
- Compte Checking : fonctionnement standard

  <img width="1396" height="121" alt="image" src="https://github.com/user-attachments/assets/214e6c82-5cb7-4f12-ae57-c90e8ce9168f" />


### 3️⃣ Partie 3 — Menu principal

- Affichage d’un menu interactif
- Exécution des opérations selon le choix
- Utilisation d’une boucle `while`
- Fermeture de l’application avec l’option 4
- Centralisation des opérations via la fonction `transfer(mode)`

<img width="842" height="224" alt="image" src="https://github.com/user-attachments/assets/04a2d26f-e9f6-4f3a-83a1-bddcc0434294" />

---

## 🔄 Fonctionnement général

1. L’utilisateur crée un compte.
2. Un solde initial est généré aléatoirement.
3. Le menu principal s’affiche en boucle.
4. Les opérations modifient le solde selon les règles définies.
5. L’application se ferme lorsque l’utilisateur choisit l’option correspondante.

---

## ⚠ Problèmes fréquents

**Erreur : Unresolved reference: accountBalance**  
Cause : fonctions déclarées en dehors de `main()` alors que la variable est locale.  
Solution : déclarer les fonctions à l’intérieur de `main()`.

**Instruction `when` non exhaustive**  
Solution : ajouter un `else`.

**Logique du compte crédit incorrecte**  
Solution : s’assurer que le solde initial du compte crédit est négatif.

---
<img width="912" height="373" alt="image" src="https://github.com/user-attachments/assets/d740d668-6d22-4dcf-858e-d00822530074" />

<img width="1336" height="316" alt="image" src="https://github.com/user-attachments/assets/a3463e32-e5ae-4136-b871-7f0f01e45b75" />

<img width="1457" height="320" alt="image" src="https://github.com/user-attachments/assets/5f7b2a50-7f00-4d2c-aaf7-75634c2bba21" />

<img width="993" height="381" alt="image" src="https://github.com/user-attachments/assets/ad8037a2-618e-4582-9480-f54edfa8aacc" />

---

## 👩‍💻 Auteur

Salma Lakhal  
CLE Info – S5 
Fondamentaux de la programmation en Kotlin
Année universitaire 2025–2026
