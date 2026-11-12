# 1st-Century Contextual Framework

*Studying the biblical texts through a thought-for-thought apostolic lens, 30–95 AD.*

The 1st-Century Contextual Framework is a set of five Markdown documents that guide an AI model to read Scripture the way its first hearers heard it. It holds the model to the Greek and Hebrew text in its own literary and historical setting, treats lexicons and commentaries as proposals to be tested rather than authorities, and sets aside the systematic theology, creeds, and transactional frameworks that came after 95 AD. What comes out is warm, plain-English teaching for an ordinary reader today, built step by step and checked by a human at every gate.

**Who it is for**

- Bible students, teachers, and small-group leaders who want AI-assisted study that stays with the text instead of drifting into whatever most commentaries say.
- Anyone who wants to test a first-century, text-first reading of Scripture for themselves.
- Builders and prompt engineers interested in how a long, rule-governed document set can restrain a language model's default habits.

---

## Quick Start

1. **Download the five files** in this repository (or the latest release).
2. **Create a dedicated AI project.** Use a Project, Gem, Custom GPT, or similar workspace on the AI platform you prefer. A model with a large context window and strong reasoning works best.
3. **Load the constitution.** Put `1st-Century Contextual Framework.md` in the project's instructions. If the instructions field is too small to hold it (some platforms cap it near 12,000 characters), paste the whole file as the first message of the chat instead. The model reads it the same way.
4. **Add the other four files** as project knowledge or uploaded files: the Standing Rules, the Style Guide, the Style FewShot Examples, and the Generated Knowledge Base. The Knowledge Base is large (about 730 KB), so check your platform's file limits.
5. **Choose a mode:**
   - Just ask a question to use **Dialogue Mode**, the default.
   - Type `[ACTIVATE: Lexical Mode]` for a study of one Greek or Hebrew word or phrase.
   - Type `[ACTIVATE: Strict Mode]` to begin a full, gated exegesis of a passage (see below).
6. **Supply your English version.** The Framework compares the original-language text with whichever English translation you name when you start a chapter. If you do not name one, it uses the NASB 2020.

**A note on the full workflow.** Version 10.0 is written for agentic production: an orchestrating AI builds each worker a written, verified packet of inputs from the live files, while the human approves every gate. That orchestration tooling is not part of this repository. The five files still govern every stage, so you can study in Dialogue or Lexical Mode, walk the gated stages by hand in your own project, or review the Framework document by document.

---

## The Files

| File | Purpose | Version |
|---|---|---|
| `1st-Century Contextual Framework.md` | The constitution: the 30–95 AD interpretation rules, operational modes, the gated three-stage protocol, Integration, and the voice and layout mandates. | v10.0 |
| `Framework Standing Rules.md` | The execution keeper: how each stage and Integration applies the constitution, with every rule tagged by who it governs. | 11-12-2026 |
| `Exegesis Style and Format Guide.md` | Tone, voice, page structure, and the required model for a Published Exegesis page, including the three registers of exegesis, witness, and exposition. | 11-12-2026 |
| `Style Guidelines FewShot Examples.md` | Short worked examples that calibrate the warm, eye-level teaching voice, pronoun choice, and family vocabulary. | 11-10-2026 |
| `Generated Knowledge Base.md` | A closure log of first-century word and concept entries, each with its claim, verse chain, settled close, honesty clause, and rival chain answered. | 11-12-2026 |

---

## How an Exegesis Runs

Full exegesis is triggered with `[ACTIVATE: Strict Mode]`. The AI is never allowed to produce a whole passage in one response. It works through three exegesis stages and then Integration, and it halts at four human gates for your approval and conversation. Even in an agentic setup, the stages are never run unattended in a single batch.

**Stage 1: Structural Outline.** From the original-language text (NA28 Greek for the New Testament; BHS, BHQ, or LHB Hebrew for the Old), the AI writes a deliberately broad structural outline of the passage and divides the chapter into 2-verse Processing Groups. Where a group boundary cuts a continuous sentence, the neighboring groups are tagged so each one can still see its whole sentence. *Gate 1: you approve the outline and the group table.*

**Stage 2: Linguistic Audit.** Each group is audited on its own. Part A lists every place the supplied English version shifts, smooths, inflates, or flattens the Greek or Hebrew. Part B gives targeted word meanings for every flagged word, citing the dictionary's own classification and verse assignment and keeping genuine first-century forks open. Key household words and Knowledge Base entries force their own entries. *Gate 2: you review the audits and any open questions.*

**Stage 3: Progressive Teaching.** For each group, the AI first writes a single plain-English paragraph, **What it says**, saying what a first-century hearer would have understood, and stops for you to accept or amend it. Then it drafts the teaching, with Translation Barriers for heavily loaded terms, drawing on the book already read but nothing from outside it. When you approve, that piece becomes the **Group file**. *Gate 3: you shape and approve each group.*

**Integration.** Integration is collaborative work after the three stages, not a fourth stage. The AI assembles the approved Group files onto the Stage 1 frame as one **Working Draft**, writes a fresh Apostolic Lens, dissolves the seams between groups, and checks every boundary across the chapter. Then it talks the draft through with you: testing cross-book **Unbroken Witness** passages against the original language, and shaping any labeled **Alongside this** units that carry what the teacher hears. *Gate 4: the Integration dialogue.*

**The Published Exegesis.** The finished, titled Working Draft is the Published Exegesis. On the page, exegesis (what the text says), witness (what Scripture says elsewhere), and exposition (what the teacher hears, always labeled) stay distinct, so the reader always knows which one is speaking.

---

## Why This Exists

I built this Framework because I believed the assertions within it, and I wanted to test them: is a first-century, text-first, union-based perspective what the Scriptures themselves bear out? I use a large language model not as a source of wisdom, but as a lexical dot-connector.

### The problem: consensus orthodoxy

Language models are trained on the aggregate text of humanity. When it comes to the Bible, most of that text is commentaries, sermons, and systematic theologies from the last five centuries. Left alone, a model drifts toward that "majority report," which includes:

- **Commercial or transactional logic,** treating salvation as a literal financial exchange.
- **Post-95 AD frameworks,** reading a first-century letter through Reformation or medieval satisfaction theories.
- **Clinical, analytical language** in place of the organic, relational vocabulary the apostles used.

The subtler danger is the **illusion of compliance.** Tell a model to "sound first-century" and it will adopt the vocabulary (redemption, propitiation, flesh) while quietly carrying its default modern logic underneath. The words look right, but the underlying spiritual mechanics are anachronistic.

### The approach: a clean room

A language model predicts text from probabilities. This Framework deliberately narrows that probability space. It works as an operational boundary that keeps the model with the Greek, Hebrew, and Aramaic text and the historical realities of 30–95 AD, and away from later consensus. Its exclusions are guardrails, not censorship:

1. **Unaltered consistency.** God's Word does not contradict itself, so no interpretation of one verse may render another untrue. The model has to harmonize the text as written instead of reaching for later theological shortcuts.
2. **Counteracting drift.** The rules pull the model off the broad path of internet consensus and back to the apostolic text.
3. **Avoiding historical shortcuts.** Vocabulary invented later to resolve apparent tensions often redefines the original words. Leaving it out keeps centuries of outside baggage out of the study.

### What I have found

When those blinders come off, the model's reading keeps arriving at the reality of the Father's household and the believer's unbroken union with the Son. You are welcome to use the Framework and test the text for yourself.

---

## Common Questions

- **"This feels restrictive."** Some friction at first is normal. The exclusions are defensive. Like a water filter, they do not take away the water; they remove the sediment.
- **"Does this argue for a denomination?"** No. The Framework does not argue for or against any modern theological view. It enforces one axiom: the text must agree with itself.
- **"Will it work on my AI model?"** It relies on written rules and careful context management, not model-specific code. Models with strong reasoning and large context windows follow the gates and halts most faithfully.
- **"How should I check the output?"** Hold it against the files. Did the AI let the passages stand together, each true at its own place, or did it slip in a modern theological shortcut?

---

## Changelog

See [CHANGELOG.md](CHANGELOG.md) for what changed in each version.

## License

This work is licensed under the [Creative Commons Attribution-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-sa/4.0/) (CC BY-SA 4.0). See [LICENSE](LICENSE).

It is offered freely as a gift. You may use, share, and adapt it, including in paid teaching or ministry work, as long as you credit the author and release any adapted version you share under the same license, so it stays free for the next person.
