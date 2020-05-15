# FAQ

## Qu'est-ce-qu'une enquête open source?
Il s'agit d'une enquête journalistique construite avec `git` de manière à être transparente et collaborative. Tous les ajouts à l'enquête sont publics et peuvent être suivis en temps réel par la communauté. 

Pour les ajouts nécessitants l'anonymat de la source:
  - Le contributeur peut lancer une PR anonyme, en utilisant cette fonction:
    ```https://github.com/PRB0t/PRB0t
    curl -X POST \
      https://xrbhog4g8g.execute-api.eu-west-2.amazonaws.com/prod/prb0t \
      -H 'cache-control: no-cache' \
      -H 'content-type: application/json' \
      -d '{
      "user": "PRB0t",
      "repo": "PRB0t",
      "description": "🤖",
      "title": "Dare to try",
      "commit": "a try",
      "files": [
      	{"path": "README.md", "content": "Failure is when you stop trying to do something."}
      ]
    }'
    # documentation: https://github.com/PRB0t/PRB0t
    ```
    
  - Lorsque le contributeur n'est pas à l'aise avec `git`, le journaliste publie les informations à la place de sa source.

Pour les ajouts d'information confidentielle, les contributeurs sont invités à chiffrer leur contribution avec la clé publique publiée à la racine de ce répertoire (`key.asc`). Les contributions sont publiées chiffrées, mais restent ouvertent aux commentaires.

## Mes données encryptées sont-elles totalement protégées?
Non. Une fois chiffrées avec la clé publique `key.asc` disponible à la racine de ce répertoire, vos informations deviennent très difficiles à lire pour quelqu'un qui ne dispose pas de la clé privée adéquate. Toutefois, avec de gros moyens, certains acteurs peuvent parvenir à décrypter vos informations. Si vos informations ne doivent **en aucun cas** fuiter, ne les publiez pas en ligne. Entrez en contact avec le journaliste en charge du dossier afin de déterminer la manière la plus adaptée de les protéger et de protéger votre identité.

## Qui dispose de la clé privée capable de décrypter mes données?
Le journaliste en charge du dossier, le rédacteur de l'agence TCA et sa directrice de publication disposent, tous les trois, d'une copie de la clé privée seule capable de déchiffrer les informations encryptées que vous ajouterez à l'enquête. Nous protégeons nos sources et maintiendrons vos informations à l'abri de toute altération.

## Qui est l'agence TCA?
L'agence est un organisme de presse référencée auprès de la Fédération française des agences de presse depuis plus de 20 ans.
Au coeur des nouvelles technologies depuis toujours, l'agence montre un intérêt très prononcé pour l'Open Source et souhaite
appliquer une déontologie stricte. 

## Puis-je forker cette enquête?
Oui. Vous pouvez également créer de nouvelles branches à notre version (que nous ajouterons au répertoire).

## A qui appartient cette enquête?
Cette enquête est publiée sous la licence GPLv3, à ce titre elle appartient à la communauté.
