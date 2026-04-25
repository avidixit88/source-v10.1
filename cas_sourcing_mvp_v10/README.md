# CAS Sourcing & Procurement Intelligence MVP v9

Streamlit MVP for CAS-number sourcing with a strict supplier-registry flow.

## What v9 changes

- Walks the curated supplier registry supplier-by-supplier instead of letting generic search results dominate.
- Gives each supplier its own extraction budget so one noisy domain cannot consume all pages.
- Adds strict CAS identity validation so a wrong product page cannot pass just because the requested CAS appeared in a search snippet or adapter seed.
- Canonicalizes URLs and collapses common multilingual mirrors such as `/jp`, `/kr`, `/de`, etc.
- Groups results into Apple-style supplier cards with product-level evidence hidden behind an expander.
- Keeps product evidence and supplier summary exports separate.

## Run locally

```bash
pip install -r requirements.txt
streamlit run app.py
```

## Recommended Streamlit Cloud Python

Use Python 3.12.

## Testing suggestions

Start with:

- `151-21-3` — Sodium dodecyl sulfate
- `64-17-5` — Ethanol
- `100-51-6` — Benzyl alcohol
- `86-73-7` — Fluorene

Use **Live supplier discovery** and keep direct supplier links enabled. SerpAPI is optional.

