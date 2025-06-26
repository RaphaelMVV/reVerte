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

### Backend (Node.js)
```bash
cd backend
npm install
npm start
```

### Frontend (React)
```bash
cd frontend
npm install
npm run dev
```

### Capteurs (Raspberry Pi + MQTT)
```bash
cd sensors
python3 ruuvi_mqtt_publisher.py
```

---

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
