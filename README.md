<div align="center">
  <img src="https://files.prismodev.fr/s/ppcSPGYkQPoF7WJ/download" alt="FCCKingdom Logo" width="160" />
  <h1>FCCKingdom Launcher</h1>
  <h3>Un launcher Minecraft multi-plateforme, natif et connecté • développé par <a href="https://files.prismodev.fr/s/qrPfeMBFz8KXJD8/download">PrismoDEV</a></h3>
</div>

---

<div align="center">

[![Made with Rust](https://img.shields.io/badge/Backend-Rust-orange?style=for-the-badge&logo=rust)](#)
[![Frontend React](https://img.shields.io/badge/Frontend-React-blue?style=for-the-badge&logo=react)](#)
[![TypeScript](https://img.shields.io/badge/Language-TypeScript-3178C6?style=for-the-badge&logo=typescript)](#)
[![Tauri](https://img.shields.io/badge/App-Tauri-FFC131?style=for-the-badge&logo=tauri)](#)
[![CI/CD](https://img.shields.io/badge/CI%2FCD-GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions)](#)
[![ASP.NET Core](https://img.shields.io/badge/API-ASP.NET%20Core-512BD4?style=for-the-badge&logo=dotnet)](#)

</div>

---

## ⚡ Résumé

**FCCKingdom Launcher** est un **launcher Minecraft professionnel et multi-plateforme** conçu pour offrir une expérience fluide et connectée à la communauté [FCCKingdom](https://fcckingdom.fr).  
Développé avec **Rust (Tauri)**, **React/TypeScript** et une **API .NET**, il allie performance native, automatisation et design moderne.

> 💻 Compatible **Windows, macOS (Intel & Apple Silicon)** et **Linux** — ce projet démontre une approche industrielle du développement multi-plateforme.

---

## 🧭 Sommaire
- [Contexte et Objectifs](#-contexte-et-objectifs)
- [Fonctionnalités Principales](#-fonctionnalités-principales)
- [Architecture et Automatisation](#-architecture-et-automatisation)
- [Système d’Intégrité des Fichiers](#-système-dintégrité-des-fichiers)
- [Défis Techniques et Innovations](#-défis-techniques-et-innovations)
- [Stack Technique](#-stack-technique)
- [Crédits](#-crédits)

---

## 🚀 Contexte et Objectifs

Le **FCCKingdom Launcher** a été créé pour **transformer l’accès au serveur Minecraft FCCKingdom** en une expérience fluide et centralisée.  
Son rôle dépasse le simple lancement du jeu : il gère **les mises à jour, les configurations, les skins**, et **l’authentification Microsoft**, tout en restant **léger et rapide** grâce à Rust.

🎯 Objectifs clés :
- Un **launcher natif et multiplateforme** sécurisé.
- Une **interface utilisateur moderne et animée**.
- Une **infrastructure CI/CD automatisée** pour un déploiement sans friction.
- Une **gestion intelligente des mods et fichiers clients**.

---

## 💡 Fonctionnalités Principales

### 🖥️ Interface Utilisateur Moderne
Conçue avec **React**, **TypeScript**, **Vite** et **TailwindCSS**, l’interface offre :
- Un design responsive et immersif.
- Des animations fluides (Framer Motion).
- Une structure front-end claire et maintenable.

| Menu Principal | Skins | Galerie |
| :---: | :---: | :---: |
| ![Menu Principal](https://files.prismodev.fr/s/JTLGXfPbAD8kxmE/download) | ![Gestionnaire de Skins](https://files.prismodev.fr/s/5gTrXJ3fr29aaKQ/download) | ![Galerie](https://files.prismodev.fr/s/AdBNZxFa9CmnT2A/download) |

| Paramètres | Addons |
| :---: | :---: |
| ![Paramètres](https://files.prismodev.fr/s/bwZJLogGt4g4Q9m/download) | ![Gestionnaire d'Addons](https://files.prismodev.fr/s/cmnqSWpCY6Ldt8M/download) |

---

## 🧩 Architecture et Automatisation

### ⚙️ CI/CD et Déploiement Continu
Pipeline entièrement automatisé avec **GitHub Actions** :
- 🔁 **Build simultané** pour Windows, macOS (Intel & ARM) et Linux.
- 🚀 **Déploiement via SFTP** vers le serveur de mise à jour.
- 🧾 **Génération dynamique** du manifeste `release.json` (signatures, hash, URLs).

![GitHub Workflow](https://files.prismodev.fr/s/TJtjjSZFC9rHRWX/download)

### 🔒 Backend & Communication
- **Rust/Tauri** : cœur applicatif, IPC et gestion du runtime.
- **ASP.NET Core** : API d’administration et gestion du manifeste.
- **Entity Framework + SQLite** : persistance légère et rapide.

---

## 🧱 Système d’Intégrité des Fichiers

Un système propriétaire de synchronisation contrôle la cohérence du contenu joueur/serveur.

| Type | Modes Disponibles |
| :-- | :-- |
| **Fichiers** | `Auto`, `Force`, `Ignore`, `Optional`, `Skip`, `Delete` |
| **Dossiers** | `Mirror`, `Additive`, `Inherit` |

- 🔍 **Synchronisation intelligente** des mods et assets.
- 🧰 **Interface web admin** pour piloter le manifeste en direct.

![File Integrity Manager](https://files.prismodev.fr/s/7BdJjnGGnaG9WBM/download)

---

## 🧠 Défis Techniques et Innovations

Créer un launcher **natif, multi-plateforme et automatisé** a impliqué plusieurs défis :

- 🦀 **Interopérabilité Rust ↔ React (IPC Tauri)** pour les échanges instantanés.
- 🪟 **Compatibilité triple OS** (Windows, macOS Intel & Apple Silicon, Linux).
- 🔐 **Intégration OAuth2 Microsoft** et gestion multi-comptes.
- 🔄 **Auto-update incrémental** via Rust + CI/CD GitHub Actions.
- 🎮 **Discord Rich Presence** et gestion des thèmes utilisateur.
- 🧱 **Architecture modulaire full-stack**, pensée pour évoluer en écosystème complet.

> Ce projet démontre la capacité à concevoir un produit robuste, multi-OS et intégrant un haut niveau de cohérence entre design, performance et déploiement.

---

## 🧰 Stack Technique

| Domaine | Technologies |
| :-- | :-- |
| **Frontend** | React, TypeScript, Vite, TailwindCSS, Framer Motion |
| **Backend & App** | Rust (Tauri Framework) |
| **API / Administration** | ASP.NET Core, C#, Entity Framework, SQLite |
| **CI/CD** | GitHub Actions |
| **Déploiement** | SSH / SFTP |
| **Systèmes supportés** | Windows, macOS (Intel & ARM), Linux |

---

## 👤 Crédits

**Développé par :** Sasha Da Silva [C4ptainF0xy] [PrismoDEV](https://files.prismodev.fr/s/qrPfeMBFz8KXJD8/download)  
**Rôle :** Conception, développement full-stack, CI/CD, architecture logicielle, UX/UI design  
**Projet :** Propriétaire – [FCCKingdom.fr](https://fcckingdom.fr)

---

<div align="center">
  <sub>🧠 Ce projet illustre une approche professionnelle du développement full-stack multiplateforme.<br>
  📬 Contact : <b>sashadasilva@prismodev.fr</b></sub>
</div>
