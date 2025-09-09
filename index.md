# La réforme des retraites est-elle équitable ?

![image_illustration_examen_depart_retraite](https://github.com/Peaceyearn/DEFI_M2_EXAM_Laiz-_Loucia_DATAVISUALISATION/assets/121464401/ea769c87-5805-4eba-98f0-97c1f309d6de)

> Source : [illustration_age_depart_retraite](https://www.ined.fr/fr/tout-savoir-population/jeux/l-esperance-de-vie/)
Réalisation : agence Gorille


La réforme des retraites révisant le système de retraite français réalisées pendant la mandature d'Emmanuel Macron, validée par le Conseil constitutionnel, le 14 avril 2023 et promulguée le jour même, a suscité de vives débats et des grèves violentes à travers tout le pays. Pourtant, la réforme a été présenté comme inéluctable par ses partisans. En effet, _« Nous vivons plus longtemps et donc (…) nous devons travailler plus longtemps »_, a déclaré le ministre du travail, Olivier Dussopt. Pourtant, beaucoup de France ont jugé cette réforme inique et convoyeuse d’inégalité. Nous chercherons à travers quelques visualisations à explorer de façon impartiale les angles des inégalités potentielles véhiculée par la réforme.


# Sommaire 
1. [Présentation des jeux de données](#1)
2. [L’espérance de vie de 30 à 80 ans selon le niveau d’éducation](#2) 
3. [L’âge de départs en retraite des catégories socioprofessionnelles](#3)
4. [Les groupes socioprofessionnels les plus touchés par les maladies](#4)
5. [Inégalité d’espérance de vie due au maladie chronique selon les catégories socioprofessionnelles](#5)

# Présentation des jeux de données <a name="1"></a>

▶ Le jeux de données n°1 :

Ce jeu de données porte sur l’espérance de vie de 30 à 90 ans selon le niveau d’éducation ou diplôme.J'ai effectué une modification en réconciliant les colonnes hommes et femmes. J'ai procédé au data cleaning en enlevant par années et les éléments de textes. Enfin, j'ai enlevé données avec un âge excédant les 80 ans puisqu'au delà, les écarts ne sont plus significatifs et tendent à se réduire.

> Sources : [Insee, Échantillon Démographique Permanent et état civil, 2009-2013.](https://www.insee.fr/fr/accueil)

> Source :[Jeux de données 1 modifie](https://github.com/Peaceyearn/DEFI_M2_EXAM_Laiz-_Loucia_DATAVISUALISATION/blob/main/Jeux_donn%C3%A9es_1_modifie_Esperance_Vie_par_diplome.xlsx)


> Source : [Jeux de données 1 original](https://github.com/Peaceyearn/DEFI_M2_EXAM_Laiz-_Loucia_DATAVISUALISATION/blob/main/Jeux_donn%C3%A9es_1_original_Esperance_Vie_par_diplome.xlsx)

▶ Le jeux de données n°2 :  
Ce jeu de données porte sur l’âge conjoncturel de départs en retraite des catégories socioprofessionnelles par année, sexe et régime. J'ai enleve les données au dessus de 2009 et excédant 2013 car le jeux de données précédent à la même date et est lié. Puis j'ai enlevé les catégories CC et sexe qui ne m'intéressaient pas ainsi que des catégories comme la CNAV puisque tout le monde cautise à la CNAV donc ce n‘est pas vraiment représentatif et aussi car certaines données étaient incomplètes au niveau des dates. Enfin j'ai fait la moyenne par catégories de 2009 à 2013 pour chaque catégorie (CNIEG) sur Excel avec la fonction calcul de moyennnes sur excel.


| Caisse       | Ensemble     |
|--------------|--------------|
| Banque de France | 59,3     |
| CNIEG        | 57,02        |
| CNRACL       | 61,3         |
| CRPCEN       | 62,5         |
| ERAPF        | 65,325       |

> Source : [Insee, Échantillon Démographique Permanent et état civil, 2009-2013.](https://www.insee.fr/fr/accueil) 

> Source : [Jeux de données 2 modifie](https://github.com/Peaceyearn/DEFI_M2_EXAM_Laiz-_Loucia_DATAVISUALISATION/blob/main/Jeux_donn%C3%A9es_2_Caisse_retraite_age_depart_ensemble__Ageconj.csv)

> Source :[Jeux de données 2 original](https://github.com/Peaceyearn/DEFI_M2_EXAM_Laiz-_Loucia_DATAVISUALISATION/blob/main/Jeux_donn%C3%A9es_2_original_Donn%C3%A9es_caisses%20_de_retraite.xlsx)
> 
> Source [Envoi We transfer](https://we.tl/t-WmOFoi8yZl)

▶ Le jeux de données n°3 :
Ce jeu de données porte sur les groupes de catégories socio-professionnels  ("_Agriculteurs exploitants_","_Artisans_", "_commerçants_", "_chefs d'entreprise_", qui sont le plus touchés par les maladies comme le "_Cancers_", "_Diabète_"... avec comme référent de 1 la catégorie _les cadres et professions intellectuelles supérieures_.J'ai enlevé les éléments de textes superflus por le traitement et j'ai les nombres en desssous de chaque case dans les colonnes principales de catégories car elles faisaient trop de valeurs à traiter pour l’outil et je les ai remis au propre.

> Source :  [data.drees.solodarities-sante.gouv.fr](https://data.drees.solodarities-sante.gouv.fr/explore/dataset/er_inegalites_maladies_chroniques/information/) 

> Source :  [Jeux de données 3 modifie](https://github.com/Peaceyearn/DEFI_M2_EXAM_Laiz-_Loucia_DATAVISUALISATION/blob/main/Jeux_donn%C3%A9es_3_A_maladies_chroniques_groupe_socioprofessionnel.xlsx)

> Source :[Jeux de données 3 original](https://github.com/Peaceyearn/DEFI_M2_EXAM_Laiz-_Loucia_DATAVISUALISATION/blob/main/Jeux_donn%C3%A9es_3_original_maladies_chroniques_et_esp%C3%A9rance_de_vie.xlsx)



▶ Le jeux de données n°4 :

Ce jeu de données porte sur les inégalité d’espérance de vie due au maladie chronique selon les catégories socioprofessionnelles. Il comporte des colonnes _"Categorie_",	"_Dixieme de niveau de vie_",	"_Sante"Esperance de vie_" avec des données sur la "_Population sans la maladie_" et des données sur les types de maladies_"_Diabète_", "_Maladies du foie ou du pancréas_". J'ai enlevé le reste des données "_toutes catégories confondues_" après la ligne "_Maladies du foie ou du pancréas" car les données semblaient erronnées, elles se répétaient.Etant donné que le but était de montrer les écarts entre chaque groupe de 1 à 6 pour chaque catégorie de maladies_, les données précédentes portant sur la population sans la maladie qui semblaient juste, suffisaient à montrer les écarts entre les groupes sociaux bien que des données de population avec les maladies aurait été préférables. Hormis ces erreurs remarquées le dossier n'a pas nécessité de datacleaning hormis le fait d'enlever les données textuelles.

> Source :  [data.drees.solodarities-sante.gouv.fr](https://data.drees.solodarities-sante.gouv.fr/explore/dataset/er_inegalites_maladies_chroniques/information/) 

> Source : [Jeux de données 4 modifie](https://github.com/Peaceyearn/DEFI_M2_EXAM_Laiz-_Loucia_DATAVISUALISATION/blob/main/Jeux_donn%C3%A9es_3_B_inegalite_esperance_vie_due_maladie_chronique.xlsx)

> Source :[Jeux de données 3 original](https://github.com/Peaceyearn/DEFI_M2_EXAM_Laiz-_Loucia_DATAVISUALISATION/blob/main/Jeux_donn%C3%A9es_3_original_maladies_chroniques_et_esp%C3%A9rance_de_vie.xlsx)

## L’espérance de vie de 30 à 80 ans selon le niveau d’éducation <a name="2"></a>
Notre premier jeu de données traite de l’espérance de vie selon les diplômes couvrant la période de 2009 à 2013, et les années de 30 à 80 ans.Cette visualisation vise à illustrer la différence d’espérance de vie selon les diplômes (_sans diplôme_, _Brevet_, _CAP-BEP_, _Baccalauréat_, _Supérieur_). Il s’agit pour nous de montrer avec cette visualisation qu’il existe à déjà une inégalité basée sur l’éducation qui influe sur l’espérance de vie des personnes et que la réforme des retraites pourrait potentiellement renforcer cette inégalité en rallongeant la durée de travail de personne défavorisé alors que leur espérance de vie est moindre en comparaison avec les personnes des classes supérieure.

<div class="flourish-embed flourish-chart" data-src="visualisation/16619337"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

> Source :[Outil Florish](https://flourish.studio/) 


Ab initio, nous observons un écart encore plus grand entre les hommes et les femmes, lorsque celles-ci sont plus diplômées sachant qu’en moyenne les femmes ont à l’origine une espérance de vie plus haute que les hommes (pour diverses raisons hormonales, sociétales…).En outre, le même phénomène entre les femmes est observable. Par exemple, une femme sans diplôme à 30 ans aura une espérance de vie de 52.9 quand une femme dans le supérieur aura une espérance de vie de 57.1. L’écart est de 4,2 ans. Cet écart d’espérance de vie selon les diplômes se retrouve dans toutes les catégories et se poursuit dans les tranches d’âges de 30 à 53 ans (puis tend à se réduire).Cet écart d’espérance de vie due au niveau d’éducation est encore plus marqué chez les hommes. Un homme sans diplôme a une espérance de vie de 45,4 ans à 30 ans, une espérance de vie de 40 ans à 36 ans et une espérance de vie de 34, 6 à 42 ans.A contrario, un homme avec un Brevet a une espérance de vie de 48,4 ans à 30 ans, une espérance de vie de 42,8 ans à 36 ans et une espérance de 37, 2 à 42 ans. Enfin, un homme dans le supérieur à une espérance de vie de 49,4 ans à 30 ans, une espérance de vie de 43,7 ans à 36 ans et une espérance de 38, 1 à 42 ans. On constate donc un bond de 3 points à l’âge de 30 entre un homme ayant un simplet brevet et un homme diplômé ce qui est plus que pour les femmes.


Enfin, nous constatons une tendance selon les genres : 
A partir de 70 ans pour les femmes, l’écart d’espérance de vie diminue sensiblement, il n’est plus « que » de 2 ans au lieu de 4 ans à l’âge de 30, et à partir de 80, il n’est plus que de 1 an.
Pour les hommes, l’écart d’espérance de vie est encore plus important à 30 ans, il est de 8 ans. 
A partir de 70 ans pour les hommes, l’écart d’espérance de vie diminue sensiblement, il n’est plus « que » de 3 ans au lieu de 8 ans à l’âge de 30, et à partir de 80, il n’est plus que de 1 an comme les femmes.
Nous concluons d’après ces données que l’espérance de vie est indéniablement liée au niveau d’éducation car des études ont montrées que plus le niveau d’éducation est élevée plus grande est la sensibilisation à la qualité de vie. Et donc l’impact sur l’espérance de vie est plus conséquent.Suivant cette visualisation, il paraît alors juste de se demander, dans le cas où l’espérance de vie est asymmétrique selon le niveau d’éducation, est-elle prise en compte dans le temps de travail et le droit de prendre sa retraite prématurément et d’échapper au prolongement de la durée de travail prévue par la loi récemment passée ?


## L’âge de départs en retraite des catégories socioprofessionnelles(#age-de-departs-retraite) <a name="3"></a>

Ces données représentent l'âge de départ à la retraite pour différents régimes de retraite ou caisses en France de 2009 à 2013… Ces données de caisses de retraites permettent de faire une visualisation rendant compte de l’âge de départ des catégories socioprofessionnelles. Chaque chart indique le nom de la caisse et l'âge de départ à la retraite présumé ou conjecturel associé. L'âge de départ à la retraite peut varier en fonction de la caisse et des spécificités du régime de retraite associé.

<iframe title="Age conjoncturel de départ à la retraite" aria-label="Stacked Bars" id="datawrapper-chart-F5xE6" src="https://datawrapper.dwcdn.net/F5xE6/1/" scrolling="no" frameborder="0" style="border: none;" width="600" height="510" data-external="1"></iframe>

Le régime des caisses de retraites donne les modalités selon lesquelles les prestations de retraite sont gérées et distribuées par une caisse de retraite spécifique. En France, il existe plusieurs caisses de retraite, chacune gérant les pensions de retraite pour des catégories spécifiques de travailleurs ou de secteurs d'activité. 

- ERAPF = retraite additionnelle de la fonction publique
- CRPCEN = clercs et employés de notaire
- AGIRC = la quasi-totalité des salariés de l’industrie, du commerce, des services de l’agriculture
- ARCCO = cadres
- CNRACL = retraite des fonctionnaires territoriaux et hospitaliers
- SSI = sécurité des sociales des indépendants
- FSPOEIE = retraite des ouvriers d’état
- Banque de France = travailleurs du secteur privé.
- CAVIMAC = ministres des cultes et des membres des congrégations et des collectivités religieuses
- CNIEG = caisse nationale des industries gazières et électriques
- RATP / SNCF = deux grandes entreprises de transport en France

Nous observons que les _CRPCEN_ (clercs et employés de notaire) partent à la retraite à 62 ans et que les travailleurs des grandes entreprises de transport en France (RATP, SNCF) partent à la retraite à 55 ans grâce aux régimes de retraite spéciaux avec des caisses dédiées. Le départ à la retraire n’est pas le même selon les catégories socioprofessionnelles.Or, l’article 1 de la réforme des retraites prévoit la suppression de la majorité des régimes spéciaux de retraite. Cela comprend la RATP, la branche des industries électriques et gazières (IEG), les clercs et employés de notaires, les personnels de la Banque de France, et les membres du Conseil économique social et environnemental (Cese). 



## Les groupes socioprofessionnels les plus touchés par les maladies (#groupes-plus-touches-maladies) <a name="4"></a>
Cette visualisation permet de rendre compte de la rareté des maladies chez les cadres et professions intellectuelles supérieures et de leur prévalence chez les autres professions :_Agriculteurs exploitants_, _Artisans_, _commercants_.

<div class="flourish-embed flourish-chart" data-src="visualisation/16636184"><script src="https://public.flourish.studio/resources/embed.js"></script></div>
> Source :[Outil Florish](https://flourish.studio/) 

Dans le jeu de données, les cadres servent de points de référence, fixé à 1. Les autres professions dépassent largement ce point de référence, elles sont plus touchées par le diabète, les maladies chroniques... .Par exemple, les ouvriers ont 1,88 % plus de chances d'avoir du diabète que les cadres et professions supérieurs qui sont la valeur de référence. Les maladies chroniques accentuent les inegalites societales en matière d'espérance de vie entre les plus aisés et les plus modestes. Les maladies qui creusent le plus les inegalités d'après la visualisation sont les maladies psychatriques et cardiaoneurovasculaires.


## 5. Inégalité d’espérance de vie due au maladie chronique selon les catégories socioprofessionnelles <a name="5"></a>

Ce jeu de données porte sur les inégalité d’espérance de vie due au maladie chronique selon les catégories socioprofessionnelles et couvre les années 2016 à 2017.
La visualisation a 2 variables affichées : "_Dixieme de niveau de vie_" et "_Esperance de vie_". .Le dixième de niveau de vie correspond dans le jeux de données en dix groupes(chaque groupe allant de 1 à 6) en fonction du niveau de vie. Une espérance de vie à été associé une espérance de vie. Les types de catégories ne sont pas détaillées dans le jeux de données.Le chiffre de 1 représente le 1er décile et donc correspond au 10 % des ménages les plus modestes qui ont un revenu disponible inférieur aux 13 630 euro par an et les 10 % de ménages les plus aisés ont un revenu supérieur à 63 000 euros dans le 9 ème décile.A Gauche de chaque barre de variables, se trouve des types de maladies (Diabètes, Maladies du foie ou du pancréas...) 

<iframe title="Inégalité d’espérance de vie due au maladie chronique selon les catégories socioprofessionnelles" aria-label="Grouped Bars" id="datawrapper-chart-5sreo" src="https://datawrapper.dwcdn.net/5sreo/1/" scrolling="no" frameborder="0" style="width: 0; min-width: 100% !important; border: none;" height="4650" data-external="1"></iframe><script type="text/javascript">!function(){"use strict";window.addEventListener("message",(function(a){if(void 0!==a.data["datawrapper-height"]){var e=document.querySelectorAll("iframe");for(var t in a.data["datawrapper-height"])for(var r=0;r<e.length;r++)if(e[r].contentWindow===a.source){var i=a.data["datawrapper-height"][t]+"px";e[r].style.height=i}}}))}();
</script>
> Source : [Outil datawrapper](https://datawrapper.dwcdn.net/) 

Prenons par exemple la catégorie "Cancers", si l'on compare les valeurs entre le premier et le dernier dixième de niveau de vie, le premier dixième, 1, a une espérance de vie de 83,20 alors que le dernier dixième a une espérance de vie de 88,87. L'écart entre ces 2 groupes d'individus est de 5,67.Cela signifie que, en termes d'espérance de vie sans cancer, la population du dixième de niveau de vie le plus élevé (10) a une valeur plus élevée de 5,67 par rapport à la population du dixième de niveau de vie correspondant au chiffre 1. En d'autres termes, les personnes du dixième de niveau de vie le plus élevé ont une espérance de vie sans cancer plus élevée que celles du dixième le plus bas, et l'écart est de 5,67 ans.
Cette visualisation montre que la réforme dessert les plus défavorisés qui travailleront plus longtemps alors qu'ils auront une espérance de vie plus réduite et sont plus touchés par les maladies chroniques comme nous l'avons vu précédemment.Par exemple, dans la catégorie "Cancers", le dixième groupe de niveau de vie a une espérance de vie de 88,87 ans pour une population sans la maladie, tandis que le premier groupe a une espérance de vie de 83,20 ans dans des conditions similaires.

# Conclusion

Nous gardons en tête que le traitement d'un sujet aussi vaste est complexe est limité car il croise plusieurs domaines, économiques, sociale  et politique . Trop de facteurs sont à prendre en compte pour affirmer avec certitude que cette réforme impopulaire est inégalitaire à tous les égards. Il aurait fallu prendre en compte les taux de cotisations en compte et le taux de pénibilité et d'autres facteurs économiques pour réaliser des croissements entre les données. Cela aurait requis de croiser des données et nécessité une compréhension plus poussée des statistiques.De plus, certains de jeux de données liées à la santé étaient complexes et difficiles à croiser avec des données socio-économiques, ils auraient fallu par exemple comprendre comment chaque groupe et les détails ou les descriptions spécifiques associées à chaque groupe dans la source d'origine des données.Ces détails auraient pu inclure des informations sur les caractéristiques socio-économiques, les comportements liés à la santé, ou d'autres facteurs qui pourraient influencer la santé dans chaque groupe. En définitive il aurait fallu réaliser un étude qui dépasse le cadre de cet examen pour croiser tous les facteurs. 

Ainsi, mon approche s'est focalisée sur l'espérance de vie qui n'est pas pris en compte dans la réforme des retraites. Mon choix à été de sélectionner l'espérance de vie par revenu et non pas par diplôme puisque le niveau d’éducation a une plus grande influence sur les individus, sur leur espérance de vie en influyant sur leur niveau de vie. Nous avons simplement observées des corrélations. Ainsi, les jeux de données ont permis de montrer que la réforme des retraites est défavorable aux plus pauvres qui sont toujours les plus touchés au niveau de l'espérance vie, à cause du niveau d'éducation et du point de vue des maladies. Nous avons montré que l'âge de départ à la retraire avec la fin des régimes spéciaux mets à égalités des individus qui ont une espérance de vie plus courte et sont plus sujets. 


Les visualisations effectuées amènent donc légitimement se poser la question suivante :  la réforme des retraites agrandira dans les années à venir les inégalités socioéconomique existantes ?

> Sources :
-[Lois réforme des retraites - wikipédia](https://fr.wikipedia.org/wiki/R%C3%A9forme_des_retraites_en_France_en_2023)
-[Réforme des retraites](https://www.service-public.fr/particuliers/actualites/A16717)
-[Réforme des retraites :](https://demarchesadministratives.fr/guides/tout-comprendre-sur-la-reforme-des-retraites-et-ses-consequences) 

