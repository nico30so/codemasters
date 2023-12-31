# Fil de L'eau

# Table des Matières

- [Lecture du document](#lecture-du-document)
- [Lecture du texte généré et ajout d'améliorations/modifications](#lecture-du-texte-généré-et-ajout-daméliorationsmodifications)
- [Phrase résumant le projet en 1 ligne](#phrase-résumant-le-projet-en-1-ligne)
- [Glossaire](#glossaire)
- [Mots compliqués](#mots-compliqués)
- [Réduction de la phrase pour le readme](#réduction-de-la-phrase-pour-le-readme)
- [Suivi du cours sur les scénarios](#suivi-du-cours-sur-les-scénarios)
- [Création des scénarios](#création-des-scénarios)
- [Scénarios non détaillés](#scénarios-non-détaillés)
- [Version détaillée](#version-détaillée)
- [Modification des scénarios et implémentation de ceux-ci, correction, et suppression des doublons.](#modification-des-scénarios-et-implémentation-de-ceux-ci-correction-et-suppression-des-doublons)
- [Ajout des scénarios développés en externe au fichier de base et création des dossiers.](#ajout-des-scénarios-développés-en-externe-au-fichier-de-base-et-création-des-dossiers)
- [Après la mise en place des scénarios et la publication de ceux-ci sur GitHub, nous commençons le développement des différents diagrammes scénario par scénario et les publions directement dans les dossiers correspondants.](#après-la-mise-en-place-des-scénarios-et-la-publication-de-ceux-ci-sur-github-nous-commençons-le-développement-des-différents-diagrammes-scénario-par-scénario-et-les-publions-directement-dans-les-dossiers-correspondants)
- [Répartition des tâches pour la création des diagrammes (Séquence / Classe) (Répartition en part égale des diagrammes) :](#répartition-des-tâches-pour-la-création-des-diagrammes-séquence--classe-répartition-en-part-égale-des-diagrammes-)
- [Importation des fichiers dans les dossiers sur le GitHub](#importation-des-fichiers-dans-les-dossiers-sur-le-github)
- [Préparation de l'oral et choix du scénario à présenter](#préparation-de-loral-et-choix-du-scénario-à-présenter)


## Lecture du document
- L'application CultureDiffusion a pour projet de créer une bibliothèque numérique décentralisée. Les membres peuvent numériser des œuvres et les emprunter selon deux modalités : gratuit pour les œuvres du domaine public et location pour les œuvres sous droits. Les membres peuvent également proposer des œuvres. Chaque œuvre est composée de fichiers d'œuvre et de métadonnées. L'application gère quatre répertoires, dont un pour les œuvres libres de droits et un pour les œuvres sous droits en attente de modération.
- L'application est organisée en quatre répertoires :
  1. "fond_commun" : contient des œuvres libres de droits de l'application.
  2. "emprunts" : stocke les œuvres sous droits empruntées par les membres, chiffrées avec leur clé personnelle.
  3. "séquestre" : gère une partie des œuvres sous droits de l'application, avec tous les fichiers chiffrés, et l'index n'est pas accessible directement.
  4. "à modérer" : contient les œuvres proposées par les membres en attente de modération.

## Lecture du texte généré et ajout d'améliorations/modifications
- Conception de ce résumé via différents outils : ChatGPT

## Phrase résumant le projet en 1 ligne
CultureDiffusion développe une bibliothèque numérique décentralisée permettant aux membres de numériser, emprunter et proposer des œuvres, avec une modération assurée par les bibliothécaires.

## Glossaire
**Bibliothèque numérique** : Une collection d'œuvres sous forme numérique, généralement accessibles via un ordinateur ou un appareil électronique.
**Gestion décentralisée** : La répartition des responsabilités et des opérations sur plusieurs emplacements ou entités au lieu d'un seul centre de contrôle.
**Œuvres** : Contenu créatif tel que des livres, de la musique, des vidéos, etc.
**Domaine public** : Œuvres dont les droits d'auteur ont expiré ou ont été volontairement partagées sans restriction.
**Emprunt** : L'action de prendre temporairement une œuvre en vue de sa lecture ou de son utilisation.
**Membre** : Une personne ou une entité qui fait partie d'une organisation ou d'un groupe.
**Fichier** : Un ensemble de données numériques stockées sous un nom spécifique.
**Format JSON** : Un format de données texte couramment utilisé pour structurer et échanger des informations.
**Index** : Une liste organisée d'éléments pour faciliter la recherche ou la récupération.
**Répertoires** : Des dossiers ou des emplacements de stockage pour organiser des fichiers.
**Fond commun** : Une collection d'œuvres librement partagées par une organisation ou une communauté.
**Séquestre** : La mise en quarantaine ou la restriction de l'accès à certaines œuvres.
**Modération** : Le processus d'examen et d'approbation de contenus soumis, notamment pour garantir leur conformité aux règles ou aux normes.
**Statut** : L'état ou la condition actuelle d'une œuvre, notamment si elle est dans le domaine public, protégée, ou rejetée.
**Protection** : Les mesures prises pour prévenir l'accès ou l'utilisation non autorisés d'une œuvre.
**Copie** : Une reproduction d'une œuvre.
**Licence d'exploitation** : Un accord légal définissant les droits d'utilisation d'une œuvre.
**Clé** : Une série de caractères utilisée pour chiffrer ou déchiffrer des données.
**Validité** : La période pendant laquelle une œuvre ou un emprunt est en vigueur ou autorisé.
**Classification** : Le tri ou la catégorisation des œuvres en fonction de leurs caractéristiques.
**Catégories** : Des groupes ou des classifications pour regrouper des œuvres similaires.

## Mots compliqués
**Modalités** : Les conditions ou les règles spécifiques régissant un accord ou une opération.
**Chiffrées** : Les données transformées en un format illisible sans la clé de déchiffrement correspondante.
**Système de rubriques** : Une structure organisée pour classer ou organiser des informations.
**Séquestre** : La mise en quarantaine ou la restriction de l'accès à certaines œuvres.

## Réduction de la phrase pour le readme
CultureDiffusion développe une bibliothèque numérique décentralisée permettant aux membres de numériser, emprunter et proposer des œuvres, avec une modération assurée par les bibliothécaires.

## Suivi du cours sur les scénarios

## Création des scénarios

### Scénarios non détaillés

Voici 11 scénarios pour votre système de bibliothèque numérique avec des actions variées :

**1. Ajout d'une œuvre au répertoire "à modérer" :**
**Description :** Un membre propose une nouvelle œuvre.
**Acteurs :** Membre, bibliothécaires.
**Précondition :** Connexion à l'application.
**Étapes :** Le membre télécharge l'œuvre et les informations au format JSON, les soumet à la bibliothèque via l'application, où les bibliothécaires les examinent pour validation.

**2. Validation d'une œuvre par les bibliothécaires :**
**Description :** Les bibliothécaires examinent et valident les propositions d'œuvres.
**Acteurs :** Bibliothécaires.
**Précondition :** Proposition d'une œuvre par un membre.
**Étapes :** Les bibliothécaires vérifient les données, complètent les informations manquantes, et décident du statut de l'œuvre (domaine public ou sous droits).

**3. Emprunt d'une œuvre dans le répertoire "emprunts" :**
**Description :** Un membre emprunte une œuvre sous droits.
**Acteurs :** Membre.
**Précondition :** Œuvre disponible pour emprunt.
**Étapes :** Le membre sélectionne l'œuvre, la télécharge en utilisant sa clé privée pour déchiffrer, et peut accéder à l'œuvre pendant la période d'emprunt.

**4. Gestion des droits d'accès pour une œuvre sous droits :**
**Description :** L'application gère les accès aux œuvres sous droits.
**Acteurs :** Système de la bibliothèque.
**Précondition :** Statut défini pour une œuvre sous droits.
**Étapes :** L'application chiffre l'œuvre avec une clé et limite le nombre de copies selon les licences d'exploitation.

**5. Suppression d'une œuvre après la fin d'emprunt :**
**Description :** L'œuvre empruntée est automatiquement retirée du répertoire d'un membre.
**Acteurs :** Système de la bibliothèque.
**Précondition :** Fin de la période d'emprunt.
**Étapes :** L'application supprime l'accès à l'œuvre dans le répertoire du membre.

**6. Classification d'une œuvre dans plusieurs catégories :**
**Description :** Attribution de catégories à une œuvre.
**Acteurs :** Bibliothécaires.
**Précondition :** Validation de l'œuvre.
**Étapes :** Les bibliothécaires classent l'œuvre dans les catégories pertinentes, en prenant en compte ses caractéristiques multiples.

**7. Mise à jour de l'index des œuvres :**
**Description :** Actualisation de l'index de la bibliothèque.
**Acteurs :** Système de la bibliothèque.
**Précondition :** Ajout ou suppression d'une œuvre.
**Étapes :** L'application met à jour son index pour refléter les changements dans la bibliothèque.

**8. Accès à une œuvre du domaine public :**
**Description :** Accès à une œuvre du domaine public.
**Acteurs :** Membre.
**Précondition :** Œuvre du domaine public.
**Étapes :** Le membre peut télécharger l'œuvre gratuitement, sans restriction de copie.

**9. Gestion des copies pour une œuvre sous droits :**
**Description :** Contrôle du nombre de copies pour une œuvre protégée.
**Acteurs :** Système de la bibliothèque.
**Précondition :** Œuvre sous droits.
**Étapes :** L'application gère le nombre de copies autorisées en fonction des licences d'exploitation.

**10. Élargissement de la bibliothèque par un nouveau membre :**
**Description :** Un nouvel utilisateur rejoint la bibliothèque.
**Acteurs :** Nouveau membre.
**Précondition :** Création d'un compte dans l'application.
**Étapes :** Le nouveau membre crée un compte et a accès aux fonctionnalités de la bibliothèque.

**11. Rejet d'une œuvre après modération :**
**Description :** L'œuvre proposée est rejetée par les bibliothécaires.
**Acteurs :** Bibliothécaires.
**Précondition :** Proposition d'une œuvre.
**Étapes :** Après vérification, si l'œuvre ne correspond pas aux critères ou aux droits requis, elle est rejetée et supprimée du répertoire "à modérer".

---

## Version détaillée : 

### S1 : Ajout d'une œuvre au répertoire "à modérer" : Proposition d'une nouvelle œuvre

**Description :** Un utilisateur anonyme propose une nouvelle œuvre pour intégration dans la bibliothèque numérique BiblioConnect.

**Acteurs :** Utilisateur Anonyme, Bibliothécaires actifs

**Précondition :** Connexion à l'application de la bibliothèque numérique.

**Étapes détaillées :**

1. **Connexion à BiblioConnect :** Un utilisateur anonyme accède à l'application de la bibliothèque numérique, BiblioConnect.

2. **Proposition de l'œuvre :** L'utilisateur repère l'option permettant de soumettre une nouvelle œuvre pour ajout à BiblioConnect.

3. **Téléchargement de l'œuvre :** L'utilisateur sélectionne le fichier numérique de l'œuvre depuis son dispositif pour l'ajouter à la bibliothèque.

4. **Saisie des informations :** Il complète un formulaire avec les détails pertinents de l'œuvre, tels que l'auteur, édition, date de publication, éditeur, et catégorie.

5. **Soumission des données et du fichier :** Une fois les détails complétés, il envoie les informations et le fichier correspondant à BiblioConnect.

6. **Stockage dans le répertoire "à modérer" :** Ces informations sont stockées dans le répertoire "à modérer" de BiblioConnect, en attente d'examen et de validation par les bibliothécaires.

7. **Examen par les bibliothécaires :** Les bibliothécaires examinent les détails et le fichier soumis pour valider l'intégration de cette nouvelle œuvre dans BiblioConnect.

**Scenario alternatif :**

Après la soumission de l'œuvre, la bibliothèque détecte des incohérences dans les informations fournies et envoie une notification à l'utilisateur anonyme demandant des détails supplémentaires. L'utilisateur fournit les informations manquantes, mais ces dernières ne suffisent pas pour garantir l'authenticité de l'œuvre. Les bibliothécaires décident de rejeter temporairement la proposition en attendant des informations plus complètes.

### S2 : Validation d'une œuvre par les bibliothécaires

**Description :** Les bibliothécaires examinent et valident les propositions d'œuvres pour leur intégration dans la bibliothèque numérique.

**Acteurs :** Bibliothécaires.

**Précondition :** Proposition d'une œuvre par un membre.

**Étapes détaillées :**

1. **Réception des propositions :** Après qu'un membre a soumis une proposition d'œuvre pour l'intégrer dans la bibliothèque, celle-ci est transmise au groupe de bibliothécaires actifs.

2. **Examen des données :** Les bibliothécaires vérifient méticuleusement les informations fournies avec l'œuvre, y compris les détails de l'auteur, l'édition, la date de publication, l'éditeur, et d'autres données pertinentes.

3. **Complétion des informations manquantes :** Si certaines informations sont incomplètes ou manquantes, les bibliothécaires peuvent rechercher et ajouter les détails manquants pour assurer la clarté et la complétude des informations relatives à l'œuvre.

4. **Évaluation du statut de l'œuvre :** Après avoir examiné et complété les informations, les bibliothécaires décident du statut de l'œuvre. Ils déterminent si l'œuvre appartient au domaine public ou si elle est soumise à des droits d'auteur et nécessite des restrictions d'accès.

5. **Validation de l'œuvre :** Une fois que les données sont complètes et que le statut est évalué, les bibliothécaires valident l'œuvre pour son intégration dans la bibliothèque numérique.

**Scenario alternatif :**

Suite à la vérification des données, les bibliothécaires découvrent des informations contradictoires concernant les droits d'auteur. Ils contactent l'auteur de l'œuvre pour confirmer ces détails et ne reçoivent aucune réponse dans le délai imparti. Ceci conduit à une suspension temporaire de la proposition d'œuvre, en attendant la clarification des droits d'auteur.

### S3 : Classification d'une œuvre dans plusieurs catégories

**Description :** Les bibliothécaires attribuent des catégories à une œuvre pour une classification plus précise.

**Acteurs :** Bibliothécaires.

**Précondition :** Validation de l'œuvre.

**Étapes :**

1. **Validation de l'œuvre :** Une fois qu'une œuvre est validée pour inclusion dans la bibliothèque, les bibliothécaires commencent le processus de classification.

2. **Analyse des caractéristiques :** Les bibliothécaires examinent les caractéristiques de l'œuvre telles que son sujet, son genre, son style, son époque, et tout autre élément pertinent.

3. **Identification des catégories :** En se basant sur ces caractéristiques, ils déterminent les catégories les plus appropriées pour l'œuvre.

4. **Attribution des catégories :** L'œuvre est classée dans plusieurs catégories selon sa nature plurielle, et chaque catégorie est attribuée en conséquence.

5. **Saisie des données :** Les bibliothécaires enregistrent les catégories assignées à l'œuvre dans la base de données de la bibliothèque, assurant une indexation précise.

**Scenario alternatif :**

Un débat sur la classification d'une œuvre entre les bibliothécaires retarde la publication de l'œuvre, entraînant des retards dans la mise à disposition. Certains catégorisent l'œuvre dans une catégorie, tandis que d'autres suggèrent une autre, provoquant un délai supplémentaire pour la décision finale.

### S4 : Rejet d'une œuvre après modération

**Description :** L'œuvre proposée ne répond pas aux critères ou aux droits requis, et est rejetée par les bibliothécaires.

**Acteurs :** Bibliothécaires.

**Précondition :** Proposition d'une œuvre pour intégration dans la bibliothèque.

**Étapes :**

1. **Examen de l'œuvre :** Les bibliothécaires passent en revue les détails et le contenu de l'œuvre soumise dans le répertoire "à modérer".

2. **Vérification des critères :** Ils vérifient si l'œuvre correspond aux critères de la bibliothèque, tels que la légalité, la qualité, la pertinence par rapport aux directives établies.

3. **Analyse des droits :** Les bibliothécaires s'assurent que l'œuvre respecte les droits d'auteur et tout autre droit applicable.

4. **Décision de rejet :** Si l'œuvre ne répond pas aux critères requis ou ne respecte pas les droits, les bibliothécaires décident de son rejet.

5. **Suppression de l'œuvre :** L'œuvre rejetée est retirée du répertoire "à modérer" et n'est pas intégrée à la bibliothèque numérique.

**Scenario alternatif :**

Une œuvre soumise n'a pas de violation directe des droits d'auteur mais suscite des inquiétudes concernant la conformité avec les règles de contenu de la bibliothèque. Les bibliothécaires ne parviennent pas à un consensus clair sur le rejet, nécessitant une analyse plus approfondie du contenu. Cela peut potentiellement entraîner des retards dans la décision finale.


### S5 : Consulter une œuvre du domaine public:

**Description:** L'utilisateur souhaite consulter une œuvre du domaine public.
**Acteurs:** Utilisateur, Serveur de BiblioConnect.
**Prérequis:** L'utilisateur est membre et l'application est installée.
**Étapes:**
1. Le membre lance l'application.
2. Le membre choisit de consulter les œuvres du domaine public.
3. L'application affiche la liste des œuvres du domaine public.
4. L'utilisateur sélectionne une œuvre spécifique pour la consulter.
5. L'application récupère les informations et le fichier de l'œuvre du serveur.
6. L'utilisateur peut consulter l'œuvre, afficher les détails et naviguer à travers le contenu.

**Scénario alternatif (étape 4)**:
L'utilisateur utilise une fonction de recherche pour trouver une œuvre spécifique.

**Scénarios erreurs**: 
données, documents, écrans non spécifiés

## S6 : Passage d’une œuvre dans le domaine public

### Description
Lorsqu'une œuvre sous droits devient libre de droits, elle passe dans le domaine public.

### Acteurs
Bibliothécaire, Serveur de BiblioConnect.

### Prérequis
L'application est installée, et un bibliothécaire est connecté.

### Étapes
1. **Ouverture de l'application par le bibliothécaire :** Le bibliothécaire ouvre l'application et accède à la rubrique de modération des œuvres.
2. **Vérification des informations :** Une œuvre est soumise à modération, et le bibliothécaire vérifie les informations.
3. **Décision de passage dans le domaine public :** Le bibliothécaire décide que l'œuvre est maintenant dans le domaine public.
4. **Mise à jour du répertoire "fond_commun" :** L'application met à jour la rubrique "fond_commun" en ajoutant l'œuvre libre de droits.
5. **Accessibilité pour tous les membres :** L'œuvre devient accessible gratuitement pour tous les membres.

## S7 : Mise à jour de l’index des œuvres

### Description
L'index des œuvres est mis à jour suite à l'ajout ou la suppression d'une œuvre.

### Acteurs
Bibliothécaire, BiblioConnect, Serveur de l'application.

### Prérequis
L'application est installée, et un bibliothécaire est connecté.

### Étapes
1. **Modification du statut par le bibliothécaire :** Un bibliothécaire modifie le statut d'une œuvre (par exemple, le passage dans le domaine public).
2. **Mise à jour de l'index :** L'application met à jour l'index en ajoutant ou supprimant l'œuvre selon la modification effectuée.
3. **Propagation des modifications :** Les modifications sont propagées aux serveurs pour assurer la cohérence de l'index.

## S8 : Consultation des rubriques

### Description
L'utilisateur souhaite consulter les différentes rubriques de la bibliothèque.

### Acteurs
Utilisateur, Serveur de l'application.

### Prérequis
L'application est installée, et l'utilisateur est membre.

### Étapes
1. **Lancement de l'application :** L'utilisateur lance l'application.
2. **Affichage des rubriques :** L'application affiche les différentes rubriques (fond_commun, emprunts, séquestre, à modérer) en fonction des droits de l'utilisateur.
3. **Accès aux rubriques :** L'utilisateur peut accéder à chaque rubrique pour consulter les œuvres correspondantes.

## S9 : Scénario : Louer une œuvre sous droits d’auteur

### Description
Un membre souhaite louer une œuvre sous droits pour une période de 2 semaines en utilisant le système de paiement en ligne intégré à l'application.

### Acteurs
Membre, Bibliothécaires, Système de Paiement en ligne.

### Préconditions
- Le membre est connecté à l'application.
- Le membre a des informations de paiement enregistrées dans son compte.

### Étapes
1. **Exploration du répertoire "emprunts" :** Le membre explore le répertoire "emprunts" avec les œuvres sous droits disponibles.
2. **Choix de l'œuvre et demande de location :** Le membre choisit une œuvre spécifique qu'il souhaite louer et sélectionne l'option de location.
3. **Affichage des détails de la transaction :** Avant de confirmer la location, l'application affiche les détails de la transaction, y compris le coût de la location et la durée.
4. **Confirmation de la location et paiement :** Le membre confirme la location et choisit la méthode de paiement (carte de crédit enregistrée).
5. **Transmission des détails de la transaction :** L'application transmet les détails de la transaction au système de paiement en ligne, qui effectue la vérification et le traitement du paiement.
6. **Chiffrement de l'œuvre et enregistrement de la location :** Une fois le paiement réussi, l'application chiffre l'œuvre avec une clé spécifique à la transaction et enregistre la location dans l'index des œuvres empruntées par le membre.
7. **Transfert de l'œuvre chiffrée :** L'œuvre chiffrée est transférée dans le répertoire "emprunts" du membre.
8. **Accès pendant la période de location :** Pendant la période de location (2 semaines), le membre peut accéder à l'œuvre, la déchiffrer et la consulter.
9. **Rappel de la date limite de retour :** À la fin de la période de location, l'application envoie une notification au membre pour le rappeler de la date limite de retour.
10. **Retour de l'œuvre :** Le membre retourne l'œuvre en utilisant l'option de retour dans l'application.
11. **Suppression automatique :** L'application supprime automatiquement l'œuvre du répertoire "emprunts" du membre.

### Scénario Alternatif
- Si le paiement en ligne échoue, l'application informe le membre de l'échec de la transaction et l'invite à mettre à jour ses informations de paiement avant de réessayer.

### Scénario d'Erreur
- Si le système de paiement en ligne rencontre un problème technique, l'application affiche un message d'erreur et conseille au membre de réessayer ultérieurement ou de contacter le support technique.

## S10 : Mise à Jour de l’Index des Œuvres avec la Passation des Œuvres dans le Domaine Public par le Bibliothécaire

### Description
Un bibliothécaire met à jour l'index des œuvres après la passation d'une œuvre dans le domaine public, rendant ainsi l'œuvre accessible gratuitement à tous les membres.

### Acteurs
Bibliothécaire, Système.

### Préconditions
- Une œuvre sous droits a été examinée et déterminée comme passant dans le domaine public.
- Le bibliothécaire est connecté à l'application.

### Étapes
1. **Accès à la section "À Modérer" :** Le bibliothécaire accède à la section "À Modérer" de l'application où les œuvres en attente de statut sont répertoriées.
2. **Sélection de l'œuvre à mettre dans le domaine public :** Il sélectionne l'œuvre qui a été déterminée comme passant dans le domaine public.
3. **Mise à jour du statut :** Le bibliothécaire met à jour le statut de l'œuvre en le changeant pour "Domaine Public".
4. **Déplacement automatique dans "fond_commun" :** L'application déplace automatiquement l'œuvre dans le répertoire "fond_commun", rendant ainsi l'œuvre accessible gratuitement à tous les membres.
5. **Mise à jour de l'index :** L'application met à jour l'index des œuvres avec les nouvelles informations, reflétant le changement de statut.
6. **Gestion des emprunts actuels :** Si des exemplaires de l'œuvre étaient déjà empruntés, l'application maintient les emprunts actuels jusqu'à leur terme, mais les nouveaux membres peuvent désormais emprunter l'œuvre gratuitement.
7. **Ajout de commentaires ou annotations :** Le bibliothécaire peut ajouter des commentaires ou des annotations pour référence future.
8. **Notification aux membres :** L'application notifie tous les membres de la bibliothèque de la disponibilité gratuite de l'œuvre nouvellement placée dans le domaine public.

### Scénario Alternatif
- Si le bibliothécaire rencontre des difficultés techniques pendant le processus, l'application génère un message d'erreur, enregistre la situation, et informe le support technique pour résolution.

### Scénario d'Erreur
- Si une erreur survient pendant la mise à jour de l'index, l'application génère un message d'erreur et propose des options de correction. Si l'erreur est critique, l'opération est annulée, et le bibliothécaire est informé de l'incident.

## S11 : Signalement d'une œuvre litigieuse par un membre

### Description
Un membre de la bibliothèque signale une œuvre qu'il considère comme litigieuse en raison de son contenu inapproprié.

### Acteurs
Membre, Bibliothécaires, Responsable de la modération.

### Préconditions
Le membre est connecté à l'application.

### Étapes détaillées
1. **Identification de l'œuvre litigieuse :** Le membre identifie une œuvre dans le répertoire "fond_commun" qu'il estime litigieuse en raison de son contenu.
2. **Options de signalement :** L'application propose une option de signalement pour chaque œuvre. Le membre sélectionne l'œuvre en question et utilise l'option de signalement.
3. **Motif du signalement :** Le membre fournit un motif détaillé expliquant pourquoi il considère l'œuvre comme litigieuse. Il peut également attacher des captures d'écran ou d'autres preuves, le cas échéant.
4. **Notification aux bibliothécaires :** Le système envoie une notification aux bibliothécaires signalant le signalement et incluant les informations fournies par le membre.
5. **Examen par les bibliothécaires :** Les bibliothécaires examinent rapidement l'œuvre signalée et les motifs fournis par le membre.
6. **Décision de modération :** Les bibliothécaires prennent une décision concernant l'œuvre signalée. Ils peuvent choisir de la retirer temporairement, de demander des informations supplémentaires, ou de la maintenir en l'état.
7. **Communication avec le membre :** En fonction de la décision, les bibliothécaires informent le membre du résultat de la modération. S'ils demandent des informations supplémentaires, le membre est invité à fournir davantage de détails.

### Scénario Alternatif
Le membre signale une œuvre, mais les bibliothécaires estiment que le contenu ne viole pas les directives de la bibliothèque. Dans ce cas, ils informent le membre de leur décision et expliquent pourquoi l'œuvre reste disponible dans la bibliothèque.

### Scénario d'Erreur
Le système de signalement rencontre un problème technique, et les signalements ne parviennent pas aux bibliothécaires. Dans ce cas, les bibliothécaires peuvent ne pas être informés du signalement, retardant ainsi le processus de modération. Un message d'erreur est généré, et le support technique est informé pour résoudre le problème.

###  Modification des scénarios et implémentation de ceux-ci, correction, et suppression des doublons.
### Ajout des scénarios développés en externe au fichier de base et création des dossiers.
###  Après la mise en place des scénarios et la publication de ceux-ci sur GitHub, nous commençons le développement des différents diagrammes scénario par scénario et les publions directement dans les dossiers correspondants.
###  Répartition des tâches pour la création des diagrammes (Séquence / Classe) (Répartition en part égale des diagrammes) :
    - S1 : fait 
    - S2 : fait 
    - S3 : fait 
    - S4 : fait 
    - S5 : fait 
    - S6 : fait 
    - S7 : fait 
    - S8 : fait 
    - S9 : fait 
    - S10: fait 
    - S11: fait  

### Importation des fichiers dans les dossiers sur le GitHub 
### Préparation de l'oral et choix du scénario à présenter
