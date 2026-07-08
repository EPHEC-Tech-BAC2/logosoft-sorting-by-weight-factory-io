# Architecture de modules logiques — LogoSoft

Projet réalisé à l'EPHEC (Classe 2AU, 2025-2026), en binôme avec **TABICH Mohamed**.

## Le cours

Ce dépôt regroupe les travaux pratiques et le projet final réalisés dans le cadre du cours "Architecture et modules logiques". L'objectif : apprendre à programmer des automates avec **LogoSoft**, à travers des cas concrets (LED, aération, chauffage, tri), jusqu'à un projet final complet sur **Factory I/O**.

## Les travaux pratiques

- **TP1 — Bascule RS, un seul bouton** : pilotage d'une LED (Q1) via un bouton poussoir (I1), bascule RS + front montant pour alterner allumage/extinction à chaque pression.
- **TP2 — Installation d'aération** : gestion de deux ventilateurs (extraction / air frais) selon capteurs de débit et temporisateurs, avec arrêt d'urgence prioritaire.
- **TP3 — Commande de chauffage** : régulation par comparateur analogique entre température extérieure et consigne, avec seuils on/off.
- **TP4 — Tri par hauteur** : tri automatisé sur convoyeur selon la hauteur des pièces (capteurs haut/bas), aiguillage gauche/droite, avec sécurité Stop + arrêt d'urgence.

## Le projet final : Sorting by Weight (Factory I/O)

Automatisation complète de la scène "Sorting by Weight" pilotée depuis LogoSoft :
- Pesée des colis sur balance, avec temporisation pour stabiliser la mesure
- Tri en 3 catégories (léger / moyen / lourd) selon le signal analogique de poids
- Aiguillage automatique vers 3 sorties (gauche, face, droite)
- Comptage par direction, affichage temps réel sur l'IHM (poids + compteurs)
- Sécurité : arrêt d'urgence prioritaire, alerte visuelle (rétroéclairage rouge) et verrouillage des actionneurs

## Logiciel

- LogoSoft (LOGO! Soft Comfort)
- Simulation Factory I/O (scène "Sorting by Weight")

## Contenu du dépôt

- `tp1-bascule-rs/` à `tp4-tri-par-hauteur/` : programmes LogoSoft de chaque TP
- `projet-final-sorting-by-weight/` : programme LogoSoft, GRAFCET niveau 1
- `rapport/` : rapport complet présentant l'ensemble du travail