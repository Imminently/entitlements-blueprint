# Why AI Can’t Modernise Legacy Welfare Systems

> “Just use AI to translate the COBOL.”  
> Sure. Then what?

AI is incredible — and yes, it might help translate a chunk of 1970s COBOL into modern code. But if you think that gets you a working, understandable, maintainable entitlements system... you’re missing the hard part.

Here’s why.

---

## 🚫 1. Porting old code = porting old problems

AI doesn’t understand what code *should* do. It just replicates what’s there.

But welfare systems contain logic that:
- Was written decades ago
- No one fully understands anymore
- May not even be valid under current legislation
- Could apply *only* to grandfathered recipients from 30 years ago

By blindly porting the logic, you're preserving:
- Outdated business rules
- Irrelevant edge-case hacks
- Misalignments with today’s law and policy

And you still don’t know what’s correct — you’ve just shifted the black box into a shinier language.

---

## 🔍 2. You can’t validate what you can’t read

Even if AI outputs code you can compile and run, you’re no better off unless someone — a policy SME, not just an engineer — can *read and understand* it.

- You won’t know if it's right
- You won’t know which rules came from which part of the law
- You won’t know how to fix it when things change

With our approach, rules are:
- Written in **natural language**
- **Linked directly** to legislation
- **Readable by non-developers**, including those who actually own the policy

That’s how we completed a complex entitlements model in just 8 weeks — with constant SME feedback and iteration.

📎 [See how our rule format works →](rule-graph-explainer.md)

---

## 🕰️ 3. Temporal logic is not optional — it’s everything

Eligibility isn’t a single calculation. It’s a timeline.

Real-world entitlements depend on:
- How long someone has lived in the country
- How their income has changed over time
- How benefit thresholds and rates have changed over time
- How their status affects (or is affected by) their partner’s status
- Whether certain rules applied to them *at the time*, based on changing law
- and more...

This isn’t something AI will infer from code. It requires a **purpose-built temporal model** — which is exactly what we built into our engine from day one.

Without temporal logic, you’ll get calculations that “look right” — until they don’t. And no way to explain why.

---

## 🕳️ 4. You’re still left with a black box

Even in a new language, your system is just as opaque as the COBOL you replaced. You can’t:
- Trace how an entitlement was determined
- Explain it to the recipient
- Prove that it matches the law

With our approach:
- Every decision includes a **human-readable audit trail**
- You get an explanation of *what* was calculated, *how*, *why*, and *where the rule came from*
- This isn’t just logging — it’s real transparency

> Our platform doesn’t just match outcomes. It explains them.

📎 [Explore a decision audit trail →](../assets/sample.decision.report.json)

---

## 👥 5. Real reform needs real people

Our system is designed so that subject matter experts — the people who understand the intent behind the law — can **read and validate** the logic themselves.

- No hidden business logic
- No dev-only domain
- No "throw it over the fence" to engineering

That’s why we were able to deliver a working, accurate engine in 8 weeks.  
It wasn’t AI. It was **collaboration**.

---

## 💸 6. AI might be cheaper — until you build the wrong thing

Yes, AI is fast and cheap.

But if it leaves you with a massive, unreadable, untrustworthy system that:
- Still doesn't reflect the legislation
- Still can’t explain itself
- Still needs to be replaced in 10 years…

…did you actually modernise?

With our approach, you:
- Build a **shared source of truth** across policy, IT, and service delivery
- Get **rules you can see, test, explain, and maintain**
- Deliver value in weeks, not years

---

## ✅ TL;DR

| AI Translation | Our Approach |
|----------------|--------------|
| Replicates old logic blindly | Rebuilds logic based on actual legislation |
| Produces new code no one can validate | Uses natural language readable by SMEs |
| Ignores time-based complexity | Built with temporal reasoning from the start |
| Creates another monolith | Creates modular, testable, explainable logic |
| Might match outcomes | Actually explains them |
| Costs less up front | Delivers real reform faster, with less risk |

---

> **Modernisation isn’t about the language. It’s about the logic.**  
> If you don’t know what the system *should* be doing, AI won’t help you build the right one.

📬 [Talk to us →](mailto:info@imminently.co)  
Or just check out the [architecture](architecture-overview.md) and [rule graph](rule-graph-explainer.md) to see for yourself.