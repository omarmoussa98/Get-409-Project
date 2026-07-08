## Backlog S3 — GET409-YoungImmo

### HMW Définitif

> Comment pourrions-nous permettre aux étudiants dakarois à budget serré d'accéder à des annonces de logement vérifiées et à des prix transparents, afin qu'ils puissent se loger sans dépendre d'intermédiaires opaques ?

---

### User Stories MUST

*(À construire obligatoirement en S3)*

#### US-01 — Consulter les annonces vérifiées

**Story :** En tant qu'Omar, étudiant à Dakar, je veux consulter une liste d'annonces de logement vérifiées dans la zone Fann / Point E avec le prix, les photos et le statut de disponibilité, afin de ne pas perdre de temps sur des annonces fausses ou périmées.

**Priorité :** MUST

**Outil :** Bolt.new — page web responsive générée en langage naturel, déployée sur Vercel

**Effort :** Moyen — interface de listing avec filtres basiques (quartier, budget), responsive mobile Android

**Adresse :** Pain Reliever n°1 (annonces vérifiées uniquement) + Gain Creator n°3 (stock dense sur zone pilote)

**Critère d'acceptation :** Omar peut ouvrir l'URL depuis son Android en 3G, voir au moins 5 annonces avec photo compressée, prix en FCFA et mention « Disponible » ou « Loué », et filtrer par budget maximum. Temps de chargement inférieur à 5 secondes sur connexion lente.

#### US-02 — Contacter le propriétaire directement

**Story :** En tant qu'Omar, je veux cliquer sur une annonce et être redirigé vers une conversation WhatsApp avec le propriétaire vérifié, afin de le contacter directement sans passer par un démarcheur et sans payer de commission.

**Priorité :** MUST

**Outil :** Bolt.new — bouton WhatsApp avec lien `wa.me/` et message pré-rempli identifiable

**Effort :** Faible — un lien WhatsApp par annonce avec message type « Bonjour, je vous contacte via YoungImmo pour le logement à [adresse]… »

**Adresse :** Pain Reliever n°3 (gratuité côté locataire) + Gain Creator n°2 (accès direct sans intermédiaire)

**Critère d'acceptation :** Le clic ouvre WhatsApp sur le téléphone d'Omar avec le numéro du propriétaire et un message pré-rempli contenant le nom du logement. Le message inclut le mot « YoungImmo » pour permettre le comptage côté propriétaire (Métrique Nord).

#### US-03 — Agent IA de matching

**Story :** En tant qu'Omar, je veux décrire ce que je cherche (budget, quartier, date) à un chatbot WhatsApp et recevoir les 3 annonces vérifiées qui correspondent le mieux, afin de ne pas avoir à scroller toute la liste et consommer ma data.

**Priorité :** MUST

**Outil :** Dify — workflow chatbot connecté à la base d'annonces, exposé via API WhatsApp (ou simulé via interface web Dify en démo S6)

**Effort :** Élevé — nécessite la configuration d'un workflow Dify avec 3 questions séquentielles (budget, quartier, date), une base de connaissances contenant les annonces, et une logique de matching simple. Pour la démo S6, le flux peut être simulé via l'interface web Dify plutôt que via une vraie intégration WhatsApp API.

**Adresse :** Produit & Service n°3 (agent IA de matching) + Gain Creator n°2 (canal sans friction)

**Critère d'acceptation :** Omar envoie « Je cherche un studio à Fann pour moins de 80 000 FCFA, disponible en août », le chatbot répond avec 1 à 3 annonces correspondantes incluant prix, quartier et lien de contact. Le temps de réponse est inférieur à 10 secondes.

#### US-04 — Back-office annonces

**Story :** En tant qu'Awa (Dev UI de l'équipe), je veux ajouter, modifier et retirer des annonces vérifiées depuis un tableau de bord simple, afin de maintenir le stock à jour sans toucher au code.

**Priorité :** MUST

**Outil :** Bolt.new — interface admin protégée par mot de passe simple, ou Google Sheets connecté via API à la page publique

**Effort :** Moyen — formulaire d'ajout (adresse, prix, photos, numéro propriétaire, statut) + liste éditable avec bouton « Marquer comme loué ». Alternative minimale : un Google Sheets partagé qui alimente la page publique.

**Adresse :** Pain Reliever n°1 (seules les annonces vérifiées sont visibles) + Contrainte n°2 (aucune annonce non validée visible)

**Critère d'acceptation :** Awa peut ajouter une nouvelle annonce en moins de 3 minutes, la voir apparaître sur la page publique, et la passer en « Loué » en un clic. Aucun utilisateur externe ne peut publier ou modifier une annonce.

---

### User Stories SHOULD

*(À construire si le temps le permet)*

#### US-05 — Reçu de caution Wave

**Story :** En tant qu'Omar, je veux saisir le numéro de ma transaction Wave après avoir payé la caution au propriétaire et obtenir un reçu numérique consultable avec le montant, la date et les deux parties, afin d'avoir une preuve en cas de litige.

**Priorité :** SHOULD

**Outil :** Bolt.new — formulaire de saisie qui génère un récapitulatif PDF ou image téléchargeable. Pas d'intégration API Wave réelle au stade MVP — saisie déclarative par Omar.

**Effort :** Moyen — formulaire (montant, date, numéro Wave, nom propriétaire) + génération d'un récapitulatif horodaté au format image ou PDF. En démo S6, expliquer au jury que c'est une simulation fonctionnelle, pas une intégration bancaire.

**Adresse :** Produit & Service n°1 (caution certifiée Wave) + Gain Creator n°1 (confiance par la traçabilité)

**Critère d'acceptation :** Omar remplit le formulaire en moins de 2 minutes, reçoit un récapitulatif visuel avec un numéro unique, et peut le retrouver ultérieurement depuis la plateforme. Le propriétaire peut consulter le même récapitulatif via un lien partagé.

#### US-06 — Tableau de bord métriques

**Story :** En tant qu'Oumarou (PM), je veux voir sur un écran unique le nombre de mises en relation (Métrique Nord), le nombre d'annonces actives (P1) et le nombre de faux contacts signalés (A1), afin de présenter ces 3 chiffres à la démo S6.

**Priorité :** SHOULD

**Outil :** Bolt.new — page dashboard simple avec 3 compteurs, alimentée manuellement ou via le Google Sheets du back-office

**Effort :** Faible — 3 cartes avec chiffre + objectif + couleur (vert si atteint, rouge si alerte)

**Adresse :** Métriques de succès (tableau de bord S6)

**Critère d'acceptation :** Les 3 métriques sont visibles sur un seul écran, avec la valeur réelle et la valeur cible côte à côte. L'écran est projetable en plein écran pour la démo S6.

---

### User Stories COULD

*(Roadmap post-MVP)*

#### US-07 — Avis communautaires des anciens locataires

**Story :** En tant qu'Omar, je veux lire les avis vérifiés d'anciens locataires d'un logement avant de le visiter, afin de savoir si l'état réel correspond à ce qui est annoncé.

**Priorité :** COULD

**Outil :** Bolt.new — section avis sous chaque annonce

**Effort :** Élevé — nécessite un système d'authentification pour vérifier que l'auteur a réellement habité le logement, ce qui dépasse le périmètre no-code débutant en S3

**Adresse :** Produit & Service n°2 (vérification communautaire)

**Critère d'acceptation :** Un ancien locataire peut soumettre un avis (texte + note 1–5) qui apparaît sous l'annonce après validation par l'équipe.

#### US-08 — Expansion géographique multi-quartiers

**Story :** En tant qu'Omar, je veux chercher des logements dans d'autres quartiers (Mermoz, Parcelles Assainies, Liberté 6) en plus de la zone pilote, afin d'élargir mes options.

**Priorité :** COULD

**Outil :** Bolt.new — filtre quartier étendu + back-office adapté

**Effort :** Moyen sur le plan technique, élevé sur le plan opérationnel (constituer le stock d'annonces vérifiées dans chaque nouveau quartier)

**Adresse :** Hypothèse S2 (expansion géographique avec le même modèle)

**Critère d'acceptation :** Au moins 5 annonces vérifiées disponibles dans un deuxième quartier, avec le même niveau de qualité que la zone pilote.

#### US-09 — Monétisation côté propriétaire

**Story :** En tant que propriétaire dans la zone Fann / Point E, je veux payer un forfait modique (2 000–5 000 FCFA) pour que mon annonce reste visible et prioritaire, afin de recevoir des locataires qualifiés plus rapidement.

**Priorité :** COULD

**Outil :** Bolt.new — badge « Annonce prioritaire » + paiement Wave

**Effort :** Moyen — nécessite la validation de l'hypothèse S1 (disposition à payer) avant toute construction

**Adresse :** Hypothèse S1 (modèle économique côté propriétaire)

**Critère d'acceptation :** Au moins 3 propriétaires sur 10 acceptent de payer le forfait après 1 mois de MVP gratuit.

---

### Sprint S3

**Semaine 1 :** US-01 (listing annonces) + US-04 (back-office) + US-02 (lien WhatsApp). L'objectif est d'avoir une page publique fonctionnelle avec au moins 5 annonces vérifiées et un bouton de contact direct avant la fin de la semaine. En parallèle, Khadidiatou et Ndeye Absa commencent la configuration du workflow Dify pour US-03.

**Semaine 2 :** US-03 (agent IA Dify) + US-06 (dashboard métriques) si le temps le permet. Tester le chatbot avec 5 étudiants du campus pour valider l'hypothèse C3. Commencer la collecte des métriques réelles.

**Démo S6 :** Démontrer en live les 3 parcours suivants devant le jury :
1. Omar ouvre YoungImmo sur son téléphone, filtre par budget, et contacte un propriétaire en 3 clics (US-01 + US-02)
2. Omar envoie un message au chatbot Dify et reçoit 3 annonces correspondantes (US-03)
3. Le PM affiche le tableau de bord avec les 3 métriques : mises en relation / annonces actives / alertes (US-06)
