# 6 Chapeaux de Bono — YoungImmo

## HMW analysé

> Comment pourrions-nous permettre aux étudiants dakarois à budget serré d'accéder à des annonces de logement vérifiées et à des prix transparents afin qu'ils puissent se loger sans dépendre de démarcheurs opaques ?

---

## 🤍 Chapeau Blanc — Faits & Données

- Dakar compte plus de 80 000 étudiants dans le supérieur, dont une large part vient de régions extérieures et doit trouver un logement en ville. Les résidences universitaires du COUD ne couvrent qu'une fraction de la demande — la majorité passe par le marché locatif informel.
- Les annonces circulent principalement via des groupes WhatsApp privés (« Location Dakar », « Appartements Dakar ») et des pages Facebook sans aucune modération ni vérification. Il n'existe pas de plateforme locale dominante qui filtre les annonces frauduleuses pour le segment étudiant.
- La caution standard à Dakar est de 2 à 3 mois de loyer payée d'avance en espèces ou via Wave. Pour un studio à 75 000 FCFA/mois dans les Parcelles Assainies, cela représente 150 000 à 225 000 FCFA d'un coup — soit 2 à 4 mois de revenus d'un étudiant qui travaille à temps partiel.

---

## ❤️ Chapeau Rouge — Émotions & Intuitions

- L'intuition forte est que la méfiance est devenue le sentiment dominant du marché locatif étudiant à Dakar : les locataires ne font pas confiance aux démarcheurs, les propriétaires ne font pas confiance aux étudiants, et personne n'a d'outil pour vérifier quoi que ce soit. Une solution qui crée de la confiance aura un impact émotionnel immédiat.
- Il y a une frustration sourde chez les étudiants qui dépasse le logement : c'est le sentiment de ne pas être pris au sérieux dans sa propre ville parce qu'on n'a pas de fiche de paie. Cette frustration peut devenir un moteur d'adoption très puissant si l'application leur donne une forme de dignité dans le processus.
- Côté propriétaire (même s'il n'est pas notre persona principal), il y a probablement une fatigue de gérer les locataires au cas par cas via des appels et du cash sans traçabilité — une intuition à valider en S2 pour comprendre si l'offre aussi est prête à migrer vers un outil.

---

## 🖤 Chapeau Noir — Risques & Critique

- **Risque de marché vide au lancement (cold start) :** sans un stock initial d'annonces vérifiées, les premiers utilisateurs trouveront une application vide et ne reviendront pas. Or vérifier une annonce demande du temps, un passage physique ou un appel au propriétaire — c'est un coût opérationnel élevé avant même d'avoir un seul utilisateur.
- **Résistance des démarcheurs :** les intermédiaires informels vivent de l'opacité du marché. Si l'application commence à les court-circuiter, ils peuvent activement décourager les propriétaires de publier dessus, ou publier eux-mêmes de fausses annonces pour saboter la confiance dans la plateforme.
- **Faible capacité de paiement de la cible :** les étudiants à budget serré sont le segment le plus difficile à monétiser. Un modèle freemium ou à commission risque de reproduire exactement le problème qu'Omar dénonce (payer un intermédiaire pour accéder à une annonce).

---

## 💛 Chapeau Jaune — Optimisme & Valeur

- Le timing est favorable : la pénétration de Wave et Orange Money est massive chez les étudiants dakarois. Une traçabilité des paiements de caution via mobile money est techniquement faisable aujourd'hui, et elle répond à la frustration n°1 d'Omar (aucune preuve en cas de litige).
- Le volume de la demande est structurellement supérieur à l'offre dans les quartiers universitaires, ce qui signifie qu'un propriétaire qui publie une annonce vérifiée sur la plateforme recevra des contacts qualifiés très vite — c'est une proposition de valeur immédiate côté offre, sans avoir à le convaincre longtemps.
- Le projet peut démarrer ultra-léger : un simple bot WhatsApp qui relaie des annonces vérifiées manuellement suffit comme MVP, puisque WhatsApp est déjà le canal naturel d'Omar. Pas besoin d'une app native pour valider l'hypothèse — c'est aligné avec la logique no-code du cours (Bolt.new, Dify).

---

## 💚 Chapeau Vert — Créativité & Idées

- **Système de « caution certifiée » via Wave :** au lieu de remettre le cash au propriétaire, Omar verse la caution sur un compte séquestre Wave intégré à l'application. Le propriétaire voit la preuve de solvabilité, Omar a un reçu numérique et une garantie de restitution. Cela transforme le point de douleur n°2 (coût d'entrée) en fonctionnalité différenciante.
- **Vérification communautaire des annonces :** les anciens locataires d'un logement peuvent laisser un avis vérifié (« j'ai vécu ici, voici l'état réel »). Cela résout le problème du cold start sans coût opérationnel élevé — ce sont les utilisateurs eux-mêmes qui alimentent la confiance.
- **Agent IA Dify pour le matching :** un chatbot WhatsApp (construit en S3 sur Dify) qui pose 3 questions à Omar (budget, quartier souhaité, date d'emménagement) et lui envoie par SMS les 3 annonces vérifiées les plus proches de ses critères. Pas d'app à télécharger, pas de data à consommer en scrollant.

---

## 💙 Chapeau Bleu — Processus & Organisation

- La priorité immédiate est de valider le persona Omar par une vraie interview d'empathie (prompt S2) avec au moins 2–3 étudiants en situation réelle de recherche de logement à Dakar, avant de figer le HMW et de passer à l'idéation.
- Le MVP doit se concentrer sur un seul quartier (par exemple Fann ou Point E, proches des campus) pour constituer un stock d'annonces vérifiées suffisant sans disperser l'effort — l'expansion géographique viendra après validation.
- Le rôle de Responsable Impact doit cadrer dès maintenant la question éthique de la donnée : quelles informations personnelles on collecte sur Omar et sur le propriétaire, où elles sont stockées, et comment on évite que la plateforme devienne elle-même un nouvel intermédiaire opaque.

---

## 🔵 Synthèse Chapeau Bleu

**HMW révisé :** Comment pourrions-nous permettre aux étudiants dakarois à budget serré d'accéder à des annonces de logement vérifiées, avec des prix transparents et une traçabilité des paiements de caution, afin qu'ils puissent se loger en confiance sans dépendre de démarcheurs opaques ?

**Risques prioritaires :** Le problème du cold start (pas d'annonces = pas d'utilisateurs = pas d'annonces) / La monétisation d'une cible à très faible pouvoir d'achat sans reproduire le modèle de commission des démarcheurs

**Question ouverte :** Les propriétaires des quartiers universitaires sont-ils prêts à publier directement sur une plateforme ouverte, ou leur dépendance aux démarcheurs est-elle aussi subie que celle d'Omar — et donc une opportunité des deux côtés du marché ?
