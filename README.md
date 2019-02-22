If you would like your clan family to be listed at [https://royaleapi.com/clans](https://royaleapi.com/clans) and [https://royaleapi.com/clans/families](https://royaleapi.com/clans/families), you will need to send us your clan configuration in [YAML](https://en.wikipedia.org/wiki/YAML). Read this guide thoroughly on how to configure it and then [open a new issue](https://github.com/RoyaleAPI/family-config/issues/new?template=family_config.md) with your configuration.

Please remember to escape your config as shown below with the three backticks when including it in your issue. First to open it with the three back ticks followed by the language `yaml`, and then to close it at the end.

````
```yaml
name: Name of the Family
key: URL shortname
color: red
emblem: A_Char_Rocket_02
…
```

````

## Fields

This table shows what all those fields mean

| Field | Description |
| --- | --- |
| name | Name of the family. |
| key | Shortcut name. Used in the URL path. |
| color | Brand color. See below for acceptable colors. HEX is not supported yet, so use the closest match. |
| emblem | Clan Badge. Find it from your clan page or look up in [RoyaleAPI/cr-api-assets/badges](https://github.com/RoyaleAPI/cr-api-assets/tree/master/badges) |
| info | Optional information. Used in clans page. |
| clans | Names and tags of your clans. |
| sort | Sort order of the clans. Don’t include this field if you wish the clans be sorted according to the order in the `clans` field. Use `sort: trophy` if you want the clans to be sorted according to the clan score. |

### Info fields

| Field | Description |
| --- | --- |
| logo | Please provide URL to your logo and we will upload it. |
| description | Family description in markdown. Please be brief as it will push all your clans down if it is too long. |
| social | Links to social media sites. |

### Social Links

You may order these in any order. The site will display them according to the order that you have entered in your configuration.

- application: url
- discord: url
- email: mailto_url
- facebook: url
- instagram: url
- twitch: url
- twitter: url
- website: url
- youtube: url

### Clans

| Field | Description |
| --- | --- |
| name | Name of the clan |
| tag | Clan tag without the `#` symbol |


## Colors

![Colors](https://raw.githubusercontent.com/RoyaleAPI/cr-api-docs/master/docs/img/colors.png)

## Examples

### RoyaleAPI Clan Family

https://royaleapi.com/clan/family/royaleapi

[royaleapi.yml](https://github.com/RoyaleAPI/family-config/blob/master/examples/family_config/royaleapi.yml)

```yaml
name: RoyaleAPI Clan Family
key: royaleapi
color: blue
emblem: Sword_02
info:
  logo: /static/img/branding/cr-api-logo.png
  description: >
    The **RoyaleAPI Clan Family** (RACF) was originally known as the Reddit Alpha Clan Family and then briefly as the 100 Thieves Clan Family. Home to professional players that eventually moved on to play at CRNAO, King’s Cup, and CRL, our family fosters an environment where casual and competitive styles of play can both flourish.
  social:
    - twitter: https://twitter.com/RoyaleAPI
    - discord: https://discord.royaleapi.com
    - website: https://fam.royaleapi.com
clans:
  - name: RoyaleAPI Alpha
    tag: 9PJ82CRC
  - name: RoyaleAPI Bravo
    tag: 9UQJUJC9
  - name: RoyaleAPI Coca
    tag: 9G99JQPL
  - name: RoyaleAPI Delta
    tag: 9G8VYGL0
  - name: RoyaleAPI Echo
    tag: 9CJ0L9RG
  - name: RoyaleAPI Zen
    tag: 9LPVG9UC
  - name: RoyaleAPI
    tag: 9R8G9290
```

### LeGeND Family

https://royaleapi.com/clan/family/legend

[legend.yml](https://github.com/RoyaleAPI/family-config/blob/master/examples/family_config/legend.yml)

```yaml
name: LeGeND Family
key: legend
color: yellow
emblem: Flame_03
info:
  logo: /static/img/brands/logo/legend.png
  description: >
    The Legend family is one of the oldest and biggest families in Clash Royale
    with our 700 members and 14 clans!
    Since creation, we as a family and individual players have grown immensely
    and continue to today.
    We believe that’s the reason why we have come so far.
    **The family is a place for everyone, as our members come from all around the world,
    from casual to competitive players, old to young,
    active to very active and so on.**
    We all share a fellow passion for the game, are friendly, always donate,
    help each other out with the same goal: to always improve our skills and have a great time!
    **Join the Family. Become a Legend. **
  social:
    - discord: https://discord.me/legendfamily
    - website: https://legendclans.com
    - twitter: https://twitter.com/TheLegendClans
    - facebook: https://www.facebook.com/LegendClans
    - instagram: https://www.instagram.com/legendclans
    - youtube: https://www.youtube.com/channel/UCU-_xxoQeJlXx1kJcH1CoBQ
    - reddit: https://www.reddit.com/user/LegendClans
    - email: mailto:board@legendclans.com
clans:
  - name: Dragons Eight
    tag: 29YPJYY
  - name: LeGeND eSports!
    tag: 2GJYVRYQ
  - name: LeGeND Squad!
    tag: 80CC8
  - name: Dragons Eight 2
    tag: Y8G9C09
  - name: LeGeND Prime!
    tag: 2LL8LC2R
  - name: LeGeND Titan!
    tag: 9PJYVVL2
  - name: LeGeND Legion!
    tag: VJQ0GJ0
  - name: LeGeND Rising!
    tag: RY9QJU2
  - name: LeGeND Dynasty!
    tag: 99R2PQVR
  - name: LeGeND Phantom!
    tag: 2CJ88808
  - name: LeGeND Empire!
    tag: 9P2PQULQ
  - name: White Plague
    tag: J0CQ9R9
  - name: Dragons Eight 3
    tag: 2ULY20LU
  - name: LeGeND Academy!
    tag: 8QRQQ8RG
```

### Nova eSports

https://royaleapi.com/clan/family/nova

[nova.yml](https://github.com/RoyaleAPI/family-config/blob/master/examples/family_config/nova.yml)

```yaml
name: Nova eSports
key: nova
color: purple
emblem: Star_Shine_03
sort: trophy
info:
  logo: /static/img/brands/logo/nova.svg
  description: >
    **Competitive excellence through community-driven values.**
    Nova is a mobile-focused eSports organization committed to empowering
    individuals through a supportive team environment.
    We look for talent that has the character to back it up.
    That talent is cultivated and supported through team-based growth strategies and
    passionate staff that care about player outcomes.
    Community is the foundation of those outcomes and is the core of player dedication.
  social:
    - website: https://novaesports.com/
    - twitter: https://twitter.com/NovaeSportsTeam
    - instagram: https://instagram.com/novaesportsgg
    - facebook: https://facebook.com/OfficialNovaeSports
    - twitch: https://twitch.tv/NovaeSportsGG
    - youtube: https://www.youtube.com/channel/UC4JS5NiRp4Sy1wl6qFkW3GQ
    - application: https://novaesports.com/apply
    - email: mailto:pr@novaesports.com
clans:
  - name: Nova eSports
    tag: LCVUYCR
  - name: Nova I ARG
    tag: 8QC8YQJC
  - name: Nova l Brazil
    tag: JVRPGV8
  - name: Nova I C.A
    tag: 8JLVR9VV
  - name: Nova l Canada
    tag: 8PLYP8V
  - name: Nova l EG
    tag: 8YLJ8UL2
  - name: Nova FrenchArmy
    tag: 8VG2C9CJ
  - name: Nova l Hispania
    tag: 2CQQVQCU
  - name: HK@852 l Nova
    tag: 8JQQP8UL
  - name: Nova l India
    tag: 8GGC990V
  - name: Nova I Iran
    tag: 8YGRJ8GG
  - name: Nova I Korea
    tag: 92LLJ828
  - name: Nova l JPN
    tag: 2GYJL2GQ
  - name: Nova l MANGÚ™
    tag: 8JQP02QQ
  - name: Nova l Potenza
    tag: 2UP8R99Y
  - name: Nova l Raze
    tag: 8UY0CPU2
  - name: Nova l Swiss
    tag: 8RR89PUY
  - name: Nova Turkey
    tag: CYCJJLG
  - name: Nova l 大唐天子
    tag: RVL2PQQ
```
