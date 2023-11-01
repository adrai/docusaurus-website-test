---
sidebar_position: 3
---

# Blog-Beitrag erstellen

Docusaurus erstellt eine **Seite für jeden Blogbeitrag**, aber auch eine **Blog-Indexseite**, ein **Tag-System**, einen **RSS**-Feed...

## Erstellen Sie Ihren ersten Beitrag

Erstellen Sie eine Datei unter `blog/2021-02-28-greetings.md`:

```md title="blog/2021-02-28-greetings.md"
---
slug: Grüße
title: Greetings!
Autoren:
  - Name: Joel Marcey
    Titel: Miterfinder von Docusaurus 1
    url: https://github.com/JoelMarcey
    bild_url: https://github.com/JoelMarcey.png
  - Name: Sébastien Lorber
    Titel: Docusaurus-Betreuer
    url: https://sebastienlorber.com
    bild_url: https://github.com/slorber.png
tags: [greetings]
---

Herzlichen Glückwunsch, du hast deinen ersten Beitrag verfasst!

Du kannst diesen Beitrag nach Herzenslust verändern und bearbeiten.
```

Ein neuer Blogeintrag ist jetzt verfügbar unter [http://localhost:3000/blog/greetings](http://localhost:3000/blog/greetings).