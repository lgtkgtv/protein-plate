# 🍽️ ProteinPlate

[![License: MIT](https://img.shields.io/badge/Code-MIT-yellow.svg)](LICENSE)
[![Content: CC BY 4.0](https://img.shields.io/badge/Content-CC%20BY%204.0-lightgrey.svg)](LICENSE-CONTENT)
[![Built with Material for MkDocs](https://img.shields.io/badge/Built%20with-MkDocs%20Material-blue.svg)](https://squidfunk.github.io/mkdocs-material/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

> A free, open guide to **high-protein, lower-calorie Indian home meals** — annotated plates, family-of-4 recipes, batch-cooking plans, grocery lists, and a keto chapter. Built for public good.

[Live Site](https://lgtkgtv.github.io/protein-plate/) · [Report an issue](https://github.com/lgtkgtv/protein-plate/issues) · [Suggest a recipe](https://github.com/lgtkgtv/protein-plate/issues)

---

## 🎯 What this is

ProteinPlate documents one simple, repeatable meal template seen across dozens of real home-cooked plates:

> **Half the plate non-starchy veg (cooked + raw) · a quarter protein · a small corner of healthy fat (nuts/seeds + a little oil) · a glass of thin dairy.**

The protein anchor rotates across **sprouts/legumes, paneer, eggs, chicken, and lentil/besan cheela**, keeping each plate around **450–600 kcal with 30–45 g protein** — without rice, roti, or sugar.

### Why it exists

- ✅ **Practical, not theoretical** — real portions in grams, scaled for a family of 4
- ✅ **Batch-cook friendly** — a 90-minute Sunday prep drives the whole week
- ✅ **Markdown-first** — contributors add recipes by editing plain text, not HTML
- ✅ **Open & free** — content under CC BY 4.0, for anyone to reuse with attribution

## 📚 Contents

| Page | What's inside |
|------|----------------|
| The Plate | Anatomy of a plate, annotated, with portions in grams |
| Ingredients & Portions | Every dish → its raw ingredients; recurring-portion summary |
| Recipes | The cookbook — recipes for 4, with verified video links |
| 7-Day Meal Plan | A decision-free week mapped to the batch-cook plan |
| Grocery List | Weekly shopping list for a family of 4 |
| Keto Chapter | An optional stricter low-carb variation (with cautions) |
| About & Health Note | Honest limitations and a wellness disclaimer |

## 🚀 Quick start

### For readers
Just visit the **[live site](https://lgtkgtv.github.io/protein-plate/)** — nothing to install.

### For contributors (run it locally)

```bash
# 1. Clone
git clone https://github.com/lgtkgtv/protein-plate.git
cd protein-plate

# 2. Install the one dependency
pip install mkdocs-material

# 3. Preview live at http://127.0.0.1:8000 (auto-reloads as you edit)
mkdocs serve
```

Edit any file in `docs/`, save, and the preview updates instantly.

## 🛠️ How deployment works

Pushing to `main` triggers `.github/workflows/deploy.yml`, which builds the site and publishes it to the `gh-pages` branch. GitHub Pages serves it at `lgtkgtv.github.io/protein-plate/`. See [`docs/about.md`](docs/about.md) and the repo's first-time setup notes.

## 🤝 Contributing

Recipes, corrections, translations, and portion data are all welcome — see [CONTRIBUTING.md](CONTRIBUTING.md).

## 📜 License

- **Code & configuration:** [MIT](LICENSE)
- **Written content, recipes & guide:** [CC BY 4.0](LICENSE-CONTENT)

## ⚠️ Disclaimer

ProteinPlate is **general food and wellness information, not medical or dietetic advice.** Calorie and protein needs are personal. Consult a registered dietitian or doctor before a calorie-restricted or ketogenic diet, especially with any medical condition.
