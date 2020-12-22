---
name: Family Config
about: Add your clan family to the website
title: ''
labels: ''
assignees: ''

---

Consult https://github.com/RoyaleAPI/cr-api-ux/wiki/Family-Config for detailed description of all the fields. Here are some tips:

- `color`: should be all lower case
- `key`: will be used in the URL. Convention is to use all lower case
- `emblem`: do not include the file extension `.png`
- `description` and `links`: delete the lines if you have none
- `tag`:  do not include the `#` hash tag with the clan tags

Fill in the configuration below:

```yaml
name: Albiceleste
key: Albiceleste
color:blue
emblem: 
info:
  logo:https://dragon.img2go.com/download-file/e4a91d4d-864d-4689-87a5-006d295120af/279e2ca5-646a-45f7-87bb-a5c0f2cec323
  description: >
¡Más que un clan, una familia!
Top 4 Arg. en Wars I 
Aquí es donde les contendremos"! 
¡Aquí es donde nosotros pelearemos! 
¡Y aquí es donde ellos morirán!"

    Add new line with 2 line breaks as above.
  social:
    - twitter: http://twitter.com/albicelesteCR
    - discord: https://discord.gg/5Ayk65kWs9
    - twitch: https://www.twitch.tv/albicelestecr
    - facebook: https://facebook.com/albicelesteCR
clans:
  - name: Albiceleste
    tag: LL92RRP
  - name: Albiceleste II
    tag: YGP0GJCC
 
```
