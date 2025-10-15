# ExamAccess
Application web permettant aux étudiants de la Faculté des Sciences ( pour un debut ) de l’Université de Yaoundé I d’accéder et partager d’anciennes épreuves.

# 🎓 ExamAccess — Faculté des Sciences, Université de Yaoundé I

## 🧭 Description du projet
**ExamAccess** est une application web conçue pour les étudiants de la **Faculté des Sciences de l’Université de Yaoundé I**.  
Elle permet d’**accéder, partager et télécharger les anciens sujets d’examens, de TD, TP et contrôles continus** pour les deux semestres.  

L’application vise à **faciliter la révision et la préparation des examens** en centralisant les ressources académiques.  
Les utilisateurs peuvent **ajouter de nouvelles épreuves**, **les consulter en ligne** ou **les sauvegarder hors connexion**, à la manière de YouTube Offline.

---

## 🚀 Fonctionnalités principales

| Fonctionnalité      | Description                                                               |
|---------------------|---------------------------------------------------------------------------|
| 🔐 Authentification | Inscription, connexion, et gestion de profil étudiant                     |
| 📚 Consultation     | Recherche et filtrage des épreuves par matière, niveau, type et semestre  |
| 📤 Ajout d’épreuve  | Téléversement de fichiers (PDF, DOCX, images) avec informations associées |
| 📥 Téléchargement   | Sauvegarde locale sur le compte étudiant                                  |
| 📴 Mode hors ligne  | Accès aux épreuves téléchargées sans connexion Internet                   |
| ⚙️ Administration   | Gestion des utilisateurs et modération du contenu                         |

---

## 🧩 Architecture technique

### 🔹 Frontend
- HTML, CSS, JavaScript (puis évolution vers **React.js**)
- Interface responsive (mobile & desktop)
- Support du **mode hors ligne (PWA)**

### 🔹 Backend
- **Python (Flask)** — pour la gestion des routes, des fichiers et des utilisateurs
- Architecture en couches : `models`, `dao`, `services`, `routes`
- API REST pour communication avec le frontend

### 🔹 Base de données
- **PostgreSQL** (ou SQLite pour le développement local)
- Tables principales : `Utilisateur`, `Epreuve`, `Téléchargement`

### 🔹 Hébergement et outils
- **GitHub** pour le suivi du code source
- **Render / Railway** pour le déploiement du backend
- **Supabase / AWS S3** pour le stockage des fichiers

---

## 🗂️ Structure du projet

ExamAccess/
├── docs/ # Documentation du projet
│ ├── cahier_des_charges.md
│ └── dictionnaire_de_donnees.md
├── backend/ # Code Flask (API, modèles, DAO, routes)
├── frontend/ # Interface web (HTML, CSS, JS)
├── .gitignore
├── README.md
└── requirements.txt # Dépendances Python


---

## ⚙️ Installation du projet (développement local)

### 1️⃣ Cloner le dépôt
```bash
git clone https://github.com/nzeukouecamel-glitch/ExamAccess.git
cd ExamAccess
```

### 2️⃣ Créer un environnement virtuel
```bash
python3 -m venv venv
source venv/bin/activate  # Sur macOS / Linux
venv\Scripts\activate     # Sur Windows
```

### 3️⃣ Installer les dépendances
```bash
pip install -r requirements.txt
```

### 4️⃣ Lancer le serveur Flask
```bash
cd backend
python app.py
```
L’application sera accessible sur http://localhost:5000/

