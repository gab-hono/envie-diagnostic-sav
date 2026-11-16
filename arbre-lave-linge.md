# Arbre d'aide au diagnostic SAV — Lave-linge (v1)

> Source de vérité du contenu. Tally n'est que l'interface.
> **Contenu technique à valider par les technicien·nes d'Envie.**
> Les numéros `p…` renvoient aux pages du formulaire Tally.

## Règles communes

- **Une question par écran**, réponses fermées.
- **« Le ou la client·e ne sait pas » → issue E**, sauf exceptions indiquées. L'appel n'est jamais bloqué.
- **Avant toute manipulation demandée au client·e : débrancher la machine.**
- **Pages de consigne (C)** : la consigne à lire, puis l'une de ces deux questions :
  - **« Résolu ? »** si le ou la client·e peut tester pendant l'appel ;
  - **« Consigne donnée / Déjà essayé »** si le test demande un lavage complet. « Consigne donnée » → B (il ou elle rappelle si ça persiste) ; « Déjà essayé » → vérification suivante.
- **Toute branche non résolue finit sur [G] (garantie).**

## Issues

| Code | Issue | Action de l'opérateur·rice |
|---|---|---|
| **A** | Urgence sécurité | Faire débrancher la machine, couper l'eau, ne plus l'utiliser. Escalade prioritaire. |
| **B** | Résolu au téléphone | Le ou la client·e rappelle si le problème revient. |
| **C** | Prise en charge sous garantie | Ouvrir une demande d'intervention / retour atelier. |
| **D** | Réparation sur devis | Proposer un devis (hors garantie). |
| **E** | Escalade technicien·ne | Transmettre à un·e technicien·ne référent·e. |

## Entrée

- **[S0] p1** — Y a-t-il une odeur de brûlé, de la fumée, des étincelles, ou de l'eau près d'une prise ? *(En cas de doute, répondre Oui. Pas d'option « ne sait pas » ici.)*
  - Oui → **A** · Non → p2
- **p2** — Quel est le problème ? → S1 (p3) · S2 (p11) · S3 (p15) · S4 (p19) · S5 (p25) · S6 (p30)

## S1 — La machine ne démarre pas

| Page | Contenu | Réponses |
|---|---|---|
| p3 | **[S1.1]** Le panneau s'allume-t-il (voyants, écran) ? | Oui → p5 · Non → p4 |
| p4 | C : vérifier que la prise est bien branchée ; tester la prise avec un autre appareil. Résolu ? | Oui → B · Non → G |
| p5 | **[S1.2]** Le hublot est-il bien fermé (on entend un clic) ? | Oui → p7 · Non → p6 |
| p6 | C : refermer le hublot fermement. Résolu ? | Oui → B · Non → p7 |
| p7 | **[S1.3]** Un symbole « cadenas / sécurité enfant » ou « départ différé » est-il affiché ? | Oui → p8 · Non → p9 |
| p8 | C : désactiver la sécurité enfant ou le départ différé (voir la notice). Résolu ? | Oui → B · Non → p9 |
| p9 | **[S1.4]** Le robinet d'arrivée d'eau est-il ouvert à fond ? | Oui → G · Non → p10 |
| p10 | C : ouvrir le robinet à fond. Résolu ? | Oui → B · Non → G |

## S2 — La lessive reste dans le bac

| Page | Contenu | Réponses |
|---|---|---|
| p11 | **[S2.1]** Le bac à produits est-il encrassé (dépôts, lessive durcie) ? | Oui → p12 · Non → p13 |
| p12 | C : sortir le bac, le nettoyer à l'eau chaude, nettoyer son logement. Résolu ? | Oui → B · Non → p13 |
| p13 | **[S2.2]** Le robinet est-il ouvert à fond et le tuyau d'arrivée sans pli ? | Oui → G · Non → p14 |
| p14 | C : ouvrir le robinet à fond, déplier le tuyau d'arrivée. Résolu ? | Oui → B · Non → G |

## S3 — De l'eau coule sous la machine

> Eau près d'une prise : déjà traité par [S0] → A.

| Page | Contenu | Réponses |
|---|---|---|
| p15 | **[S3.1]** La fuite apparaît-elle juste après un nettoyage du filtre de vidange ? | Oui → p16 · Non → p17 |
| p16 | C : revisser le filtre à fond ; remettre en place le petit tuyau de vidange d'urgence. Résolu ? | Oui → B · Non → p17 |
| p17 | **[S3.2]** Le tuyau de vidange est-il bien en place dans l'évacuation (pas sorti, pas percé) ? | Oui → G · Non → p18 |
| p18 | C : remettre le tuyau dans l'évacuation et le fixer. Résolu ? | Oui → B · Non → G |

## S4 — L'eau reste dans le tambour en fin de programme

| Page | Contenu | Réponses |
|---|---|---|
| p19 | **[S4.1]** Un programme sans essorage ou « arrêt cuve pleine » a-t-il été choisi ? | Oui → p20 · Non → p21 |
| p20 | C : lancer un programme « Vidange ». Résolu ? | Oui → B · Non → p21 |
| p21 | **[S4.2]** Le tuyau de vidange, derrière la machine, est-il plié, écrasé, ou trop enfoncé dans l'évacuation ? | Oui → p22 · Non → p23 |
| p22 | C : replacer le tuyau correctement. Résolu ? | Oui → B · Non → p23 |
| p23 | **[S4.3]** Le ou la client·e peut-il ou elle nettoyer le filtre de vidange (trappe en bas à l'avant) ? | Oui → p24 · Non → G |
| p24 | C : débrancher ; prévoir bassine et serpillières ; vider l'eau, retirer les objets (pièces, peluches), revisser à fond, relancer une vidange. Résolu ? | Oui → B · Non → G |

## S5 — Le linge sort sale ou avec des traces

> ⚠️ Branche la moins documentée : à valider en priorité.

| Page | Contenu | Réponses |
|---|---|---|
| p25 | **[S5.1]** Le tambour était-il rempli au maximum ? | Oui → p26 · Non → p27 |
| p26 | C : charger moins le tambour au prochain lavage. Consigne donnée / Déjà essayé | Donnée → B · Essayé → p27 |
| p27 | **[S5.2]** La lessive est-elle bien partie du bac ? | Oui → p28 · Non → **p11** (bascule sur S2) |
| p28 | **[S5.3]** Le linge a-t-il des traces grises ou grasses ? | Oui → p29 · Non → G |
| p29 | C : lancer un programme d'entretien à vide, à haute température. Consigne donnée / Déjà essayé | Donnée → B · Essayé → G |

## S6 — Bruit fort et vibrations à l'essorage

| Page | Contenu | Réponses |
|---|---|---|
| p30 | **[S6.1]** La machine a-t-elle été livrée ou installée il y a moins d'un mois ? | Oui → p31 · Non → p34 · **Ne sait pas → p31** (on vérifie les brides par précaution) |
| p31 | **[S6.2]** Y a-t-il encore des vis ou brides de transport à l'arrière de la machine ? | Oui → p32 · Non → p34 |
| p32 | **[S6.2b]** Le ou la client·e peut-il ou elle les retirer en suivant la notice ? | Oui → p33 · Non → **C** (installation) |
| p33 | C : arrêter tout essorage ; retirer les brides selon la notice, les conserver, boucher les trous avec les caches fournis. Consigne donnée | → B |
| p34 | **[S6.3]** La machine touche-t-elle un mur ou un meuble, ou bouge-t-elle sur ses pieds ? | Oui → p35 · Non → p36 |
| p35 | C : écarter la machine du mur, la mettre à niveau en réglant les pieds. Consigne donnée / Déjà essayé | Donnée → B · Essayé → p36 |
| p36 | **[S6.4]** Le linge était-il en boule, ou une seule grosse pièce (couette, tapis) ? | Oui → p37 · Non → G |
| p37 | C : répartir le linge ou ajouter des pièces pour équilibrer. Consigne donnée / Déjà essayé | Donnée → B · Essayé → G |

## [G] Nœud commun : garantie (p38)

- La machine a-t-elle été achetée chez Envie il y a moins de 2 ans ?
  - Oui → **C** · Non → **D** · Ne sait pas → **E**

> En production, cette information viendrait du logiciel Réemploi.

---

## Sources

- Vidange : [Haier](https://www.haier-europe.com/fr_FR/blogs/news/lave-linge-ne-vidange-plus), [Coolblue](https://www.coolblue.be/fr/conseils/le-lave-linge-nevacue-pas-eau.html), [electroguide](https://www.electroguide.com/?p=17994)
- Vibrations, brides de transport : [Siemens](https://www.siemens-home.bsh-group.com/ch/fr/service-consommateurs/centre-de-assistance/resolution-de-probleme/lave-linge/vibration), [Darty](https://www.darty.com/dossier/gros_electromenager/lavage_toutes_les_solutions_a_vos_questions.html)
- Bac à lessive : [Siemens](https://www.siemens-home.bsh-group.com/ch/fr/service-consommateurs/centre-de-assistance/resolution-de-probleme/lave-linge/detergent), [Miele](https://www.miele.fr/support/customer-assistance/lave_linge-579/toutes_les_categories/la_lessive_en_poudre_reste_dans_le_bac_a_produits-93001465611)
- Démarrage : [Darty SAV](https://sav.darty.com/thematic/MA-MACHINE-A-LAVER-NE-DEMARRE-PAS/76?p=77)
- Fuite : [Samsung](https://ushl.samsung.com/fr/support/home-appliances/que-faire-si-mon-lave-linge-fuit)
- Garantie et installation : [Selectra](https://selectra.info/energie/actualites/marche/lave-linge-vis-de-transport-oubliees-qui-paie)
