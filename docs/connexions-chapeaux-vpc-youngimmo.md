## Connexions 6 Chapeaux → VPC — GET409-YoungImmo

### Profil Client — Origines

#### Jobs To Be Done

| Job | Chapeau d'origine | Citation exacte |
|---|---|---|
| Trouver un logement abordable à proximité des campus dans un marché où la demande dépasse l'offre | Chapeau Blanc | « Dakar compte plus de 80 000 étudiants… les résidences universitaires du COUD ne couvrent qu'une fraction de la demande » |
| Distinguer les annonces fiables des annonces frauduleuses | Chapeau Blanc | « groupes WhatsApp et pages Facebook sans aucune modération ni vérification. Il n'existe pas de plateforme locale dominante qui filtre les annonces frauduleuses » |
| Réunir et sécuriser la caution avec des revenus irréguliers | Chapeau Blanc | « 150 000 à 225 000 FCFA d'un coup — soit 2 à 4 mois de revenus d'un étudiant qui travaille à temps partiel » |

#### Pains

| Pain | Chapeau d'origine | Citation exacte |
|---|---|---|
| Méfiance généralisée : Omar s'attend à être trompé avant même de commencer | Chapeau Rouge | « la méfiance est devenue le sentiment dominant du marché locatif étudiant à Dakar » |
| Sentiment de ne pas être pris au sérieux en tant qu'étudiant sans fiche de paie | Chapeau Rouge | « frustration sourde… sentiment de ne pas être pris au sérieux dans sa propre ville parce qu'on n'a pas de fiche de paie » |
| Plateforme vide au lancement qui reproduit le problème | Chapeau Noir | « sans un stock initial d'annonces vérifiées, les premiers utilisateurs trouveront une application vide et ne reviendront pas » |
| Sabotage possible par les démarcheurs | Chapeau Noir | « les intermédiaires informels vivent de l'opacité… peuvent activement décourager les propriétaires ou publier de fausses annonces » |
| Toute commission facturée à Omar reproduit le modèle des démarcheurs | Chapeau Noir | « un modèle freemium ou à commission risque de reproduire exactement le problème qu'Omar dénonce » |

#### Gains

| Gain | Chapeau d'origine | Citation exacte |
|---|---|---|
| Tracer le paiement de la caution via Wave avec un reçu numérique | Chapeau Jaune | « la pénétration de Wave et Orange Money est massive… traçabilité des paiements de caution techniquement faisable aujourd'hui » |
| Les propriétaires reçoivent des contacts qualifiés rapidement | Chapeau Jaune | « un propriétaire qui publie une annonce vérifiée recevra des contacts qualifiés très vite — proposition de valeur immédiate côté offre » |
| Utiliser un service sur WhatsApp sans télécharger de nouvelle app | Chapeau Jaune | « un simple bot WhatsApp qui relaie des annonces vérifiées suffit comme MVP, WhatsApp est déjà le canal naturel d'Omar » |

---

### Proposition de Valeur — Origines

#### Produits & Services

| Produit / Service | Chapeau d'origine | Citation exacte |
|---|---|---|
| Caution certifiée Wave avec reçu numérique | Chapeau Vert | « Omar verse la caution sur un compte séquestre Wave intégré… reçu numérique et garantie de restitution » |
| Vérification communautaire des annonces par les anciens locataires | Chapeau Vert | « les anciens locataires peuvent laisser un avis vérifié… ce sont les utilisateurs eux-mêmes qui alimentent la confiance » |
| Agent IA de matching via WhatsApp (Dify) | Chapeau Vert | « chatbot WhatsApp construit en S3 sur Dify qui pose 3 questions à Omar et lui envoie les 3 annonces vérifiées les plus proches » |

#### Pain Relievers

| Pain Reliever | Pain adressé | Chapeau d'origine |
|---|---|---|
| Publication uniquement d'annonces vérifiées (prix, photos, disponibilité confirmés) — aucune publication libre | Méfiance généralisée (Rouge) + Plateforme vide (Noir) | Chapeau Noir — mitigation du cold start par stock vérifié manuellement |
| Zone pilote restreinte (Fann / Point E) + suivi qualitatif des propriétaires | Sabotage par les démarcheurs (Noir) | Chapeau Noir — mitigation par restriction géographique et monitoring |
| Accès 100% gratuit pour Omar — monétisation côté propriétaire uniquement | Commission qui reproduit le modèle des démarcheurs (Noir) | Chapeau Noir — mitigation par gratuité côté demande |

#### Gain Creators

| Gain Creator | Gain adressé | Chapeau d'origine |
|---|---|---|
| Reçu numérique Wave horodaté consultable par les deux parties | Traçabilité de la caution (Jaune) | Chapeau Jaune — « traçabilité techniquement faisable » |
| Lien WhatsApp direct vers le propriétaire vérifié, sans commission ni numéro masqué | Contacts qualifiés rapidement (Jaune) | Chapeau Jaune — « proposition de valeur immédiate côté offre » |
| Concentration sur Fann / Point E pour garantir un stock dense et à jour | Service sur canal habituel sans friction (Jaune) | Chapeau Bleu — « se concentrer sur un seul quartier pour constituer un stock suffisant » |

---

### Éléments Non Tracés

| Élément VPC | Statut | Action requise |
|---|---|---|
| Disposition réelle des propriétaires à publier directement (sans démarcheur) | Non tracé — déduit du Jaune mais jamais validé terrain | À valider en interview S3 : entretien avec 10 propriétaires zone Fann / Point E |
| Capacité réelle d'Omar à utiliser un chatbot WhatsApp (vs simple conversation humaine) | Non tracé — supposé à partir du Vert mais non testé | À valider en test utilisateur S3 : observer 5 étudiants interagir avec un prototype Dify |
| Acceptation par les propriétaires d'un forfait payant pour la visibilité | Non tracé — hypothèse secondaire S1 des hypothèses de validation | À valider après le MVP, hors périmètre S3 |

---

### Synthèse de Cohérence

**Alignement :** Fort — les 3 Jobs, les 5 Pains et les 3 Gains sont tous traçables à un Chapeau d'origine identifié. Les 3 Pain Relievers correspondent chacun à un Pain spécifique issu du Noir, et les 3 Gain Creators sont ancrés dans des opportunités du Jaune. Aucun élément du Canvas n'est orphelin.

**Tension principale :** Toute la proposition de valeur repose sur l'hypothèse que les propriétaires accepteront de publier directement — or cette hypothèse vient du Chapeau Jaune (optimisme) et n'a jamais été challengée par un fait terrain (Blanc) ni confirmée par une émotion captée en interview (Rouge). C'est le maillon non vérifié de la chaîne.

**Recommandation avant S3 :** Consacrer la première semaine de S3 à 10 entretiens avec des propriétaires de la zone Fann / Point E pour valider ou invalider l'hypothèse C1. Préparer une maquette visuelle de l'annonce type (screenshot ou prototype Bolt.new) à montrer pendant l'entretien pour rendre la proposition concrète. Si l'hypothèse est invalidée, pivoter vers un modèle de collaboration avec les démarcheurs existants plutôt que de contournement — et mettre à jour le VPC en conséquence.
