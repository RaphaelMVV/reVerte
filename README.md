# 🌿 ReVerte – Surveillance des îlots de chaleur urbains

> Projet de fin d'études Web3 – Bachelor Développeur Web

---

## 🎯 Objectif

**ReVerte** est un système de surveillance environnementale utilisant des capteurs **RuuviTag** pour détecter les **îlots de chaleur urbains**.  
Lorsqu'une zone dépasse un seuil critique de chaleur, le système déclenche une **alerte automatique** vers une **ONG partenaire**, afin d’intervenir auprès des populations vulnérables **sans surcharger les services d’urgence (comme les pompiers).**

---

## 🧩 Technologies utilisées

| Composant        | Technologie              |
|------------------|---------------------------|
| Capteurs         | RuuviTag + Raspberry Pi   |
| Collecte         | Python + MQTT             |
| Backend          | Node.js (Express)         |
| Base de données  | PostgreSQL                |
| Frontend         | React + Chakra UI         |
| Cartographie     | React-Leaflet             |
| Graphiques       | Recharts / Chart.js       |
| Alerte           | Telegram Bot (via API)    |

---

## 📁 Structure du projet

```
reverte/
├── backend/         # API Node.js (Express, MQTT, PostgreSQL)
├── frontend/        # Interface React (Dashboard, Carte, Alertes)
├── sensors/         # Scripts Python pour collecte des capteurs
├── docs/            # Spécifications, maquettes, PDF
├── README.md
└── .gitignore
```

---

## 🚀 Fonctionnalités principales

- 🔍 Lecture des capteurs RuuviTag (température, humidité)
- 🌡️ Détection des seuils critiques de chaleur
- 🧠 Traitement des données via API Node.js
- 🗺️ Visualisation temps réel sur une carte interactive
- ⚠️ Alerte automatisée à des ONG via Telegram
- 🕒 Historique des mesures et tableau de bord statistiques

---

## 🛠️ Installation rapide

### 📦 Prérequis

Assurez-vous d’avoir installé sur votre machine :

- [Node.js](https://nodejs.org) (v18 ou plus)
- [npm](https://www.npmjs.com/)
- [Python 3](https://www.python.org/)
- `pip3` (inclus avec Python)
- [MQTT Explorer](https://mqtt-explorer.com/) (pour visualiser les messages MQTT)
- [Git](https://git-scm.com/)

---

### 🧰 Étapes pour démarrer le projet ReVerte

#### 1. Cloner le projet
```bash
git clone https://github.com/<utilisateur>/reverte.git
cd reverte
```

#### 2. Lancer le backend (Node.js)
```bash
cd backend
npm install
npm start
```

> Le backend écoute sur http://localhost:3000

#### 3. Lancer le frontend (React)
```bash
cd ../frontend
npm install
npm start
```

> L’interface est accessible sur http://localhost:3000

#### 4. Lancer les capteurs (Python + MQTT)
```bash
cd ../sensors
pip3 install ruuvitag_sensor paho-mqtt
python3 ruuvi_mqtt_publisher.py
```

> Ce script lit les données des balises RuuviTag et les publie sur un broker MQTT.
> Utilisez MQTT Explorer pour voir les messages en temps réel.

---

### 🧪 Test de fonctionnement

1. Approchez une source de chaleur d’un capteur (lampe, main…)
2. Vérifiez les messages MQTT dans MQTT Explorer
3. Assurez-vous que :
   - Le backend reçoit les données
   - L’alerte est déclenchée si un seuil est dépassé
   - Le dashboard frontend affiche les mesures en direct

---

### ℹ️ Remarque

> La base de données PostgreSQL n’est pas encore utilisée. Aucune configuration n’est requise à ce stade.

## 👥 Équipe projet

- 👤 Nelson ALMEIDA
- 👤 Nour FELLAG
- 👤 Rafik ZEFFANE
- 👤 Raphael PAES RODRIGUES DA SILVA

## 👥 Taches projet

- Backend/API
- Capteurs et MQTT
- Frontend React
- Base de données & intégration

---

## 📄 Licence

Ce projet est sous licence **MIT** – utilisation libre à but éducatif ou communautaire.

---
