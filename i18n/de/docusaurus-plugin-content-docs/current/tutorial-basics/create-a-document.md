---
sidebar_position: 2
---

# Ein Dokument erstellen

Dokumente sind **Gruppen von Seiten**, die durch:

- eine **Seitenleiste**
- **Vorherige/Nächste Navigation**
- **Versionierung**

## Erstellen Sie Ihr erstes Doc

Erstellen Sie eine Markdown-Datei unter `docs/hello.md`:

```md title="docs/hello.md"
## Hallo

Dies ist mein **erstes Docusaurus-Dokument**!
```

Ein neues Dokument ist jetzt unter [http://localhost:3000/docs/hello](http://localhost:3000/docs/hello) verfügbar.

## Konfigurieren Sie die Seitenleiste

Docusaurus **erzeugt automatisch eine Seitenleiste** aus dem Ordner "docs".

Fügen Sie Metadaten hinzu, um die Bezeichnung und Position der Seitenleiste anzupassen:

```md title="docs/hello.md" {1-4}
---
sidebar_label: 'Hallo!'
sidebar_position: 3
---

# Hallo

Dies ist mein **erstes Docusaurus-Dokument**!
```

Es ist auch möglich, Ihre Seitenleiste explizit in `sidebars.js` zu erstellen:

```js title="sidebars.js"
export default {
  tutorialSidebar: [
    'intro',
    // highlight-next-line
    'hallo',
    {
      Typ: 'Kategorie',
      Bezeichnung: 'Tutorial',
      items: ['tutorial-basics/create-a-document'],
    },
  ],
};
```