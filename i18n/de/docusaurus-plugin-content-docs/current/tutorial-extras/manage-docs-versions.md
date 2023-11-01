---
sidebar_position: 1
---

# Docs-Versionen verwalten

Docusaurus kann mehrere Versionen Ihrer Dokumente verwalten.

## Erstellen einer Doku-Version

Geben Sie eine Version 1.0 Ihres Projekts frei:

```bash
npm run docusaurus docs:version 1.0
```

Der Ordner `docs` wird in `versioned_docs/version-1.0` kopiert und `versions.json` wird erstellt.

Ihre Dokumente haben nun 2 Versionen:

- `1.0` unter `http://localhost:3000/docs/` für die Version 1.0 der Dokumente
- `current` unter `http://localhost:3000/docs/next/` für die **künftigen, unveröffentlichten Dokumente**

## Hinzufügen eines Versions-Dropdowns

Um nahtlos zwischen den Versionen zu navigieren, fügen Sie ein Versions-Dropdown hinzu.

Ändern Sie die Datei `docusaurus.config.js`:

```js title="docusaurus.config.js"
export default {
  themeConfig: {
    navbar: {
      Elemente: [
        // highlight-start
        {
          Typ: 'docsVersionDropdown',
        },
        // highlight-end
      ],
    },
  },
};
```

Das Dropdown für die Docs-Version erscheint in Ihrer Navigationsleiste:

![Docs Version Dropdown](./img/docsVersionDropdown.png)

## Eine bestehende Version aktualisieren

Es ist möglich, versionierte Dokumente in ihrem jeweiligen Ordner zu bearbeiten:

- `versioned_docs/version-1.0/hello.md` aktualisiert `http://localhost:3000/docs/hello`
- `docs/hello.md` aktualisiert `http://localhost:3000/docs/next/hello`