# Music AI Compliance Navigator

> Interactive decision-tree tool for AI music compliance.  
> EU AI Act · GDPR · Artist rights · Built as a learning side project.

**Status:** V1 live prototype. V2 in development with a collaborating backend engineer.

**Try it:** [pi-kay.github.io/Music-ai-compliance-navigator](https://pi-kay.github.io/Music-ai-compliance-navigator/)

---

## What it does

Input a use case → get relevant requirements, risks, and action steps, with citations back to the source regulations.

Structured decision tree, not a chatbot — every answer is predictable, verifiable, and traceable to a primary source. Each decision path ends in a structured output with four consistent fields (requirements, risks, actions, sources), so content is uniform across use cases and easy to update.

Unhandled situations route to a lightweight edge-case log so the tree can grow from real user input rather than guesswork.

## Use cases (v1)

1. **Consent & Attribution** — Was this data, voice, or work used with permission? What attribution is required?
2. **Training Data Provenance** — Where did this model's training data come from? How do I document or verify it?
3. **Generated Output Rights** — Who owns what I made with AI? Can I sell it? What do I owe?
4. **Transparency & Disclosure** — When must I disclose AI use? To whom? How?
5. **Authenticity & Recognition** — How can creators prove and protect original work?

These use cases are bidirectional — useful whether you're an artist protecting yourself or a company trying to do right.

---

## Project context

Navigator is one part of a small toolkit for music-AI compliance:

- **Guide** — creator-side reference, published Dec 2025 ([Music-AI-Vault repo](https://github.com/Pi-Kay/Music-AI-Vault))
- **Navigator web app (this repo)** — decision-tree tool, V1 live
- **Handbook** — developer-facing companion, in progress
- **Backend V2** — production version with auto-updating regulation feeds, in development with a collaborating engineer

Full arc and reasoning: [portfolio case study](https://pi-kay.github.io/portfolio/navigator.html).

This is an exemplary, open side project. Orientation, not legal advice. Practitioner-to-practitioner — not a product, not a consultancy offering.

---

## Tech stack

- **React 18** — component structure for the decision tree
- **Vanilla CSS** — no framework, intentionally simple
- **JSON** — decision tree data, separated from logic for easier updates
- **GitHub Pages** — static hosting
- **Git** — version control and change history

Prototyped with Claude as a design-and-code collaborator. See [docs/PROMPTS.md](docs/PROMPTS.md) for the pivotal prompts that shaped the architecture.

---

## Run locally

```bash
git clone https://github.com/Pi-Kay/music-ai-compliance-navigator.git
cd music-ai-compliance-navigator
npm install
npm run dev
```

Updating the decision tree: edit the relevant JSON file under `src/data/` — no code changes required for content updates.

---

## Project documentation

This project documents AI-human collaboration openly. The documentation is part of the deliverable, not a side-note.

- [docs/PROJECT.md](docs/PROJECT.md) — scope, roles, methodology
- [docs/DECISIONS.md](docs/DECISIONS.md) — key human decisions with rationale (architecture, scope, positioning)
- [docs/PROMPTS.md](docs/PROMPTS.md) — pivotal AI prompts, with annotations on what worked and what didn't
- [CHANGELOG.md](CHANGELOG.md) — running updates

---

## V2 in development

A collaborating backend engineer is building the production version:

- Auto-updating regulation feeds from official sources (AI Office, EDPB, ENISA)
- Embeddable API so platforms can offer compliance guidance inside their own products
- Draft API surface and user stories are in the forthcoming developer handbook

My ongoing role: frontend collaboration, accessibility implementation, language translation, editorial calls on tree logic.

---

## Contributing

Corrections and worked examples from practitioners are welcome. Two paths:

- **Open an issue** for wrong, unclear, or out-of-date content. Use labels: `correction`, `clarification`, `update`, `editorial`.
- **Submit a pull request** for concrete edits. For larger changes, open an issue first so we can discuss fit.

---

## Licence

Code: MIT.  
Decision tree content and copy: CC BY-SA 4.0, consistent with the [Music-AI-Vault](https://github.com/Pi-Kay/Music-AI-Vault) Guide.

*(Adjust if your actual licence setup differs.)*

---

## Author

Petra Kühnle  
[Portfolio](https://pi-kay.github.io/portfolio/) · [LinkedIn](https://www.linkedin.com/in/petrakuhnle)
