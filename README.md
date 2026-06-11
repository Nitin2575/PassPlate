# PassPlate

**A portable dietary identity layer, so no one has to re-explain their allergies, restrictions, or food needs every time they eat with others.**

PassPlate turns the messy, repeated, often awkward work of communicating food needs into a single structured profile that travels with you. Share it by link, QR code, tap, or an Apple Wallet-style pass, and let the hosts, restaurants, and events that need it read it directly.

---

## The Problem

Communicating food needs is still fragmented, manual, and emotionally loaded.

Today, dietary information lives in reservation notes, text threads, server conversations, catering spreadsheets, and "allergy/restriction" fields that are unstructured, inconsistent, and easy to miss. The burden sits entirely on the individual to re-explain personal health, religious, cultural, or lifestyle needs, over and over, and hope the other side understood.

That creates real friction on both sides:

- People repeat sensitive personal information at every meal and often feel like a burden for asking to be accommodated.
- Hosts and restaurants receive incomplete or unclear information, sometimes about safety-critical allergies.
- Group dining turns stressful or exclusionary.

The problem isn't finding food. It's **communicating food identity with clarity and dignity.**

---

## The Thesis

The future of food coordination isn't restaurant discovery. It's **dietary compatibility.**

People need a portable, structured, shareable way to express what they can eat, what they avoid, and what matters most in a food environment. PassPlate is the identity and handoff layer that makes that possible across every place food happens.

Think of it as a wallet pass for your dietary identity.

---

## What PassPlate Is

PassPlate is one system with four surfaces:

**PlateID:** Your portable dietary identity. Allergies, restrictions, religious rules, preferences, sensitivities, severity levels, safe foods, foods to avoid, and how you prefer to communicate them. One profile, owned by you.

**The Pass:** Your PlateID as a shareable credential. A clean summary you open and hand off in seconds, by link, QR code, NFC tap, or Apple Wallet-style pass. No re-explaining from scratch.

**HostPlate:** The host-, restaurant-, and event-facing view. A host creates a link, guests fill in their needs, and HostPlate generates one clean dietary summary for the whole table.

**ScanPlate:** The compatibility layer. Scan a menu, table, or event and check it against your PlateID.

PassPlate is designed to sit *on top of* existing systems (Square, OpenTable, Resy, Toast, DoorDash, Uber Eats, event and catering tools), not replace them. It's the structured dietary layer that travels across all of them.

---

## How It Works

1. A host creates a HostPlate link for a dinner, event, group meal, or catering order.
2. Guests fill in allergies, restrictions, preferences, and severity. No account required.
3. HostPlate generates one clean dietary summary for the host.
4. Guests are prompted to save their answers as a reusable **PlateID**.
5. From then on, they share that PlateID anywhere by link, QR, tap, or wallet pass.
6. Over time, ScanPlate checks a PlateID against menus, events, and food options.

---

## Why HostPlate First (the wedge)

Most dietary-profile ideas die at the cold start: a profile is only useful if the other side reads it, and the other side won't adopt a new tool unless enough people already use it. Consumer-only apps stall, restaurant-only dashboards stall, and two-sided marketplaces need both sides at once.

PassPlate avoids that trap by starting where the need already exists.

A host, caterer, event organizer, or group-dinner planner needs to collect dietary information *today*, usually through a chaotic mix of texts and spreadsheets. HostPlate is immediately useful for that one job, with zero network required. It delivers value on day one, even if no guest has ever heard of PassPlate.

Then the loop closes: every guest who fills out a HostPlate form is one prompt away from saving a reusable PlateID. One-time intake becomes long-term identity. The wedge is a workflow tool that quietly grows into a portable identity network.

---

## The Landscape

Tools exist for pieces of this: allergy translation cards, restriction-filtering apps, restaurant directories. But they tend to solve **one-time disclosure for one person in one place.**

No one owns the part that's actually hard: a *reusable* dietary identity that the individual controls, that hands off cleanly to the *other side* of the table, and that travels across hosts, restaurants, and events. That two-sided, portable, reusable handoff is the white space PassPlate is built for.

*(Detailed competitive comparison: in progress.)*

---

## Why Now

The pieces this needs all arrived in the last few years, and they arrived together.

Portable credentials became muscle memory. Apple Wallet and Google Wallet, NameDrop-style tap sharing, and scan-to-open interactions are now everyday behavior. A few years ago, "open your pass and share it" needed explaining. Today it's a reflex, which means the handoff PassPlate depends on no longer has to be taught.

Restaurants already digitized the read side. QR menus and digital ordering went mainstream after 2020. Venues that would never have added a new screen now already have scan-based touchpoints, which lowers the cost of the other side ever reading a PlateID.

AI made the messy part cheap. Structuring free-text allergy notes, summarizing a whole guest list for a host, and translating needs into plain language were impractical to build before modern language models. They're now a thin, affordable layer. The work that makes the data actually usable just dropped in cost by an order of magnitude.

Dietary identity is more common and more visible. Food allergy prevalence is rising, and dietary identity has broadened well beyond allergies into religious, health, and lifestyle needs that people now carry openly into every social meal. The friction surface is growing, not shrinking.

None of these alone makes PassPlate possible. Together they mean the infrastructure, the behavior, and the enabling technology finally line up at the same time.

---

## The AI Layer

AI acts as a communication and coordination layer, never a substitute for medical, nutritional, or allergy advice. Use cases include:

- Menu compatibility checks against a PlateID
- Structuring messy, free-text allergy notes into clear categories
- Host-facing summaries across a whole guest list
- Translating dietary needs into plain, shareable language
- Safer ordering suggestions and group-dining coordination

---

## Who It's For

**Primary:** People with allergies, restrictions, preferences, sensitivities, or specific food goals.
**Secondary:** Restaurants, hosts, caterers, and event teams that need to understand guest food needs.
**Everyone around them:** Friend groups, families, and event teams trying to coordinate food without the stress.

---

## MVP Scope

A web-based dietary profile and share page, with HostPlate as the first practical wedge.

**In scope**
- PlateID profile with allergy/restriction entry and severity tagging
- Shareable profile link plus QR/tap access
- Apple Wallet-style pass concept
- HostPlate intake form and host summary
- AI-generated dietary explanation

**Out of scope (for now)**
- Restaurant marketplace, payments, reservations
- Medical claims, full nutrition planning
- Deep platform integrations

---

## Status

**Concept · product brief · systems design · MVP planning.**

This repo documents the thesis, product surfaces, AI layer, user flow, cold-start strategy, and MVP direction. It's an active design effort, not a shipped product.

---

## My Role

Product strategy and positioning · consumer product thinking · user-flow and dietary-identity system design · MVP planning · AI workflow framing · public project documentation.

---

## Disclaimer

PassPlate is a conceptual portfolio project at the intersection of dietary identity, hospitality, and AI-assisted communication. It is **not** a medical, nutritional, or allergy-safety tool, and should not be relied on for safety-critical decisions.

---

## Contact

**Nitin Bhogaraju**, Biomedical Engineering graduate, focused on consumer health, foodtech, AI workflows, and product design.

- LinkedIn: www.linkedin.com/in/nitinbhogaraju
- Email: nitinbhogaraju@gmail.com
