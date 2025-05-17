# 🐝 Projet Ruche Connectée

Prototype d'une ruche connectée pour la surveillance à distance dans le cadre de l’apiculture urbaine.

## 🎯 Objectif

Fournir aux apiculteurs un système numérique pour :
- Suivre à distance l’état de leurs ruches
- Être alerté en cas de conditions anormales
- Visualiser les données depuis une **application mobile Flutter** ou un **site Web Spring Boot**

---

## ⚙️ Technologies utilisées

| Composant       | Stack                                                                 |
|-----------------|-----------------------------------------------------------------------|
| Mobile          | Dart + Flutter                                                        |
| Backend         | Java Spring Boot                                                      |
| Base de données | Firebase (Auth, Firestore, Realtime DB si besoin)                    |
| IoT             | ESP32 + capteur DHT11 (température + humidité) + interrupteur        |
| Communication   | Wifi (les ruches sont connectées à un point d’accès)                 |
| Alertes         | Envoi d’e-mails en cas d'ouverture suspecte de ruche                 |

---

## 📱 Fonctionnalités attendues

- Authentification des apiculteurs
- Gestion des ruchers (ajout, modification, suppression)
- Gestion des ruches dans chaque rucher
- Visualisation :
  - Température
  - Humidité
  - État du couvercle (ouvert / fermé)
  - Historique des données (courbe sur 7 jours)
- Réception de mail si le couvercle est ouvert (sauf si désactivé manuellement)
- Version Web avec les mêmes fonctionnalités
