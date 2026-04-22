# MyServing/NutriScan — Food Health & Nutrition Tracker

> A smart, camera-powered food tracking app that reads nutrition labels, monitors your intake, and helps you make healthier choices — all tailored to *your* serving sizes.

---

## Project Overview

NutriScan is a mobile-first food health application that removes the friction from calorie and nutrition tracking. Instead of manually logging meals, users can simply scan the packaging of any food item. The app reads the nutrition label automatically and then calculates an accurate breakdown based on how much the user actually consumed — not just the suggested serving size on the box.

The goal is to give users a clear, honest picture of what they're eating, flag potential dietary concerns, and guide them toward healthier habits over time.

---

## App Structure

The app is organized into two primary tabs:

### Tab 1 — Scanner
The entry point of the app. Users point their camera at a food item's packaging and the app:
- Reads and parses the **ingredients list**
- Extracts the **nutrition facts panel** (calories, protein, sugar, fat, etc.)
- Identifies **dietary warnings** (e.g. high gluten, added dyes, excessive sugar content)
- Stores the scanned item for future reference

### Tab 2 — My Serving
Once a food is scanned, users define their own serving size — because real portions rarely match the label. This tab:
- Lets users **set or adjust their personal serving size** (by weight, volume, or visual reference)
- Recalculates all nutrition values proportionally to their actual serving
- Displays a clean breakdown of **calories, protein, sugar, food groups**, and any **health flags**
- Supports scanning or photographing the portion directly using a user-provided reference object (e.g. a hand, a bowl, a cup) for a visual size estimate

---

## Core Features

### Smart Label Scanning
- OCR-powered camera scan of nutrition labels and ingredient lists
- Automatic extraction of macronutrients: calories, protein, carbohydrates, sugars, fats
- Food group classification based on ingredient data

### Dietary Warning System
Flags items that contain or exceed thresholds for:
- High gluten content
- Excessive added sugars
- Artificial dyes / colorants
- Other configurable dietary alerts

### Personalized Serving Sizes
- Users set what *their* serving looks like, independent of the label
- Nutrition totals dynamically recalculate to match the custom serving
- Previously scanned foods can be re-used — just snap a new photo of your portion using a visual reference

### Recently Scanned Foods
- Quick access to a history of scanned items
- Re-scan or re-use any previous food entry without rescanning the full label
- Takes a new picture of the current portion for an updated, accurate reading

---

## Planned Features

| Feature | Description |
|---|---|
| **Flavour Profiles** | Categorize and surface foods by taste profile (sweet, savory, umami, etc.) |
| **Healthier Alternatives** | Suggest nutritionally similar but healthier swaps for flagged items |
| **Shopping Cart & Fridge Tracker** | Log purchases, track what's in the fridge, and monitor consumption over time |
| **Recipe Recommendations** | Based on what's currently in the fridge, suggest balanced meal ideas |

---

## Vision

The broader vision for NutriScan is to act as a **personalized nutrition companion** — one that understands your pantry, adapts to your eating habits, and proactively suggests ways to improve your diet without requiring obsessive manual tracking. By anchoring everything to what the user actually eats (not idealized label servings), the app aims to be both more accurate and more realistic than traditional calorie counters.

---

## Tech Stack *(TBD / In Progress)*

- Camera / OCR integration for label scanning
- Nutrition database or label parsing model
- Dynamic UI with two-tab navigation
- User profile & history storage
- (Future) Computer vision for portion size estimation via reference objects

---

## Contributing

This project is in early planning/development. If you're a team member and want to contribute ideas, flag an issue or reach out directly. Core architecture decisions are still open for discussion — especially around the OCR/label-parsing approach and the portion estimation model.

---

*Built to make eating well a little less complicated.*
