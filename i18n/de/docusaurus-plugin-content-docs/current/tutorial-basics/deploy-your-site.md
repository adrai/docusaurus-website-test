---
sidebar_position: 5
---

# Stellen Sie Ihre Site bereit

Docusaurus ist ein **Static-Site-Generator** (auch **[Jamstack](https://jamstack.org/)** genannt).

Er erstellt Ihre Website als einfache **statische HTML-, JavaScript- und CSS-Dateien**.

## Erstellen Sie Ihre Website

Erstellen Sie Ihre Seite **für die Produktion**:

```bash
npm run build
```

Die statischen Dateien werden im Ordner `build` erzeugt.

## Verteilen Sie Ihre Site

Testen Sie Ihren Produktions-Build lokal:

```bash
npm run serve
```

Der "Build"-Ordner wird nun unter [http://localhost:3000/](http://localhost:3000/) bereitgestellt.

Sie können den "Build"-Ordner nun **fast überall** einfach bereitstellen, **kostenlos** oder für sehr geringe Kosten (lesen Sie den **[Deployment Guide](https://docusaurus.io/docs/deployment)**).