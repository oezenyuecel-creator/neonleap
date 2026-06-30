# NEON LEAP ⚡

Ein moderner, vertikaler Endless-Jumper (Doodle-Jump-DNA) im **Synthwave-/Neon-Look**.
Eigenständiger One-File-Prototyp — `index.html` öffnen, fertig. Keine Build-Tools, keine Dependencies.

## Vision
Casual, sofort verständlich, hochgradig teilbar ("nur noch ein Run"). Signature-Element:
ein **Charakter mit verpixeltem, wehendem Neon-Umhang**, dessen Skin (Body + Cape) austauschbar ist.

## Was schon drin ist (v0.4)
- **Gameplay**: Auto-Bounce, prozedurale Plattformen, Screen-Wrap, nur-nach-oben-Kamera, Höhen-Score
- **Biome beim Klettern** (eskalierender Look + Gefühl, mit Übergangs-Banner), jedes mit **eigenem Hazard**:
  - 🌆 **SYNTHWAVE** (Start) — 🕳️ Schwarzes Loch (saugt an)
  - 🏙️ **CYBER CITY** (~900, Skyline) — ⚡ Laser-Gate (an/aus im Takt, durchtimen)
  - 🌌 **DEEP SPACE** (~2000, Planeten, leichtere Gravity) — 🛸 UFO (driftet, tötet bei Kontakt)
  - 👾 **GLITCH VOID** (~3300, Glitch-Flackern, schwerer) — ⚙️ Sägeblatt (rotiert, fährt quer)
- **Plattform-Typen**: normal (cyan), Spring/Booster (grün, Mega-Sprung), beweglich (lila), zerbrechlich (pink), Cloud (vergeht)
- **Power-Ups**:
  - 🚀 **Jetpack** — kurzer Auto-Flug mit Flammen-Trail, schießt dich nach oben
  - 🧲 **Magnet** — zieht Orbs im Umkreis an (Aura um den Charakter)
  - aktives Power-Up mit Countdown-Balken im HUD
- **Hazard**: 🕳️ **Schwarzes Loch** — saugt dich an (ab ~650 Höhe); Jetpack reduziert den Sog & macht kurz immun → du kannst dich rauspowern
- **Orbs** als Währung — fließen in dauerhaftes Orb-Konto
- **Skins**: 6 Stück (VOLT, MAGMA, TOXIC, NOVA, FROST, SPECTRUM/Rainbow), per Orbs freischaltbar & equippbar
- **Verpixelter Neon-Cape**: geflärter Pixel-Cloak mit Glow, der wogt und entgegen der Laufrichtung trailt
- **Juice**: Partikel, Screenshake, Combo-System, Squash-&-Stretch, Web-Audio-SFX
- **⚙️ Einstellungs-Screen** (Zahnrad oben links, immer sichtbar): **Steuerung** umschaltbar — **Tippen** (Finger-Folge: der Held steuert präzise dorthin, wo der Daumen liegt/zieht, mit sanfter Ankunft & sauberem Stopp) ODER **Neigen** (Tilt, mit Neutral-Kalibrierung beim Start) — plus **Ton** an/aus. Alles wird gespeichert. Am PC immer ← → / A D. Default: Tippen (kein Permission-Prompt, läuft überall)
- **Persistenz** (localStorage): Bestscore, Orbs, freigeschaltete/equippte Skins, Mute
- Mobile-first, responsiv, hochauflösend (DPR-aware Canvas)

## Lokal starten
```
npx serve . -l 4711
# oder einfach index.html im Browser öffnen
```

## Roadmap-Ideen
Spieltiefe als Nächstes:
- **Mehr Power-Ups**: Schild, Slow-Mo, Raketen-Feder
- **Adaptive Musik pro Biom** + Haptics
- **Run-Missionen** ("erreiche 1.500", "5er-Spring-Combo")
- Neue Plattform-Typen: Conveyor, Portal, Eis · Skill-Move: Dash/Doppelsprung

Richtung viral (später):
- **Share-Card** nach Game Over (Score + Skin als teilbares Bild)
- **Tägliche Challenge / Seed-Runs**, **Leaderboard** (Supabase, wie bei Zigzy) + Freundes-Ghost
- **Cape-Muster** (Glitch, Flammen, Sterne) + saisonale Skin-Drops
- Haptics, Musik-Loop, Tutorial-Onboarding
```
```
