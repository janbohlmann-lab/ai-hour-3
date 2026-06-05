# pd-brand/fonts — Schrift-Dateien

Lokale Font-Files, damit unsere Outputs CDN-unabhängig und reproduzierbar rendern.

> **Privates/internes Repo.** Diese Fonts sind lizenziert für Pets Deli. Sie werden
> bewusst hier committet (Entscheidung 2026-06-04, Jan), damit ein frischer Clone
> alles hat. **Nicht öffentlich pushen / weiterverteilen.**

## Erwartete Struktur

| Ordner / Datei | Schrift | Lizenz | Quelle | Status |
|---|---|---|---|---|
| `roboto/` | **Roboto** (400/500/900, Variable-woff2 latin + latin-ext) | Apache 2.0 (frei) | Google Fonts / gstatic | ✅ vorhanden |
| `mindset/` | **Mindset Slim** (Headlines, OTF + TTF) | kommerziell (PintassilgoPrints) — PD-lizenziert | PD Drive › 02 PD FONTS › Mindset | ✅ vorhanden |
| `neue-haas/` | **Neue Haas Grotesk** (55 Roman + 75 Bold, woff2 + woff) | kommerziell (Monotype) — PD-lizenziert | PD Drive › 02 PD FONTS › 00 WEB FONT KITS | ✅ vorhanden |

## Provenienz

- **Roboto:** frei (Apache 2.0), self-hosted aus Google Fonts. Lizenz in `roboto/LICENSE.txt`.
- **Mindset Slim** & **Neue Haas Grotesk:** PD besitzt die Lizenzen; die Files
  stammen ausschließlich aus PDs eigener Brand-Ablage
  (`PD Drive › Geteilte Ablagen › PETS DELI › 00 PD BRAND › 02 PD FONTS`,
  inkl. License-Ordner). **Nicht** von Drittquellen bezogen.

## Einbindung

`@font-face` wird in `../pd-brand.css` verdrahtet (lokale Pfade, kein Google-Fonts-`@import`).
Fredoka bleibt nur als Last-Resort-Fallback für Headlines, bis Mindset Slim hier liegt.
