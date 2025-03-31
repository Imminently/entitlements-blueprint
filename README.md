# Entitlements Blueprint
![Build Real Rules](https://img.shields.io/badge/Builds-real_rules-green)
![COBOL-Free](https://img.shields.io/badge/Codebase-COBOL_free-brightgreen)
![Temporal Logic Included](https://img.shields.io/badge/Temporal--support-yes-blue)

> A practical blueprint for building transparent, rules-based entitlements engines — no black boxes.

✅ 100% accuracy vs mainframe | 🧠 Natural language rules | 📊 Fully traceable decisions | ⏱️ Sub-500ms runtime | 👥 Built by 3 engineers + 3 SMEs in 8 weeks

## 👋 Why this exists

Modernising legacy welfare systems doesn't have to start with millions of lines of 1970s COBOL.

What if you started from the legislation itself?

This repo presents a reference architecture and case study from a project delivered inside the Australian Government, where — in just 8 weeks — we digitised the entire Aged Pension Act into a fully operational rules engine.

We ran side-by-side with a national mainframe and achieved **100% accuracy**, while also generating **real-time audit reports** that explained every outcome — in natural language.

Built by a team of **3 engineers and 3 policy experts. No black boxes. No months of handover.**

And yes, it was faster, cheaper, and more transparent than the existing system.

## 🧠 Our Philosophy

Legacy systems in social services often contain a complex web of decisions buried in code. Instead of rewriting this legacy code line-by-line, we took a **top-down approach**:

- Start with **legislation**, not legacy code.
- Use natural language and graph-based rules to **digitise the actual logic**.
- Generate a **transparent, explainable, and auditable engine**.
- Deliver decisions in sub-500ms with complete traceability.

This approach uncovered gaps and contradictions in the old implementation — and fixed them.

You get a system that’s correct **by design**, not just by matching outputs.  
> (You can't fix a black box by building a newer black box.)
## 🚀 What We Delivered (In Just 8 Weeks)

- ✅ Fully digitised Aged Pension Act (2015–present rules)
- 🔁 Reusable rules across multiple benefit types (e.g. DSP)
- ⚖️ 100% accuracy in comparison testing with legacy system
- 📄 Detailed audit trail for every decision
- 💬 Explanations in natural language for why a person receives (or doesn’t receive) an entitlement
- ⚡ Sub-500ms processing time in production-like environments

All delivered with a tiny team of 3 engineers on our side, and 3 SME's on the Governments. 

> “This is actually better than the old mainframe. It doesn't just get the same answer — it shows you how.”  
> – Senior Policy Analyst, Government (via project feedback)

## ✍️ How the Rules Are Written

At the heart of our platform is a powerful but deceptively simple idea:

> **Rules should be written in natural language.**

In Decisively, rules are authored in plain English, in a structure that mirrors legislation — then compiled into a decision graph that can be executed, tested, and traced. For example:

```text
The individual is qualified for an age pension if:
  - They have reached pension age
  - They have at least 10 years of qualifying Australian residence
```  
This means:

* Policy experts can read and understand the rules directly
* Complex interactions between rules become visible and manageable
* The system is fast, auditable, and version-controlled — just like code, but human-friendly

Want to see what this looks like in action?
[📎 Check out the residency requirement scenario](docs/residency-example.md)

## 🤖 Why AI Alone Won’t Fix This

You could throw GPT at your COBOL and hope it works. But here’s the thing:

>GPT might reproduce your bugs — it won’t find your logic.

AI might be able to parse COBOL.  
It can’t explain **why** someone is eligible for a benefit — or ensure that logic matches the law.

We’ve seen this firsthand. In one part of the legislation, we discovered that the legacy mainframe was making entitlement decisions based on logic that wasn’t written anywhere — not in the documentation, not in the code we could access, and not in any test data.

It took modelling the legislation, interpreting the policy, and working closely with subject matter experts to reverse engineer what the mainframe must have been doing. And even then, we found the logic was:

* Dependent on time-based changes to a person’s circumstances
* Sensitive to interactions between individuals (e.g. partners’ entitlements)
* Encoded in a way that even the owning agency couldn’t fully explain

AI might be able to parse COBOL. It can’t understand how entitlements evolve through time, or how one rule affects another across weeks, months, or decades.

That’s why we built a temporal engine, designed from day one to calculate rules over time — because real-life eligibility is rarely a single moment.

[📎 Read more about why AI can’t fix legacy logic](docs/why-ai-fails.md)

## 🏗️ Architecture At a Glance

The Decisively platform — built by Imminently — powers this entire approach. Key components:

- **Rule Compiler**: Converts natural language rules into executable logic
- **Rule Graph**: A visual, inspectable logic model linked to legislation
- **Decision API**: Accepts requests and returns decisions + detailed audit trail
- **Interview & SDK**: Optional UI tools to walk users through questions
- **Streaming Audit Engine**: For downstream systems to consume decisions

📎 [See the full architecture](docs/architecture-overview.md)

## 🎯 What This Repo Includes

- 📘 Background & project summary ([docs/approach-methodology.md](docs/approach-methodology.md))
- 🧱 Architecture & integration diagrams ([docs/architecture-overview.md](docs/architecture-overview.md))
- 📷 Screenshots of tools, UI, and audit reports ([docs/screenshots](docs/screenshots))
- 🔎 Example audit output ([docs/audit-trail-sample.md](docs/sample.decision.report.json))
- 📋 Example rules ([docs/residency-example.md](docs/residency-example.md))
- 🧩 How our rule graph works ([docs/rule-graph-explainer.md](docs/rule-graph-explainer.md))

## 💡 Who Should Read This?

- Engineers tasked with rebuilding Social Security codebases
- Public policy analysts seeking a more transparent system
- Tech leads exploring rule engines and explainable automation
- Anyone trying to modernise legacy decision systems the *right* way

## ✉️ Talk To Us

We’re Imminently — builders of Decisively, a platform for digitising rules and decisions at enterprise scale.

This repo is just a blueprint. The real opportunity is adapting this model to your context.

If you're exploring how to:
- Modernise a legacy codebase with explainability
- Bring legislation, tech, and SMEs into one loop
- Build something better than just another rules engine

📬 [Let’s chat](mailto:info@imminently.co) — we’ll walk you through a demo, an architecture session, or just share what we learned building this in production.

---

> “Modernising welfare delivery isn't just a tech problem — it's a decision integrity problem. Start with the rules, and everything else follows.”