# Value Proposition Canvas — GET409-YoungImmo

## HMW Définitif

> Comment pourrions-nous permettre aux étudiants dakarois à budget serré d'accéder à des annonces de logement vérifiées et à des prix transparents, afin qu'ils puissent se loger sans dépendre d'intermédiaires opaques ?

---

## 👤 Profil Client — Omar Ba

### 🔧 Jobs To Be Done

*(Source : Chapeau Blanc)*

- Trouver un logement abordable à proximité des campus universitaires de Dakar dans un marché où la demande étudiante dépasse largement l'offre du COUD *(Blanc — « plus de 80 000 étudiants, résidences universitaires ne couvrent qu'une fraction »)*
- Distinguer les annonces fiables des annonces frauduleuses dans un écosystème sans aucune modération ni vérification *(Blanc — « groupes WhatsApp et pages Facebook sans aucune modération ni vérification »)*
- Réunir la caution de 2 à 3 mois de loyer d'avance avec des revenus irréguliers, tout en conservant une preuve de paiement *(Blanc — « 150 000 à 225 000 FCFA d'un coup, soit 2 à 4 mois de revenus d'un étudiant »)*

### 😣 Pains

*(Sources : Chapeau Rouge + Chapeau Noir)*

- La méfiance est devenue le sentiment par défaut de toute interaction locative : Omar s'attend à être trompé avant même de commencer sa recherche *(Rouge — « la méfiance est devenue le sentiment dominant du marché locatif étudiant »)*
- Le sentiment de ne pas être pris au sérieux parce qu'il est étudiant sans fiche de paie, ce qui génère une frustration qui dépasse la question du logement *(Rouge — « sentiment de ne pas être pris au sérieux dans sa propre ville parce qu'on n'a pas de fiche de paie »)*
- Sans stock initial d'annonces vérifiées, toute plateforme est vide et reproduit le problème qu'elle prétend résoudre — Omar arrive, ne trouve rien, et retourne sur WhatsApp *(Noir — « cold start : pas d'annonces = pas d'utilisateurs = pas d'annonces »)*
- Les démarcheurs peuvent activement saboter la plateforme en décourageant les propriétaires ou en publiant de fausses annonces *(Noir — « les intermédiaires informels vivent de l'opacité du marché »)*
- Toute commission ou abonnement facturé à Omar reproduit exactement le modèle qu'il dénonce *(Noir — « un modèle freemium ou à commission risque de reproduire exactement le problème »)*

### 🌟 Gains

*(Source : Chapeau Jaune)*

- Pouvoir tracer le paiement de sa caution via Wave, un outil qu'il utilise déjà au quotidien, et disposer d'une preuve en cas de litige *(Jaune — « la pénétration de Wave est massive, traçabilité techniquement faisable »)*
- Accéder à des propriétaires qui reçoivent des contacts qualifiés rapidement, ce qui les incite à jouer le jeu de la transparence *(Jaune — « un propriétaire recevra des contacts qualifiés très vite — proposition de valeur immédiate côté offre »)*
- Utiliser un service qui fonctionne sur son canal habituel (WhatsApp) sans télécharger une nouvelle application ni consommer de data supplémentaire *(Jaune — « un simple bot WhatsApp suffit comme MVP, WhatsApp est déjà le canal naturel d'Omar »)*

---

## 💡 Proposition de Valeur — YoungImmo

### 📦 Produits & Services

*(Source : Chapeau Vert)*

- **Caution certifiée Wave :** Omar verse sa caution sur un mécanisme traçable via Wave. Le propriétaire voit la preuve de solvabilité, Omar obtient un reçu numérique consultable *(Vert — « compte séquestre Wave intégré, reçu numérique et garantie de restitution »)*
- **Vérification communautaire des annonces :** les anciens locataires d'un logement laissent un avis vérifié sur l'état réel du bien, alimentant la confiance sans coût opérationnel élevé pour l'équipe *(Vert — « les utilisateurs eux-mêmes alimentent la confiance »)*
- **Agent IA de matching via WhatsApp :** un chatbot construit sur Dify qui pose 3 questions à Omar (budget, quartier, date) et lui envoie les annonces vérifiées correspondantes, sans app à télécharger ni data à consommer en scrollant *(Vert — « chatbot WhatsApp construit en S3 sur Dify »)*

### 💊 Pain Relievers

*(Source : Chapeau Noir — mitigations)*

- **Méfiance généralisée** → YoungImmo ne publie que des annonces vérifiées (prix, photos, disponibilité confirmés) avant mise en ligne. Aucune publication libre n'est possible, ce qui élimine le bruit et les arnaques à la source *(Noir — mitigation du cold start par un stock vérifié manuellement avant lancement)*
- **Sabotage par les démarcheurs** → Lancement sur une zone pilote restreinte (Fann / Point E) où le volume est trop faible pour menacer l'activité des démarcheurs. Suivi qualitatif des propriétaires participants pour détecter toute pression *(Noir — mitigation par restriction géographique et monitoring)*
- **Risque de reproduire le modèle payant des démarcheurs** → Accès 100% gratuit pour Omar. La monétisation repose sur le propriétaire (forfait modique pour visibilité auprès de locataires qualifiés), validée en hypothèse secondaire après le MVP *(Noir — mitigation par gratuité côté demande)*

### 🎁 Gain Creators

*(Source : Chapeau Jaune + Chapeau Bleu)*

- **Confiance par la traçabilité :** chaque paiement de caution via Wave génère un reçu numérique horodaté, consultable par les deux parties. Omar a une preuve, le propriétaire a une confirmation — la confiance n'est plus interpersonnelle, elle est documentée *(Jaune — « traçabilité des paiements de caution via mobile money techniquement faisable »)*
- **Accès direct sans intermédiaire :** la mise en relation se fait via un lien WhatsApp vers le propriétaire vérifié. Pas de commission, pas de numéro masqué, pas de démarcheur entre les deux *(Jaune — « proposition de valeur immédiate côté offre »)*
- **Concentration géographique pour qualité maximale :** en se limitant à Fann / Point E, le MVP garantit un stock d'annonces dense et à jour plutôt qu'une couverture large mais vide *(Bleu — « se concentrer sur un seul quartier pour constituer un stock suffisant »)*

---

## ✅ FIT Check

*(Source : Chapeau Bleu)*

**Combinaison synergique retenue :** Les 3 Produits & Services (caution Wave, vérification communautaire, agent IA WhatsApp) répondent chacun à un Pain distinct et créent chacun un Gain tracé. La caution Wave adresse le Pain émotionnel de méfiance (Rouge) et crée le Gain de traçabilité (Jaune). La vérification communautaire adresse le Pain fonctionnel du cold start (Noir) et crée le Gain de confiance documentée (Jaune). L'agent IA WhatsApp adresse le Pain fonctionnel de l'accès (Noir — commission) et crée le Gain d'un canal sans friction (Jaune).

**Pain Relievers sans Pain correspondant :** Aucun — chaque Pain Reliever est directement mappé à un Pain identifié dans les Chapeaux Rouge ou Noir.

**Éléments non tracés :** Aucun — tous les éléments du Canvas sont traçables à un Chapeau d'origine.

**Conclusion :** Le FIT est solide sur le papier. Chaque fonctionnalité du MVP est justifiée par un fait (Blanc), motivée par une douleur (Rouge/Noir) et orientée vers une opportunité validée (Jaune). Le risque principal reste opérationnel (constituer le stock d'annonces — C1 et C2 des hypothèses de validation) plutôt que conceptuel. La validation terrain en S3 confirmera ou invalidera ce FIT.
