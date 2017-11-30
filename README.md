# hugo sites

## todo

Améliorer le markdown :
* remplacer les paragraphes par des sauts de lignes
* ajouter des infos au front matter exemple :
```bash
---
title: "Les Dojos"
description: "Les dojos sur Paris"
date: 2017-11-15T14:04:27+01:00
draft: false
private: true
tags: [ "dojo", "mugaikai", "Paris", "Kazuki", "adresse" ]
keywords: [ "dojo", "mugaikai", "Paris", "Kazuki", "adresse" ]
categories:
  - "dojo"
---
```

## contrib and deploy

```bash
git branch in-the-dimension

git checkout in-the-dimension
```
(don't forget to generate static content with **hugo**) 

```bash
git add <object>

git commit -m "something"

git push --set-upstream origin in-the-dimension
```

and on the system target

```bash
git clone -b in-the-dimension git@github.com:ronron22/hugo_sites.git
```
take the last commit number with 

```bash
git log
```

and copy public/* files on the target /var/www/<site>/<n° of commit>

create soft link like ln -s /var/www/<site>/<n° of commit> /var/www/<site>/current

that all ... 

#### le thème de base

```bash
cd themes 
 git clone https://github.com/sethmacleod/dimension.git
```

### Retaillage des images

```bash
convert Umegawa_in_Sagami_province.jpg -resize 300x200 Umegawa_in_Sagami_province-mini.jpg
```

# Jamstack

## API

### Mail

* https://formspree.io/
