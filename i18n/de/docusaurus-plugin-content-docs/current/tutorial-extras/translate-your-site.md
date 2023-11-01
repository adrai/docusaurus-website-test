---
sidebar_position: 2
---

# Übersetze deine Seite

Lassen Sie uns `docs/intro.md` ins Französische übersetzen.

## Konfigurieren Sie i18n

Ändern Sie `docusaurus.config.js`, um Unterstützung für das Gebietsschema `fr` hinzuzufügen:

```js title="docusaurus.config.js"
export default {
  i18n: {
    defaultLocale: 'en',
    locales: ['en', 'fr'],
  },
};
```

## Eine Dokumentation übersetzen

Kopieren Sie die Datei `docs/intro.md` in den Ordner `i18n/fr`:

```bash
mkdir -p i18n/fr/docusaurus-plugin-content-docs/current/

cp docs/intro.md i18n/fr/docusaurus-plugin-inhalt-docs/current/intro.md
```

Übersetzen Sie `i18n/fr/docusaurus-plugin-content-docs/current/intro.md` in Französisch.

## Starten Sie Ihre lokalisierte Seite

Starten Sie Ihre Seite mit dem französischen Gebietsschema:

```bash
npm run start -- --locale fr
```

Ihre lokalisierte Seite ist unter [http://localhost:3000/fr/](http://localhost:3000/fr/) erreichbar und die Seite "Getting Started" ist übersetzt.

:::caution

In der Entwicklung können Sie immer nur ein Gebietsschema verwenden.

:::

## Ein Gebietsschema Dropdown hinzufügen

Um nahtlos zwischen den Sprachen zu navigieren, fügen Sie ein Gebietsschema-Dropdown hinzu.

Ändern Sie die Datei `docusaurus.config.js`:

```js title="docusaurus.config.js"
export default {
  themeConfig: {
    navbar: {
      Elemente: [
        // highlight-start
        {
          Typ: 'localeDropdown',
        },
        // highlight-end
      ],
    },
  },
};
```

Das Gebietsschema-Dropdown erscheint nun in Ihrer Navigationsleiste:

![Locale Dropdown](./img/localeDropdown.png)

## Erstellen Sie Ihre lokalisierte Website

Erstellen Sie Ihre Seite für ein bestimmtes Gebietsschema:

```bash
npm run build -- --locale fr
```

Oder erstellen Sie Ihre Seite in