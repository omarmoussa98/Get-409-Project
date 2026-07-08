## Contraintes MVP — GET409-YoungImmo

### Persona

Omar Ba · 30 ans · Étudiant en Master avec petit job à temps partiel · Dakar, Sénégal (cherche autour de Point E, Fann, Mermoz) · Smartphone Android entrée de gamme, forfait data prépayé, WhatsApp, Facebook, Wave

### HMW définitif

> Comment pourrions-nous permettre aux étudiants dakarois à budget serré d'accéder à des annonces de logement vérifiées et à des prix transparents, afin qu'ils puissent se loger sans dépendre d'intermédiaires opaques ?

---

### Contraintes Non Négociables

#### Contrainte 1

**Critère :** Le MVP DOIT fonctionner sur un smartphone Android entrée de gamme avec une connexion data limitée (forfait prépayé, réseau 3G instable).

**Origine :** Chapeau Blanc — la majorité des étudiants dakarois utilisent un Android bas de gamme avec un forfait rechargé au coup par coup. Toute solution qui consomme trop de data ou nécessite un appareil performant exclut la cible.

**Élimine :** Application native lourde à télécharger (APK > 20 Mo), interface riche en images haute résolution chargées automatiquement, fonctionnalités nécessitant une connexion permanente (streaming vidéo de visites virtuelles).

#### Contrainte 2

**Critère :** Le MVP DOIT afficher uniquement des annonces dont le prix, la localisation et la disponibilité ont été vérifiés avant publication — aucune annonce non validée ne doit être visible par Omar.

**Origine :** Chapeau Blanc — les annonces circulent aujourd'hui sur WhatsApp et Facebook sans aucune modération ni vérification, ce qui est la source directe de la méfiance d'Omar. Chapeau Noir — sans stock initial d'annonces vérifiées, la plateforme reproduit exactement le problème qu'elle prétend résoudre.

**Élimine :** Publication libre par n'importe qui (modèle Leboncoin/Expat-Dakar), système de « marketplace ouverte » où les démarcheurs peuvent poster sans contrôle, toute fonctionnalité de mise en ligne instantanée sans validation préalable.

#### Contrainte 3

**Critère :** Le MVP NE DOIT PAS facturer l'étudiant pour accéder aux annonces ni lui imposer de commission pour contacter un propriétaire.

**Origine :** Chapeau Noir — les étudiants à budget serré sont le segment le plus difficile à monétiser. Un modèle freemium ou à commission côté locataire reproduit exactement le problème des démarcheurs opaques (payer pour accéder à une information).

**Élimine :** Modèle d'abonnement côté locataire, commission prélevée sur le locataire à la mise en relation, paywall sur les coordonnées du propriétaire, annonces « premium » visibles uniquement en version payante.

#### Contrainte 4

**Critère :** Le MVP DOIT se concentrer sur un périmètre géographique restreint (un ou deux quartiers proches des campus : Fann, Point E) pour garantir un stock d'annonces suffisant dès le lancement.

**Origine :** Chapeau Noir — le risque de cold start (pas d'annonces = pas d'utilisateurs = pas d'annonces) est le risque n°1 identifié. Disperser l'effort sur tout Dakar garantit une plateforme vide partout plutôt qu'une plateforme utile quelque part.

**Élimine :** Couverture de tout Dakar au lancement, fonctionnalité de recherche par carte sur l'ensemble de la région, expansion vers la banlieue (Pikine, Guédiawaye, Parcelles Assainies) avant validation du modèle sur la zone pilote.

#### Contrainte 5

**Critère :** Le MVP DOIT intégrer Wave ou Orange Money comme moyen de traçabilité des paiements de caution, avec un reçu numérique consultable par le locataire et le propriétaire.

**Origine :** Chapeau Blanc — Wave est déjà massivement adopté par la cible. La caution (2–3 mois d'avance) est la frustration n°2 d'Omar, et l'absence de trace écrite rend tout litige impossible à résoudre.

**Élimine :** Paiement en espèces sans traçabilité, intégration de moyens de paiement non présents au Sénégal (Stripe, PayPal), système de paiement par carte bancaire (taux de bancarisation trop faible chez la cible).

---

### Fonctionnalités Éliminées

- **Visite virtuelle en vidéo** → éliminée parce que la contrainte 1 (data limitée, Android entrée de gamme) rend le streaming vidéo inutilisable pour Omar. Des photos compressées et vérifiées suffisent au MVP.

- **Publication libre d'annonces (modèle marketplace ouverte)** → éliminée parce que la contrainte 2 (annonces vérifiées uniquement) interdit toute mise en ligne sans validation. Le MVP fonctionne avec un stock d'annonces vérifiées manuellement, pas avec du contenu généré par les utilisateurs.

- **Abonnement ou commission côté locataire** → éliminé parce que la contrainte 3 (gratuité pour l'étudiant) l'interdit. La monétisation devra venir du côté propriétaire (visibilité, contacts qualifiés) ou d'un partenaire (agence, institution).

- **Couverture géographique de tout Dakar** → éliminée parce que la contrainte 4 (zone pilote restreinte) impose de concentrer le stock d'annonces. L'expansion viendra après validation sur Fann / Point E.

- **Système de messagerie intégrée entre locataire et propriétaire** → éliminé parce que WhatsApp remplit déjà cette fonction et qu'Omar l'utilise quotidiennement. Recréer une messagerie dans le MVP consomme du temps de développement sans valeur ajoutée — le MVP fournit le numéro vérifié du propriétaire, la conversation se fait sur WhatsApp.

- **Notation et avis des propriétaires par les locataires** → éliminée au MVP parce qu'elle nécessite une masse critique d'utilisateurs pour être utile (problème de cold start). Fonctionnalité pertinente en V2 une fois la base d'utilisateurs établie.

---

### Critère de Validation Final

Le MVP est valide si et seulement si : un étudiant dakarois peut, depuis un smartphone Android entrée de gamme en 3G, consulter des annonces de logement vérifiées dans la zone Fann / Point E avec des prix transparents, contacter directement le propriétaire sans frais, et tracer le paiement de sa caution via Wave — le tout sans passer par un démarcheur.
