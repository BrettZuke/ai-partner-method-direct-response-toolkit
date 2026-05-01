# Onboarding — How to think about direct response

Five minutes here saves you a hundred hours of writing copy that doesn't convert.

---

## The single most important concept

**Direct response copy isn't writing — it's persuasion engineering.**

You're not trying to sound smart, win a literary prize, or impress your client. You're trying to move a specific reader, in a specific awareness state, to a specific action. Every word either moves them closer to that action or doesn't. Cut the ones that don't.

Translation: when you doubt a sentence, the question isn't *"is it well-written?"* — it's *"does it earn its place?"*

---

## Awareness levels — the most important diagnostic

Before you write a single word, you need to know what awareness state your reader is in. This determines **everything** — the framework, the length, the angle.

| Stage              | What they know                                  | What they need from you                          |
|--------------------|--------------------------------------------------|--------------------------------------------------|
| **Unaware**        | They don't know they have the problem.           | Education. Story. A pattern interrupt.           |
| **Problem-aware**  | They know the pain, not the solution.            | Reframe + show your unique mechanism.            |
| **Solution-aware** | They know solutions exist, comparing options.    | Why YOU. Differentiation. Proof.                 |
| **Product-aware**  | They know about your specific product.            | Push past objections. Risk reversal.             |
| **Most-aware**     | Ready to buy, just need a nudge.                  | Urgency. Scarcity. Clear CTA.                    |

Send the wrong copy to the wrong stage and your conversion drops to zero — even if the copy is well-written. Get it right, and a paragraph can outsell a 30-page sales page.

This is in `frameworks.md` as a decision tree. Memorize it.

---

## The mental model: three layers

Same pattern as the funnel and email toolkits. Once you see it, you can't unsee it.

| Layer        | What it is                                          | How often you touch it      |
|--------------|-----------------------------------------------------|------------------------------|
| **Frameworks** | The structural patterns (PAS, AIDA, BAB, PASTOR). | Rarely — these don't change. |
| **Templates**  | Skeletons for sales pages, VSLs, ads.              | Per project — pick the right one. |
| **Brief**      | This client, this audience, this offer.            | Every job.                   |

99% of your work is at the **brief** layer. Frameworks and templates do the heavy lifting.

---

## Your first piece of copy — the actual workflow

1. **Diagnose the awareness level.** Where is the reader on the chart above? If you can't answer, you don't have a brief yet — go talk to your client.

2. **Pick the framework.** See the decision tree in `frameworks.md`. Most-aware = short PAS. Unaware = long AIDA or PASTOR. Selling a transformation = BAB.

3. **Pick the format.** What asset is needed?
   - **Headline** → `swipe-headlines.md` (85 templates by category)
   - **Long-form sales page** → `templates/sales-page.md`
   - **VSL script** → `templates/vsl-script.md`
   - **Paid ad** → `templates/ads.md`
   - **Email** → use the companion repo, [email-copywriting-toolkit](https://github.com/murathancetin/email-copywriting-toolkit).

4. **Fill out the brief.**
   ```bash
   cp examples/brief.example.json my-brief.json
   ```
   Open it. Replace every field. Be specific — *"30-something fitness coaches stuck at $5k/mo"* beats *"fitness coaches"*.

5. **Generate the draft.** In Claude Code:
   > *"Write me a long-form sales page using `my-brief.json`."*
   Claude reads the brief, follows the SOP, applies the right framework, and produces a draft.

6. **Edit for voice.** AI gets you to 80%. The last 20% is making it sound like *your client*. Read every line out loud — if it sounds like a generic guru, rewrite it shorter and more specific.

7. **Run the QA checklist** in `SOP.md`. The biggest killers: passive voice, vague claims, multiple CTAs, banned opening phrases ("In today's world...").

8. **Test.** Test headlines especially. Two-variant tests on traffic — let the data tell you which version works. Direct response is a measurement game, not an opinion game.

---

## The four frameworks (90-second version)

You'll use these in 95% of copy.

| Framework | When                                          | Structure                                            |
|-----------|-----------------------------------------------|------------------------------------------------------|
| **PAS**   | They're aware of the pain                     | **P**roblem → **A**gitate → **S**olution             |
| **AIDA**  | Cold or unaware audience                       | **A**ttention → **I**nterest → **D**esire → **A**ction |
| **BAB**   | Selling a transformation                      | **B**efore → **A**fter → **B**ridge                  |
| **PASTOR**| Long-form sales pages, big-ticket offers      | **P**roblem → **A**mplify → **S**tory → **T**ransformation → **O**ffer → **R**esponse |

Full breakdown in `frameworks.md`.

---

## Voice — the thing that separates pros from amateurs

Most beginner copy fails not because the structure is wrong but because it sounds like every other piece of beginner copy.

Three rules that fix 80% of voice problems:

### 1. Conversational authority

Write like you're explaining something to a smart friend over coffee. Confident, but not arrogant. Direct, but not harsh. Helpful, but not pushy.

### 2. Specific over vague

> *"Most people see results."* ← garbage
>
> *"77.6% of clients hit their first $10k month within 90 days."* ← copy

Numbers, names, timeframes, locations — these are credibility. Adjectives are noise.

### 3. The corporate filter test

If a sentence sounds like it came from a press release, rewrite it as if you're sending a 1-on-1 email to a friend. Cut "synergy", "leverage", "unlock", "revolutionize", "seamless" — and watch the copy improve.

Full voice rules in `voice-and-constraints.md`.

---

## What kills conversions (the short list)

| Mistake                                       | Why it kills                                              |
|-----------------------------------------------|-----------------------------------------------------------|
| Multiple CTAs                                 | Splits attention. One clear action wins.                  |
| Passive voice                                 | Sounds weak. "We deliver results" not "Results are delivered." |
| Banned openers like "In today's world..."     | Reader tunes out in the first 3 seconds.                  |
| Feature dumps with no benefits                | Readers don't care what it *is*. They care what it *does for them*. |
| Vague claims ("amazing results!")             | No conversion. Specifics convert.                          |
| Reading level above 6th grade                 | Mobile readers bounce. Hemingway-simple wins.             |
| Long paragraphs (>3 sentences)                | Visual overwhelm. Whitespace is your friend.               |

Full list in `SOP.md` → "Common Mistakes."

---

## What's next

- [`SETUP.md`](SETUP.md) — get Claude Code installed.
- [`SOP.md`](SOP.md) — the deep reference. Read it once, refer back forever.
- [`frameworks.md`](frameworks.md) — when to use which structure.
- [`swipe-headlines.md`](swipe-headlines.md) — 85 headline templates. Open this first when you're stuck on a headline.
- [`templates/`](templates/) — pick a template (sales page, VSL, or ad) and start writing.

The fastest way to learn this is to ship one piece. Pick the easiest scenario you have right now and go.
