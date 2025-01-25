Étude de cas : Définir les étapes principales d’un projet informatique visant à installer une salle serveur pour une PME.
Le projet inclut le câblage et la mise en service complète des infrastructures. Voici les spécifications :
1.	Serveurs physiques et clustering :
o	La PME dispose de 5 serveurs physiques, dont 3 doivent être configurés en cluster avec redondance.
o	Les 2 serveurs restants serviront de redondants physiques, et une redondance supplémentaire sera configurée sur le cloud.
2.	Équipements des employés :
o	Chaque employé (50 au total) dispose d’un PC fixe.
o	Les 15 cadres supérieurs disposent également d’un ordinateur portable en plus de leur PC fixe.
3.	Réseau et connectivité :
o	Le bâtiment comprend 3 niveaux, et un accès Wi-Fi par hotspot doit être disponible sur chaque étage.
o	Le câblage réseau devra être réalisé pour prendre en charge les postes et les hotspots.
4.	Stockage et sauvegarde :
o	La PME dispose d’un serveur NAS pour le stockage des données.
o	Une licence Veeam est disponible pour assurer la réplication et la sauvegarde des données critiques.
5.	Activité principale :
o	La PME propose des solutions logicielles en mode SaaS et accorde une importance capitale à la satisfaction client, ce qui implique une haute disponibilité et des performances optimales des infrastructures IT.


# Projet d'Installation Salle Serveur PME
## Documentation Technique et Plan de Déploiement

### 1. PHASE PRÉLIMINAIRE (2 semaines)

#### 1.1 Audit et Analyse
- Évaluation de l'espace disponible pour la salle serveur
- Audit des besoins électriques et de climatisation
- Analyse des flux de données et besoins en bande passante
- Évaluation des contraintes réglementaires (RGPD, normes sectorielles)

#### 1.2 Conception Architecture
- Architecture réseau détaillée
- Plan d'adressage IP
- Schéma de câblage
- Architecture de clustering
- Plan de redondance (on-premise + cloud)

#### 1.3 Documentation Initiale
- Cahier des charges technique
- Plans d'implantation
- Liste des équipements nécessaires
- Budget détaillé

### 2. INFRASTRUCTURE DE BASE (3 semaines)

#### 2.1 Préparation Salle Serveur
- Installation système de climatisation redondant
- Mise en place alimentation électrique sécurisée
- Installation onduleurs (UPS)
- Pose chemins de câbles
- Installation système contrôle d'accès
- Mise en place système détection incendie

#### 2.2 Câblage Structuré
- Déploiement câblage vertical entre étages
- Installation câblage horizontal par étage
- Mise en place prises réseau
- Tests de certification câblage
- Étiquetage et documentation

### 3. INFRASTRUCTURE RÉSEAU (3 semaines)

#### 3.1 Équipements Réseau Core
- Installation switches core redondants
- Configuration VLANs
- Mise en place routeurs
- Installation et configuration pare-feu
- Mise en place supervision réseau

#### 3.2 Couverture WiFi
- Installation points d'accès WiFi par étage
- Configuration contrôleur WiFi
- Paramétrage sécurité et authentification
- Tests de couverture
- Optimisation placement et puissance

### 4. INFRASTRUCTURE SERVEURS (4 semaines)

#### 4.1 Mise en Place Cluster
- Installation hyperviseur sur serveurs
- Configuration cluster 3 nœuds
- Mise en place haute disponibilité
- Configuration load balancing
- Tests de basculement

#### 4.2 Serveurs de Backup
- Configuration 2 serveurs backup physiques
- Setup environnement cloud backup
- Installation et configuration Veeam
- Tests de réplication
- Validation des sauvegardes

#### 4.3 Stockage
- Configuration serveur NAS
- Mise en place politique de stockage
- Configuration quotas
- Setup réplication NAS
- Tests performance stockage

### 5. DÉPLOIEMENT POSTES UTILISATEURS (2 semaines)

#### 5.1 Configuration Standard
- Création image master PC fixes
- Création image master laptops
- Déploiement configurations
- Installation logiciels métiers
- Tests utilisateurs

#### 5.2 Spécificités Cadres
- Configuration accès VPN
- Setup synchronisation données
- Configuration double authentification
- Tests mobilité

### 6. TESTS ET VALIDATION (3 semaines)

#### 6.1 Tests Infrastructure
- Tests charge serveurs
- Validation haute disponibilité
- Tests failover cluster
- Vérification performances réseau
- Validation backup/restore

#### 6.2 Tests Utilisateurs
- Validation accès applications
- Tests performances SaaS
- Validation connexions WiFi
- Tests mobilité cadres
- Validation sécurité

### 7. MISE EN PRODUCTION (2 semaines)

#### 7.1 Migration
- Plan de migration détaillé
- Bascule progressive services
- Migration données
- Tests post-migration
- Validation production

#### 7.2 Documentation et Formation
- Documentation technique complète
- Procédures exploitation
- Formation équipe IT
- Formation utilisateurs
- Support post-déploiement

### INDICATEURS DE PERFORMANCE (KPIs)

1. **Disponibilité Infrastructure**
   - Objectif 99.99% disponibilité services SaaS
   - Temps bascule cluster < 5 minutes
   - RPO < 15 minutes, RTO < 1 heure

2. **Performance Réseau**
   - Latence interne < 5ms
   - Couverture WiFi > -65dBm partout
   - Bande passante garantie > 100Mbps/utilisateur

3. **Sécurité**
   - Temps détection incidents < 5 minutes
   - Temps réponse incidents < 30 minutes
   - 100% données critiques chiffrées

### LIVRABLES

1. **Documentation Technique**
   - Architecture détaillée
   - Schémas réseau
   - Procédures exploitation
   - Plan de reprise d'activité

2. **Rapports**
   - Tests de charge
   - Certification câblage
   - Tests sécurité
   - Validation performances

3. **Formation**
   - Supports formation IT
   - Guides utilisateurs
   - Procédures urgence
   - Documentation maintenance
