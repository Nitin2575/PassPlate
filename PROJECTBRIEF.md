# PassPlate: Project Brief

A systems design exercise in turning a fragmented, emotionally loaded coordination problem into a portable identity layer, and solving the cold-start problem that kills most products in this space.

This brief is written to show how I think, not to pitch a product. The full overview lives in the [README](./README.md).

---

## The one-line version

People with allergies, restrictions, or dietary needs re-explain themselves at every meal, through unstructured channels that lose or distort safety-critical information. PassPlate replaces that with a structured dietary identity the individual owns and hands off cleanly to whoever is feeding them.

---

## The problem worth solving

The interesting problem here isn't food discovery, which is crowded. It's the handoff.

Dietary information today lives in reservation notes, text threads, server conversations, and catering spreadsheets. Every one of those is unstructured, lossy, and re-created from scratch each time. The cost isn't only inconvenience. It's the person who feels like a burden for asking, and the allergy that gets missed because it was buried in a free-text field.

So I framed the real problem as a **data and trust handoff** between two parties who currently have no shared format: the person with the need, and the person preparing the food.

---

## The hard part: cold start

This is where most products in this category die, and where I spent the most design effort.

A dietary profile is worthless if the other side won't read it. The other side won't adopt a new tool unless enough people already use it. That leaves the usual dead ends:

- Consumer-only profile app: no reason for restaurants to read it.
- Restaurant-only dashboard: no reason for restaurants to add another screen.
- Two-sided marketplace: needs both sides to show up on day one.

My answer was to refuse the marketplace framing entirely and find a job that's valuable with **zero network**.

**HostPlate is that wedge.** A host, caterer, or event organizer already needs to collect dietary info today, through a painful mix of texts and spreadsheets. HostPlate does that one job better immediately, for one user, with no network required. Then the loop closes: every guest who fills out a form is one tap away from saving a reusable identity. One-time intake becomes long-term adoption. A workflow tool grows into an identity network, instead of betting on network effects that don't exist yet.

That sequencing decision (workflow value first, identity network second) is the core of the product.

---

## System design

One system, four surfaces, each with a clear job:

| Surface | Job | Who it serves |
|---|---|---|
| **PlateID** | The portable dietary identity. Owned by the user. | Individual |
| **The Pass** | PlateID as a shareable credential (link, QR, tap, wallet pass). | Individual to host |
| **HostPlate** | Collects and summarizes guest needs into one view. | Host / venue |
| **ScanPlate** | Checks a PlateID against a menu or event. | Both sides |

The deliberate constraint: PassPlate sits *on top of* existing systems (OpenTable, Toast, Resy, the rest) rather than replacing them. The bet is that an identity layer travels further than another standalone app.

---

## Decisions and tradeoffs

A few choices I'd defend in a design review:

**Dignity as a product requirement, not a tagline.** The emotional cost of re-explaining yourself is the actual problem. That pushed specific decisions: the individual owns the data, the handoff is one action, and the host sees a clean summary rather than a raw medical disclosure.

**HostPlate before the consumer app.** Counterintuitive, since the "product" feels like the consumer profile. But shipping the consumer side first walks straight into the cold start. Leading with the host workflow is the only sequence where day-one value doesn't depend on a network.

**AI as a communication layer, scoped narrowly.** It structures messy notes and translates needs into plain language. It explicitly does not make medical or safety claims. Drawing that line is a product-safety decision, not a limitation I backed into.

**An honest competitive read.** Allergy cards and restriction-filtering apps exist, but they solve one-time disclosure for one person in one place. The unowned space is the reusable, two-sided, portable handoff. That's the only territory worth defending.

---

## What I'd build first

A web-based PlateID profile plus a shareable page, with HostPlate as the wedge. Allergy and severity entry, a host intake form, an AI-generated summary, and the wallet-pass concept. No marketplace, no payments, no medical claims in v1. The goal of the MVP is to validate one thing: that the host workflow is good enough to pull guests into saving a reusable identity.

---

## What this project demonstrates

- Reframing a crowded space (food discovery) into an unowned one (dietary compatibility and handoff).
- Diagnosing and designing around the cold-start failure mode that kills this category.
- Sequencing a product so day-one value doesn't depend on network effects.
- Drawing a clear, defensible line around what AI should and shouldn't do in a safety-adjacent context.
- Translating an emotional user problem into concrete product constraints.

---

## Status and role

**Status:** Concept, systems design, and MVP planning. Active design work, not a shipped product.

**My role:** Problem framing, product strategy and positioning, system and user-flow design, cold-start strategy, MVP scoping, and AI workflow design.

**Disclaimer:** PassPlate is a conceptual portfolio project. It is not a medical, nutritional, or allergy-safety tool and should not be relied on for safety-critical decisions.

---

**Nitin Bhogaraju**, Biomedical Engineering graduate. Consumer health, foodtech, AI workflows, and product design.
