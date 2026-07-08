## Hypothèses de Validation — GET409-YoungImmo

### HMW Définitif

> Comment pourrions-nous permettre aux étudiants dakarois à budget serré d'accéder à des annonces de logement vérifiées et à des prix transparents, afin qu'ils puissent se loger sans dépendre d'intermédiaires opaques ?

---

### Hypothèses CRITIQUES

*(Si fausse → le MVP ne fonctionne pas)*

#### Hypothèse C1 — Les propriétaires acceptent de publier directement

**Affirmation :** Nous croyons que les propriétaires de studios et chambres dans la zone Fann / Point E sont prêts à publier leurs annonces sur une plateforme ouverte plutôt que de passer par des démarcheurs informels, parce qu'ils y gagneraient des locataires qualifiés plus rapidement.

**Indicateur :** Nous le saurons si au moins 5 propriétaires sur 10 contactés acceptent de fournir les informations de leur logement (prix, photos, disponibilité) pour publication sur la plateforme, sans exiger de commission en retour.

**Méthode :** Entretiens en face-à-face avec 10 propriétaires identifiés dans la zone pilote. Préparer une maquette papier ou écran de ce à quoi ressemblerait leur annonce pour rendre la proposition concrète.

**Qui valide :** Marie Fall (Responsable Impact) + Oumarou Moussa (PM) — binôme terrain.

**Délai S3 :** Semaine 1 — c'est le bloquant absolu. Sans offre, il n'y a pas de plateforme.

#### Hypothèse C2 — Le stock initial d'annonces vérifiées est constituable

**Affirmation :** Nous croyons qu'il est possible de constituer un stock minimum de 10 annonces vérifiées (prix, photos, disponibilité confirmés) dans la zone Fann / Point E en moins de deux semaines, avec les ressources de l'équipe seule (pas de budget marketing).

**Indicateur :** Nous le saurons si l'équipe parvient à publier 10 annonces vérifiées en 10 jours ouvrés, en combinant le porte-à-porte (pancartes « À louer »), les contacts issus de C1 et le réseau étudiant de l'équipe.

**Méthode :** Test opérationnel — chaque membre de l'équipe consacre 2 heures par semaine au repérage terrain dans la zone pilote. Comptage brut du nombre d'annonces collectées et vérifiées.

**Qui valide :** Awa Kone (Dev UI) tient le tableau de suivi des annonces. Khadidiatou Faye ou Ndeye Absa Déme Gueye (Prompt Engineers) rédigent et formatent les annonces.

**Délai S3 :** Semaines 1 et 2 — en parallèle de C1.

#### Hypothèse C3 — Omar utilise réellement la plateforme plutôt que WhatsApp

**Affirmation :** Nous croyons qu'un étudiant en recherche de logement préférera consulter une plateforme d'annonces vérifiées plutôt que scroller les groupes WhatsApp « Location Dakar », parce que la vérification des annonces lui fait gagner du temps et de l'argent en déplacements inutiles.

**Indicateur :** Nous le saurons si, sur 10 étudiants à qui on présente le MVP (même en version maquette), au moins 7 déclarent qu'ils l'utiliseraient en priorité par rapport aux groupes WhatsApp, et au moins 3 effectuent une action concrète (cliquer sur une annonce, contacter un propriétaire via le lien fourni).

**Méthode :** Test utilisateur en contexte — montrer le MVP (ou une maquette cliquable) à 10 étudiants en recherche active de logement sur le campus, puis observer leur comportement et recueillir leur réaction à chaud.

**Qui valide :** Khadidiatou Faye et Ndeye Absa Déme Gueye (Prompt Engineers) mènent les tests utilisateurs. Oumarou Moussa (PM) observe et note.

**Délai S3 :** Semaine 2 — une fois le stock d'annonces constitué (C2).

---

### Hypothèses IMPORTANTES

*(Si fausse → expérience dégradée mais MVP utilisable)*

#### Hypothèse I1 — Les démarcheurs ne sabotent pas la plateforme

**Affirmation :** Nous croyons que les démarcheurs informels n'auront pas un impact significatif sur la plateforme au stade MVP, parce que le volume d'annonces sera trop faible pour menacer leur activité et que la zone pilote est restreinte.

**Indicateur :** Nous le saurons si, après 2 semaines de fonctionnement du MVP, aucune annonce vérifiée n'a été signalée comme frauduleuse ou détournée, et qu'aucun propriétaire participant ne s'est retiré sous pression d'un démarcheur.

**Méthode :** Suivi qualitatif — rappeler chaque propriétaire participant après 2 semaines pour vérifier s'il a subi des pressions ou des désagréments liés à sa publication sur la plateforme.

**Qui valide :** Marie Fall (Responsable Impact) — c'est une question d'éthique et d'impact sur l'écosystème.

**Délai S3 :** Semaine 3 — après le lancement du MVP.

#### Hypothèse I2 — La traçabilité de la caution via Wave apporte de la confiance

**Affirmation :** Nous croyons que proposer un reçu numérique Wave pour le paiement de la caution augmente significativement la confiance d'Omar dans le processus de location, même si le paiement se fait directement entre locataire et propriétaire (pas de séquestre).

**Indicateur :** Nous le saurons si, lors des tests utilisateurs (C3), au moins 6 étudiants sur 10 déclarent que la fonctionnalité de reçu numérique les rassurerait au moment de verser la caution.

**Méthode :** Question intégrée au test utilisateur de C3 — montrer un écran simulé de « reçu de caution Wave » et mesurer la réaction (échelle de confiance 1–5).

**Qui valide :** Khadidiatou Faye et Ndeye Absa Déme Gueye (Prompt Engineers) lors des tests utilisateurs.

**Délai S3 :** Semaine 2 — en même temps que C3.

---

### Hypothèses SECONDAIRES

*(À valider après le MVP)*

#### Hypothèse S1 — Le modèle économique peut reposer sur le propriétaire

**Affirmation :** Nous croyons que les propriétaires sont prêts à payer un forfait modique (entre 2 000 et 5 000 FCFA par annonce) pour accéder à des locataires qualifiés via la plateforme, parce que c'est moins cher et plus rapide que de passer par un démarcheur (qui prend souvent un mois de loyer en commission).

**Indicateur :** Nous le saurons si, parmi les propriétaires ayant participé au MVP gratuit, au moins 3 sur 10 déclarent qu'ils seraient prêts à payer ce forfait pour renouveler ou maintenir leur annonce.

**Méthode :** Entretien de sortie avec les propriétaires participants après 1 mois de MVP — question directe sur la disposition à payer.

**Qui valide :** Oumarou Moussa (PM) + Marie Fall (Responsable Impact).

**Délai :** Après le MVP — hors périmètre S3.

#### Hypothèse S2 — L'expansion géographique fonctionne avec le même modèle

**Affirmation :** Nous croyons que le modèle validé sur Fann / Point E peut se répliquer dans d'autres quartiers à forte population étudiante (Mermoz, Parcelles Assainies, Liberté 6) sans modifier fondamentalement la mécanique de vérification des annonces.

**Indicateur :** Nous le saurons si, lors d'un test exploratoire dans un deuxième quartier, le ratio d'annonces vérifiables par semaine est comparable à celui de la zone pilote (au moins 5 annonces / semaine / membre mobilisé).

**Méthode :** Déploiement pilote dans un deuxième quartier avec un seul membre de l'équipe pendant 2 semaines.

**Qui valide :** Awa Kone (Dev UI) — test opérationnel.

**Délai :** Après le MVP — hors périmètre S3.

---

### Priorité de Validation S3

La première chose à tester en S3 : aller frapper aux portes de 10 propriétaires de la zone Fann / Point E avec une maquette de l'annonce type, pour vérifier qu'ils acceptent de publier directement — si l'offre ne vient pas, rien d'autre ne fonctionne.
