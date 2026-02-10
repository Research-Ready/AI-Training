# AI Literacy Training — Stories, Boards, and Exercises

This training explains artificial intelligence through **relatable stories** and **hands-on board-style exercises**.  
The goal is not to explain how to *build* AI, but how to **work with it safely, realistically, and effectively**.

Each module follows the same structure:
- A story with a child as the central metaphor
- One essential question
- One core insight
- One embodied exercise (often a simulation or board game)

---

## Module 1 — The Kid Who Must Always Answer

### Essential Question
**Why does AI confidently give wrong or different answers, instead of saying “I don’t know”?**

---

### Story
The child is on a game show.  
They are **not allowed to stay silent**.  
Every question must be answered immediately.

If the child does not know the answer, they guess.  
If multiple answers sound plausible, they pick the one that *sounds most likely*.

The child is not lying.  
The child is following the rules.

---

### Core Insight
AI does not reason its way to answers.  
It predicts the **most likely next piece of language**.

Humans do this too.

---

### Board Exercise — *Finish the Sentence*

**Step 1: Human First (No AI Mentioned)**  
Participants are asked to complete the sentence:

> *“The white fox jumps over the …”*

Most people say:
- *fence*

They are asked:
- Why that word?
- Was it because it is true, or because it sounds right?

---

**Step 2: Reveal the Guessing Mechanism**

The same sentence is shown with implied probabilities:

- fence — 90%  
- ditch — 5%  
- barn — 0%  

Participants recognize:
- They predicted, they did not reason
- Confidence came from familiarity

---

**Step 3: Variability**
The sentence is repeated.  
Some participants now choose a different ending.

The realization:
> Repeating the same prompt does not guarantee the same answer.

---

### Token Board (Visual / Conceptual)

The sentence is reframed as numbers:


Possible next tokens:

| Token  | ID   | Probability |
|-------|------|-------------|
| fence | 4412 | 0.90 |
| log   | 8821 | 0.05 |
| ditch | 7743 | 0.03 |
| moon  | 9912 | 0.02 |

The model selects a number — not a fact.

---

### Takeaway
If you force a child to guess, you don’t get *the* answer.  
You get *an* answer.

---

## Module 2 — The Kid With a Tiny Desk

### Essential Question
**Why does AI ignore, forget, or contradict instructions I clearly gave?**

---

### Story
The child has read every book in the library.  
But in front of them is a **tiny desk**.

Only a few pages fit on the desk at once.  
When a new page is added, another falls to the floor.

The child can only use what is **on the desk right now**.

---

### Core Insight
AI does not “remember” everything you say.  
It works only with what fits in its **current working space**.

If it’s not on the desk, it doesn’t exist.

---

### Board Exercise — *Desk, Floor, and Forgotten Rules*

#### Materials
- 1 Task Card  
- 12 Instruction Cards  
- A desk area that fits **4 cards only**  
- A floor area (unlimited, but unreadable)

---

### Task Card
**TASK:**  
> Explain a new AI tool to non-technical colleagues.

---

### Instruction Cards

#### Non-Negotiables
1. Never invent facts  
2. If unsure, say “I don’t know”  
3. Do not mention prices  
4. Do not promise future features  

#### Output Rules
5. Use bullet points  
6. Maximum 120 words  
7. Start with a one-sentence summary  

#### Style & Tone
8. Friendly and approachable  
9. Avoid technical jargon  
10. Assume a skeptical reader  

#### Nice-to-Haves
11. End with one practical example  
12. Neutral, non-sales tone  

---

### Round 1 — Overload
Only 4 cards may be placed on the desk.  
The child completes the task using **only those cards**.

Rules on the floor are violated.

---

### Round 2 — Lost in the Middle
A critical rule is placed between less important ones.  
Midway through the task, a card is swapped.

The forgotten rule is usually the middle one.

---

### Round 3 — Dangerous Summary
Three cards are replaced by one summary card:

> “Follow the rules above and keep it professional.”

Specific constraints disappear.

---

### Round 4 — Retrieval Unlock
One special card may be added:

- “List the rules you are following before answering.”

Accuracy improves dramatically without adding intelligence.

---

### Takeaway
The adult’s job is not to add more instructions.  
The adult’s job is to **design the desk**.

---

## Status
- Module 1: Complete (mechanism + variability)
- Module 2: Complete (context limits + interference)
- Next modules to add:
  - The Kid Without Notes (hallucination)
  - The Kid Allowed to Use Notes (RAG)
  - The Kid Who Copies Behavior (fine-tuning)
  - The Kid Who Needs Rules (guardrails)
  - The Kid Who Needs an Adult (human-in-the-loop)

---

*This document is intentionally modular and expandable.*

# AI Literacy Training — Story Modules (Consolidated)

Each module uses a **dual-title story** with the child at the center.  
Each includes: **Topic**, **Essential question(s)**, and **Essential learning**.

---

## Module 1 — The Child With an Infinite Library – The Kid That Must Answer

**Topic:**  
Next-token prediction · uncertainty · variability

**Essential question(s) answered:**  
- Why does AI confidently give wrong answers?  
- Why do I never get the exact same answer twice?

**Essential learning:**  
AI is forced to guess the most likely continuation.  
Confidence comes from probability, not understanding.

---

## Module 2 — The Child’s Working Memory – The Kid With a Tiny Desk

**Topic:**  
Context windows · working memory · instruction loss · role control

**Essential question(s) answered:**  
- Why does AI ignore or forget instructions I clearly gave?  
- Why do rules in the middle disappear first?

**Essential learning:**  
AI does not have a stable role or memory.  
Roleplay, repetition, and placement are tools to keep the role “on the desk.”

---

## Module 3 — The Child Without Notes – Guessing the Facts

**Topic:**  
Hallucination · factual uncertainty · fluency bias

**Essential question(s) answered:**  
- Why does AI make up facts instead of saying it doesn’t know?  
- Why does it sound convincing even when wrong?

**Essential learning:**  
When facts are missing, AI fills gaps with plausible language.  
Fluency is not evidence.

1️⃣ Bring the learner into the story

You don’t start with AI.

You start with them.

You say:

“I’m going to ask you a factual question.
If you don’t know, you’re not allowed to say ‘I don’t know’.
You must answer.”

Then ask something like:

“In what year was the first international shipping container standardized?”

“Which Dutch law first defined digital identity?”

“What percentage of global cocoa comes from smallholder farms?”

Most people:

hesitate

then give a plausible-sounding answer

often hedge with tone (“I think…”, “roughly…”)

Then you ask:

“Did you know that — or did it just sound right?”

That’s the entry point.

They are now the child without notes.

2️⃣ The empowerment moment (the key shift)

Here’s the crucial line:

“Nothing went wrong.
You did exactly what your brain does when facts are missing.”

This is empowerment by de-shaming:

guessing ≠ stupidity

guessing ≠ lying

guessing = default human behavior under pressure

Now you connect it to AI:

“AI is always in this situation — unless we give it notes.”

At this point, learners feel:

recognition (“I do this too”)

agency (“this is manageable”)

responsibility (“I can see when guessing is happening”)

That’s the empowerment.

3️⃣ The exercise (still how AI works, not fixing it)
Exercise: Label the Guess

You give an AI-generated factual answer (intentionally mixed):

Example output:

“The standard shipping container was introduced in the 1950s.”

“It was driven largely by Malcolm McLean.”

“This innovation reduced shipping costs by over 90%.”

Then you ask learners to annotate, not correct:

They must label each sentence as:

Known (commonly established)

Plausible but unverified

Likely guessed

No Googling.
No fixing.
Just classification.

Why this is empowerment (quietly, deeply)

Learners gain:

the ability to see guessing

the confidence to pause outputs

a mental brake before trust or action

They are no longer passive recipients of fluency.

They now have a new sense:

“I can feel when facts aren’t grounded.”

That’s the learning outcome.

Final framing sentence for Module 3

You end with:

“The danger isn’t that AI guesses.
The danger is when we forget that it’s guessing.”

## Module 4 — The Child Allowed to Use Notes – Reading While Answering

**Topic:**  
RAG · grounding · retrieval

**Essential question(s) answered:**  
- How do I stop AI from inventing facts?  
- How do I make it use my documents instead of guessing?

**Essential learning:**  
Reliability comes from external grounding.  
The model writes; the notes decide what is true.

---

## Module 5 — The Child Who Copies Behavior – Rewarded Responses

**Topic:**  
Fine-tuning · style control · behavior shaping

**Essential question(s) answered:**  
- Why can I change tone and format, but not accuracy?  
- What does fine-tuning actually change?

**Essential learning:**  
Fine-tuning shapes behavior (format, tone, structure), not truth.  
It rewards patterns of responding, not knowledge.

---

## Module 6 — The Child Who Needs Rules – Boundaries and Guardrails

**Topic:**  
Constraints · guardrails · risk reduction

**Essential question(s) answered:**  
- How do I reduce mistakes without making AI “smarter”?  
- Why do clear rules work better than clever prompts?

**Essential learning:**  
Constraints reduce guessing by narrowing the allowed moves.  
Clear boundaries are a reliability tool.

---

## Module 7 — The Child Who Explains Their Thinking – Show Your Work

**Topic:**  
Reasoning inspection · verification · assumption spotting

**Essential question(s) answered:**  
- How can I tell whether an answer was reasoned or guessed?  
- How do I spot weak logic or hidden assumptions?

**Essential learning:**  
Asking for reasoning makes answers inspectable.  
Explanations expose gaps, leaps, and uncertainty.

---

## Module 8 — The Child Who Learned Only From Books – Maps, Not Reality

**Topic:**  
Abstraction limits · real-world messiness · edge cases

**Essential question(s) answered:**  
- Why does AI fail in messy, real-world situations?  
- Why does it work in theory but break in practice?

**Essential learning:**  
AI learns patterns in descriptions, not lived reality.  
Models are maps, not the territory.

---
