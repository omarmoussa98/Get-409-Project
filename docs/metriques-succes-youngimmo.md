## Métriques de Succès — GET409-YoungImmo

### MVP

YoungImmo permet aux étudiants dakarois de consulter des annonces de logement vérifiées dans la zone Fann / Point E avec des prix affichés, et de contacter directement le propriétaire sans passer par un démarcheur. Le paiement de la caution est traçable via Wave avec un reçu numérique.

---

### ⭐ Métrique Nord

**Indicateur :** Nombre d'étudiants ayant contacté un propriétaire via une annonce vérifiée sur YoungImmo (mise en relation effective, pas juste une consultation).

**Valeur cible à 30 jours :** 15 mises en relation effectives — c'est-à-dire 15 étudiants distincts qui ont cliqué sur le lien WhatsApp du propriétaire ou utilisé le numéro fourni par la plateforme.

**Comment mesurer :** Chaque annonce contient un lien WhatsApp avec un message pré-rempli identifiable (ex : « Bonjour, je vous contacte via YoungImmo pour le studio à Fann… »). Compter les messages reçus côté propriétaire lors du rappel hebdomadaire de suivi. Alternative : compteur de clics sur le lien WhatsApp intégré à la page web (Bolt.new le permet nativement).

---

### 📈 Métriques de Progression

#### Métrique P1

**Indicateur :** Nombre d'annonces vérifiées publiées et actives sur la plateforme.

**Valeur cible à 30 jours :** 15 annonces actives (disponibilité confirmée dans la semaine).

**Comment mesurer :** Tableur Google Sheets partagé par l'équipe. Chaque annonce a une ligne avec la date de publication, la date de dernière vérification et le statut (active / louée / expirée). Awa (Dev UI) met à jour chaque vendredi après un appel rapide au propriétaire.

#### Métrique P2

**Indicateur :** Nombre de visiteurs uniques sur la plateforme YoungImmo par semaine.

**Valeur cible à 30 jours :** 100 visiteurs uniques cumulés sur les 4 premières semaines (soit environ 25/semaine en régime de croisière).

**Comment mesurer :** Compteur de visites intégré à la page Bolt.new (analytics basiques gratuits). Si non disponible, utiliser un raccourcisseur de lien traçable (Bitly gratuit) pour le lien partagé dans les groupes WhatsApp étudiants.

#### Métrique P3

**Indicateur :** Nombre de propriétaires ayant accepté de renouveler ou mettre à jour leur annonce après la première publication.

**Valeur cible à 30 jours :** Au moins 8 propriétaires sur les 15 initiaux renouvellent ou confirment la disponibilité de leur annonce après 2 semaines — signe que le canal leur apporte de la valeur.

**Comment mesurer :** Lors du rappel de suivi du vendredi (même appel que P1), poser la question : « Souhaitez-vous maintenir votre annonce ? Avez-vous reçu des contacts via YoungImmo ? » Réponse notée dans le tableur.

---

### 🚨 Métriques d'Alerte

#### Alerte A1

**Signal :** Le taux de « faux contact » — un étudiant contacte un propriétaire via YoungImmo mais le logement est déjà loué ou le prix annoncé ne correspond pas au prix réel demandé.

**Seuil :** Si plus de 3 cas de faux contact sont remontés sur une période de 2 semaines, la promesse de vérification est rompue et la confiance de la cible s'effondre.

**Action corrective :** Passer d'une vérification hebdomadaire à une vérification tous les 3 jours pour les annonces actives. Retirer immédiatement toute annonce signalée comme inexacte. Appeler le propriétaire concerné pour comprendre l'écart (a-t-il loué entre-temps ? a-t-il changé son prix ?).

#### Alerte A2

**Signal :** Aucun nouveau propriétaire n'accepte de publier sur la plateforme pendant 2 semaines consécutives — le stock d'annonces stagne ou diminue sans renouvellement.

**Seuil :** 0 nouvelle annonce ajoutée sur 14 jours alors que des annonces existantes expirent (logements loués).

**Action corrective :** Organiser une session terrain d'urgence : toute l'équipe consacre un après-midi au porte-à-porte dans la zone pilote avec la maquette mise à jour et les témoignages des premiers propriétaires satisfaits. Si le blocage persiste, tester un élargissement de zone (Mermoz) ou un changement de canal d'acquisition (partenariat avec une agence immobilière locale qui accepterait d'alimenter le stock).

---

### Tableau de Bord S6

À la démo S6, nous présenterons ces 3 chiffres :

1. **Métrique Nord** — Mises en relation effectives : objectif 15, valeur réelle = [à compléter le jour J]
2. **Métrique P1** — Annonces vérifiées actives : objectif 15, valeur réelle = [à compléter le jour J]
3. **Alerte A1** — Faux contacts signalés : seuil critique = 3, nombre réel = [à compléter le jour J]
