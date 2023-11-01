---
sidebar_position: 1
---

# Eine Seite erstellen

Fügen Sie **Markdown- oder React**-Dateien zu `src/pages` hinzu, um eine **eigenständige Seite** zu erstellen:

- `src/pages/index.js` → `localhost:3000/`
- `src/pages/foo.md` → `localhost:3000/foo`
- `src/pages/foo/bar.js` → `localhost:3000/foo/bar`

## Erstellen Sie Ihre erste React-Seite

Erstellen Sie eine Datei unter `src/pages/my-react-page.js`:

```jsx title="src/seiten/meine-react-seite.js"
importiere React von 'react';
importiere Layout von '@theme/Layout';

export default function MeineReactSeite() {
  return (
    <Layout>
      <h1>Meine React-Seite</h1>
      <p>Dies ist eine React-Seite</p>
    </Layout>
  );
}
```

Eine neue Seite ist nun unter [http://localhost:3000/my-react-page](http://localhost:3000/my-react-page) verfügbar.

## Erstellen Sie Ihre erste Markdown-Seite

Erstellen Sie eine Datei unter `src/pages/my-markdown-page.md`:

```mdx title="src/seiten/meine-markdown-seite.md"
# Meine Markdown-Seite

Dies ist eine Markdown-Seite
```

Eine neue Seite ist jetzt verfügbar unter [http://localhost:3000/my-markdown-page](http://localhost:3000/my-markdown-page).