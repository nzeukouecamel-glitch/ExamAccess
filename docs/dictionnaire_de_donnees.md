# 🗃️ Dictionnaire de Données — **ExamAccess**

## Table : Utilisateur
| Champ         | Type         | Description                 |
|---------------|--------------|-----------------------------|
| id_user       | INT          | Identifiant unique          |
| nom           | VARCHAR(50)  | Nom complet                 |
| filiere       | VARCHAR(100) | spécialité de l'utilisateur |
| email         | VARCHAR(100) | Adresse email unique        |
| mot_de_passe  | VARCHAR(255) | Mot de passe chiffré        |
| date_creation | DATE         | Date d’inscription          |
--------------------------------------------------------------
---

## Table : Epreuve
| Champ      | Type         | Description                                       |
|------------|--------------|---------------------------------------------------|
| id_epreuve | INT          | Identifiant unique                                |
| titre      | VARCHAR(100) | Nom de l’épreuve                                  |
| type       | VARCHAR(20)  | TD, TP, CC, Examen                                |
| semestre   | VARCHAR(10)  | S1 ou S2                                          |
| matiere    | VARCHAR(100) | Nom de la matière                                 |
| niveau     | VARCHAR(20)  | L1, L2, L3, M1, M2                                |
| filiere    | VARCHAR(100) | Filière concernée par l'épreuve                   |
| fichier    | VARCHAR(255) | Lien du fichier sur le serveur                    |
| id_user    | INT          | Référence de l’utilisateur ayant ajouté l’épreuve |
| date_ajout | DATE         | Date d’ajout de l’épreuve                         |
---------------------------------------------------------------------------------
---

## Table : Téléchargement
| Champ               | Type | Description                  |
|---------------------|------|------------------------------|
| id_telechargement   | INT  | Identifiant unique           |
| id_user             | INT  | Identifiant de l’utilisateur |
| id_epreuve          | INT  | Identifiant de l’épreuve     |
| date_telechargement | DATE | Date du téléchargement       |
-------------------------------------------------------------
---

## Relations entre les tables
- **Utilisateur (1,n)** → **Epreuve**  
  Un utilisateur peut ajouter plusieurs épreuves.  
- **Utilisateur (1,n)** → **Téléchargement**  
  Un utilisateur peut télécharger plusieurs épreuves.  
- **Epreuve (1,n)** → **Téléchargement**  
  Une épreuve peut être téléchargée plusieurs fois.
