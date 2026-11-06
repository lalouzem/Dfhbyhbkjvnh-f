# Sources et vérifications — 6 novembre 2026 (version des règles 2026-11-06.2)

Chaque règle a été contrôlée par recherche web le 6 novembre 2026. Une règle non confirmée a été **exclue**.

| Situation | Règle retenue | Sources consultées |
|---|---|---|
| Achat à distance (bien) | 14 jours calendaires ; départ le lendemain de la réception ; report au premier jour ouvrable si le dernier jour est un samedi, dimanche, férié ou chômé | Service-Public F10485, Justice.fr (mis à jour le 01/01/2026), Économie.gouv.fr (écrit le 19/06/2026), fiches de médiation |
| Achat à distance (service) | 14 jours à compter de la conclusion du contrat | Économie.gouv.fr (19/06/2026) |
| Crédit à la consommation | 14 jours calendaires révolus à compter du jour de l'acceptation de l'offre (C. conso. L312-19, L312-20) ; report non confirmé → non appliqué | Texte de L312-19 cité par la Cour de cassation (Civ. 1re, 19 juin 2024, n° 22-10.300), documents de l'Assemblée nationale ; pas de fiche Service-Public directe vérifiée |
| Amende forfaitaire | Minoré : 15 j (30 j télépaiement CB si avis envoyé) ; normal : 45 j (60 j télépaiement CB) ; contestation : 45 j | Service-Public F18509 (vérifiée par ses rédacteurs le 11/01/2025) |
| Amende majorée | Contestation : 30 j (3 mois si recommandé) ; paiement avec −20 % : 30 j (45 j télépaiement CB) | Service-Public F18509 |
| Préavis du locataire | Vide 3 mois ; vide en zone tendue ou motif légal 1 mois (motif à indiquer dans la lettre, sinon 3 mois) ; meublé 1 mois ; point de départ = jour où le bailleur prend possession de la lettre ; date à date, sans report | **Service-Public F1168 (vérifiée par ses rédacteurs le 16 avril 2026)** ; loi du 6 juillet 1989, art. 15 et 25-8 |
| Dépôt de garantie | 1 mois (état des lieux conforme) ou 2 mois, à compter de la remise des clés ; pénalité 10 % du loyer par mois de retard commencé | Service-Public F31269 (contenu relu via sa reprise par des sites d'information publique) ; loi du 6 juillet 1989, art. 22 ; Assemblée nationale |
| Solde de tout compte | 6 mois à compter de la signature ; la dénonciation doit parvenir à l'employeur dans le délai | Code du travail L1234-20 ; Cass. soc. 7 mars 2018, n° 16-13.194 ; Éditions Tissot, CFDT |
| Contestation du licenciement | 12 mois à compter de la notification (L1471-1) ; exceptions listées | Fiches DREETS, avocats, Légisocial |
| Recours administratif | 2 mois à compter de la notification ou publication (CJA R421-1) ; **date affichée = la plus proche possible** (date à date) ; recours administratif prolonge ; silence 2 mois = rejet ; R421-5 | Service-Public F2474, décisions de tribunaux administratifs 2025-2026 ; sources divergentes sur le « délai franc » |
| Feuille de soins papier | Fin du trimestre civil, 2 ans plus tard (maladie) ; ex. soin le 23/04/2025 → 30/06/2027 | Service-Public / Justice.fr (mis à jour le 23/04/2025), forum officiel Ameli |

## Écarts avec la base de départ proposée (ChatGPT)
- **Amendes** : base incomplète. Ajoutés : tarif minoré, contestation (45 j), amende majorée (30 j / 3 mois).
- **Rétractation** : ajout du point de départ « lendemain » et de la réforme du 19 juin 2026 (fonction de rétractation ; prolongation jusqu'à 12 mois + 14 jours sans information).
- **Feuille de soins** : résultat identique, mais l'article cité (L332-1) est contesté par une source secondaire, qui cite L160-11 ; **article non repris** dans le site.
- **Solde de tout compte** : ajout de la règle « lettre reçue dans les 6 mois ».
- **Exclus faute de vérification** : assurance-vie (30 j) ; délai de renvoi du bien après rétractation (14 j).

## Limites assumées
- Jours fériés métropolitains uniquement (pas d'Alsace-Moselle, pas d'outre-mer).
- Report au jour ouvrable appliqué **uniquement** à la rétractation achat à distance, seule règle où il est confirmé.
- Dates de départ à saisir par l'utilisateur ; le site ne juge pas laquelle est juridiquement la bonne dans les cas ambigus.

## Relecture croisée (ChatGPT) : ce qui a été retenu ou écarté
| Remarque | Décision |
|---|---|
| Recours administratif : « délai franc » à calculer | **Partiellement retenue.** Les sources consultées divergent (certaines parlent de délai franc, d'autres de date à date). Plutôt que trancher, le site affiche la date la plus proche possible, avec la mention « date prudente ». Jamais une date plus tardive que la plus sûre. |
| Crédit à la consommation : retirer le calcul | **Écartée après vérification** : le texte de L312-19 (14 jours calendaires révolus à compter du jour de l'acceptation) est confirmé. Report toujours non appliqué. |
| Export .ics : repliement des lignes | **Retenue et corrigée** : repliement en octets UTF-8 (75 max), sans couper un caractère. Validé par l'analyseur Python `icalendar` (2 événements, 3 alarmes, UTF-8 valide). **Non testé** : import réel dans Apple Calendrier, Google Agenda et Outlook. |
| Liens directs vers des fiches | **Retenue en partie** : liens directs pour les fiches dont l'identifiant a été vérifié (F10485, F18509, F2474, F1168, F31269, Justice.fr). Trois situations (crédit, solde de tout compte, licenciement) gardent un lien de recherche Service-Public, un lien direct non vérifié étant pire. |
| Poser les questions déterminantes avant de calculer | **Retenue** : aucun cas n'est présélectionné, aucun résultat n'apparaît tant que le cas n'est pas choisi. |
| Version des règles, date de vérification, alerte hors ligne | **Retenue** : version et date affichées, bandeau hors ligne, bandeau d'alerte automatique si les règles ont plus de 90 jours. |

## Erreur trouvée pendant la relecture
La fiche officielle F1168 (préavis) indique que, pour une lettre recommandée, le préavis part du jour où le destinataire **prend possession** de la lettre. La première version du site disait « réception ou première présentation » : **corrigé**, avec ajout du motif à indiquer dans la lettre pour obtenir 1 mois.
