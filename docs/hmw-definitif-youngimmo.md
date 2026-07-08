## HMW Définitif — GET409-YoungImmo

### HMW Draft S1

> « Comment pourrions-nous permettre aux étudiants dakarois à budget serré d'accéder à des annonces de logement vérifiées et à des prix transparents, afin qu'ils puissent se loger sans dépendre de démarcheurs opaques ? »

---

### 3 Versions Proposées

#### Version A — Axée sur le canal et la zone pilote

> « Comment pourrions-nous permettre aux étudiants dakarois à budget serré de trouver un logement vérifié dans la zone Fann / Point E via WhatsApp, afin qu'ils puissent contacter directement un propriétaire sans payer de commission à un démarcheur ? »

- **Plus précise car :** elle ancre le HMW dans un périmètre géographique concret (Fann / Point E) et un canal d'interaction spécifique (WhatsApp), ce que le draft S1 laissait ouvert. L'étudiant sait où et comment.
- **Risque Chapeau Noir intégré :** le cold start — en restreignant la zone à deux quartiers, on rend le stock d'annonces constituable avec les moyens de l'équipe, ce qui atténue le risque de plateforme vide.
- **Évaluation :** Légèrement trop précis — mentionner WhatsApp dans le HMW impose un canal technique avant l'idéation. Si le test utilisateur révèle qu'un site web simple suffit, le HMW devrait rester valide. Fixer le canal dans le HMW ferme des portes prématurément.

#### Version B — Axée sur la confiance et la traçabilité

> « Comment pourrions-nous aider les étudiants dakarois à budget serré à se loger en confiance, en leur donnant accès à des annonces vérifiées, des prix transparents et une traçabilité de leurs paiements de caution, sans dépendre d'intermédiaires opaques ? »

- **Plus précise car :** elle ajoute la dimension « traçabilité des paiements de caution » absente du draft S1, qui est le Gain Creator n°1 du VPC et la réponse directe au Pain émotionnel de méfiance (Chapeau Rouge). Le draft S1 ne parlait que d'annonces et de prix — celui-ci couvre aussi le moment critique du paiement.
- **Risque Chapeau Noir intégré :** la reproduction du modèle des démarcheurs — en mentionnant explicitement « sans dépendre d'intermédiaires opaques » et en ajoutant la traçabilité, le HMW signale que la gratuité et la transparence sont des engagements fondamentaux, pas des options.
- **Évaluation :** Légèrement trop large — elle cumule trois promesses (annonces vérifiées + prix transparents + traçabilité des paiements) dans un seul énoncé. Le risque est de disperser le MVP sur trois fronts alors que le backlog S3 montre que la traçabilité Wave est un SHOULD, pas un MUST.

#### Version C — Axée sur le problème terrain et le résultat concret

> « Comment pourrions-nous permettre aux étudiants dakarois à budget serré de trouver et visiter un logement vérifié dans les quartiers universitaires sans perdre de temps ni d'argent en déplacements inutiles, et sans payer de commission à un intermédiaire ? »

- **Plus précise car :** elle reformule le bénéfice en termes de résultat concret et mesurable (« sans perdre de temps ni d'argent en déplacements inutiles ») plutôt qu'en termes abstraits (« prix transparents »). C'est directement relié au Pain n°3 de la carte d'empathie (temps et argent perdus en visites) et à la Métrique Nord (mises en relation effectives = visites utiles).
- **Risque Chapeau Noir intégré :** le cold start et le sabotage — en parlant de « quartiers universitaires » plutôt que de « Dakar » entier, le HMW intègre la logique de zone pilote. En mentionnant « sans payer de commission », il pose un garde-fou contre la dérive du modèle économique.
- **Évaluation :** Bien calibré — assez précis pour guider le prototypage (zone universitaire, résultat concret, gratuité) sans imposer de solution technique. Il laisse l'équipe libre de choisir entre un site web, un bot WhatsApp ou un agent Dify pour y répondre.

---

### ✅ Version Recommandée

> « Comment pourrions-nous permettre aux étudiants dakarois à budget serré de trouver et visiter un logement vérifié dans les quartiers universitaires sans perdre de temps ni d'argent en déplacements inutiles, et sans payer de commission à un intermédiaire ? »

**Pourquoi :** La version C est la seule qui formule le bénéfice en termes de résultat mesurable sur le terrain (temps, argent, déplacements) plutôt qu'en concepts abstraits (transparence, confiance). Elle intègre les deux risques prioritaires du Chapeau Noir (cold start via la zone restreinte, modèle économique via la gratuité) sans imposer de canal technique. C'est le HMW le plus facile à tester en S3 : si Omar trouve un logement via YoungImmo en moins de visites qu'avant, le HMW est validé. Si non, il faut pivoter.
