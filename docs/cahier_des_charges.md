# 🧾 Cahier des Charges — Projet **ExamAccess**

## 1. Présentation du projet
**Nom :** ExamAccess  
**Objectif :** Permettre aux étudiants de la Faculté des Sciences ( pour un debut ) de l’Université de Yaoundé I d’accéder, télécharger et partager d’anciennes épreuves (TD, TP, CC, examens).  
**Public cible :** Étudiants de L1 à M2.  

---

## 2. Fonctionnalités principales
| ID | Fonctionnalité          | Description                                        |
|----|-------------------------|----------------------------------------------------|
| F1 | Authentification        | Inscription, connexion, déconnexion                |
| F2 | Consultation d’épreuves | Recherche par matière, semestre, niveau            |
| F3 | Téléchargement          | Sauvegarde d’épreuves sur le compte personnel      |
| F4 | Mode hors ligne         | Consultation d’épreuves téléchargées sans Internet |
| F5 | Ajout d’épreuve         | Upload de fichiers (PDF, DOCX, images)             |
| F6 | Administration          | Gestion des utilisateurs et épreuves               |
-------------------------------------------------------------------------------------
---

## 3. Architecture technique
- **Frontend :** HTML, CSS, JavaScript (puis React)
- **Backend :** Python (Flask)
- **Base de données :** PostgreSQL
- **Stockage fichiers :** Local (tests) puis Cloud (Supabase)
- **Hébergement :** GitHub + Render/Railway (plus tard)

---

## 4. Contraintes
- Interface responsive (mobile et PC)
- Sécurité minimale (hachage mots de passe)
- Téléchargement asynchrone et gestion de cache hors ligne
- Interface simple et intuitive

---

## 5. Planning
| Étape       | Durée      | Description                       |
|-------------|------------|-----------------------------------|
| Conception  | RAS        | Cahier des charges + dictionnaire |
| Backend     | RAS        | API Flask, base de données        |
| Frontend    | RAS        | Interface utilisateur             |
| Tests       | RAS        | Validation et corrections         |
| Déploiement | RAS        | Mise en ligne du projet           |
