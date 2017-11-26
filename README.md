# hugo sites

## todo

Améliorer le markdown :
* remplacer les paragraphes par des sauts de lignes

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
