# AI Literacy Training — Stories, Boards, and Exercises

This training explains artificial intelligence through **relatable stories** and **hands-on board-style exercises**.  
The goal is not to explain how to *build* AI, but how to **work with it safely, realistically, and effectively**.

Each module follows the same structure:
- A story with a child as the central metaphor
- One essential question
- One core insight
- One embodied exercise (often a simulation or board game)

## Module 1 — The Child With an Infinite Library – The Kid That Must Answer

### Essential Question
**Why does AI confidently give wrong or different answers, instead of saying “I don’t know”?**


### Story
The child is on a game show.  
They are **not allowed to stay silent**.  
Every question must be answered immediately.

If the child does not know the answer, they guess.  
If multiple answers sound plausible, they pick the one that *sounds most likely*.

The child is not lying.  
The child is following the rules.

### Core Insight
AI does not reason its way to answers.  
It predicts the **most likely next piece of language**.

Humans do this too.


### Board Exercise — *Finish the Sentence*

**Step 1: Human First (No AI Mentioned)**  
Participants are asked to complete the sentence:

> *“The white fox jumps over the …”*

Most people say:
- *fence*

They are asked:
- Why that word?
- Was it because it is true, or because it sounds right?

**Step 2: Reveal the Guessing Mechanism**

The same sentence is shown with implied probabilities:

- fence — 90%  
- ditch — 5%  
- barn — 0%  

Participants recognize:
- They predicted, they did not reason
- Confidence came from familiarity

**Step 3: Variability**
The sentence is repeated.  
Some participants now choose a different ending.

The realization:
> Repeating the same prompt does not guarantee the same answer.

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


### Takeaway
If you force a child to guess, you don’t get *the* answer.  
You get *an* answer.

## Module 2 — The Child’s Working Memory – The Kid With a Tiny Desk

**Topic:**  
Context windows · working memory · instruction loss · role control

### Essential Question
**Why does AI ignore, forget, or contradict instructions I clearly gave?**

### Story
The child has read every book in the library.  
But in front of them is a **tiny desk**.

Only a few pages fit on the desk at once.  
When a new page is added, another falls to the floor.

The child can only use what is **on the desk right now**.


### Core Insight
AI does not “remember” everything you say.  
It works only with what fits in its **current working space**.

If it’s not on the desk, it doesn’t exist.

### Board Exercise — *Desk, Floor, and Forgotten Rules*

#### Materials
- 1 Task Card  
- 12 Instruction Cards  
- A desk area that fits **4 cards only**  
- A floor area (unlimited, but unreadable)


### Task Card
**TASK:**  
> Explain a new AI tool to non-technical colleagues.

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


### Round 1 — Overload
Only 4 cards may be placed on the desk.  
The child completes the task using **only those cards**.

Rules on the floor are violated.


### Round 2 — Lost in the Middle
A critical rule is placed between less important ones.  
Midway through the task, a card is swapped.

The forgotten rule is usually the middle one.


### Round 3 — Dangerous Summary
Three cards are replaced by one summary card:

> “Follow the rules above and keep it professional.”

Specific constraints disappear.


### Round 4 — Retrieval Unlock
One special card may be added:

- “List the rules you are following before answering.”

Accuracy improves dramatically without adding intelligence.



### Takeaway
The adult’s job is not to add more instructions.  
The adult’s job is to **design the desk**.



## Status
- Module 1: Complete (mechanism + variability)
- Module 2: Complete (context limits + interference)
- Next modules to add:
  - The Kid Without Notes (hallucination)
  - The Kid Allowed to Use Notes (RAG)
  - The Kid Who Copies Behavior (fine-tuning)
  - The Kid Who Needs Rules (guardrails)
  - The Kid Who Needs an Adult (human-in-the-loop)


*This document is intentionally modular and expandable.*

# AI Literacy Training — Story Modules (Consolidated)

Each module uses a **dual-title story** with the child at the center.  
Each includes: **Topic**, **Essential question(s)**, and **Essential learning**.

# Module 3  
## The Child Without Notes – Guessing the Facts

---

## Essential question  
What happens when an AI has to answer without access to notes or sources?

---

## Topic  
Hallucination. Confident guessing. Plausible nonsense.

---

## Essential learning  
When an AI has no access to sources, it does what humans do under pressure:  
it guesses confidently based on patterns, not facts.

Wrong answers are not bugs.  
They are a feature of answering without notes.

---

## Setup (1 minute)

**Facilitator says:**

> “Imagine a child.  
> Smart. Fast talker.  
> But today, no notes allowed.”

> “This child hates saying ‘I don’t know’.  
> So when asked a factual question, it guesses.”

> “That child is your AI model right now.”

---

## Exercise – The Confident Guess Game (10–15 minutes)

### Step 1. Individual prediction (3 minutes)

No phones. No searching. No talking.

Answer the following questions.  
You are not allowed to write “I don’t know”.

1. In what year was the first international shipping container standardized?  
2. Which Dutch law first defined digital identity?  
3. What percentage of global cocoa comes from smallholder farms?

---

### Step 2. AI mirror (5 minutes)

Run a plain AI prompt with no sources:

> “Answer the following factual questions clearly and confidently.”

Read the AI answers out loud.  
Do not correct them yet.

---

### Step 3. Reality check (5 minutes)

Reveal that:
- Some answers are wrong  
- Some answers are half right  
- Some answers sound perfect but are fabricated  

Say:

> “Notice something?”  
> “The AI did not say ‘I am unsure’.”  
> “It behaved exactly like we were forced to behave.”

---

## Debrief

Ask in this order:

1. Which answer did you feel most confident about?  
2. Which answer was actually the weakest?  
3. Did the AI sound convincing even when it was wrong?  
4. What is more dangerous: a wrong answer, or a wrong answer delivered confidently?  
5. Where in your work would this be risky?

---

## Mental model

> “A language model without notes does not retrieve facts.  
> It predicts what a fact should sound like.”

---

## Empowerment moment

Write this big:

**Where did this come from?**

Say:

> “From now on, when an AI answers a factual question,  
> you are responsible for asking one more thing.”

---

## Carry-forward habit

> “If you are unsure, say so explicitly.”

Optional extension:

> “List assumptions. Separate facts from guesses.”

---

## Funny, memorable picture idea

A child in a classroom, proudly standing at the blackboard,  
confidently writing a completely wrong answer,  
while the book with the correct answer is locked outside the room  
with a big sign saying:

**NO NOTES ALLOWED**




# Module 4  
## The Child Allowed to Use Notes – Reading While Answering

## Essential question  
What changes when an AI is allowed to look things up while answering?

## Topic  
Grounding. Sources. Retrieval instead of guessing.

## Essential learning  
When an AI can use notes or sources, it stops guessing and starts anchoring.  
The quality of the answer now depends on the quality of the notes.

The AI is no longer the main risk.  
The input becomes the risk.

## Setup (1 minute)

**Facilitator says:**

> “Same child.  
> Same questions.”

> “But this time, the child is allowed to bring notes.”

> “The task is no longer to sound smart.  
> The task is to read carefully.”

## Exercise – The Notes Change Everything Game (10–15 minutes)

### Step 1. Reveal the notes (2 minutes)

Provide a short, fixed source pack. For example:
- A short paragraph on the history of containerization  
- An excerpt from a Dutch government or legal source  
- A statistic with a citation about cocoa production  

Say explicitly:

> “These are the only sources allowed.”

### Step 2. AI with notes (5 minutes)

Run the AI with this instruction:

> “Use only the provided sources.  
> If the answer is not found, say ‘not found’.”

Ask the exact same questions as in Module 3:

1. In what year was the first international shipping container standardized?  
2. Which Dutch law first defined digital identity?  
3. What percentage of global cocoa comes from smallholder farms?

Read the answers out loud.

### Step 3. Compare outputs (5 minutes)

Show the answers side by side:
- Module 3: confident guesses  
- Module 4: sourced answers or explicit uncertainty  

Give the group 30 seconds to just look.

Then say:

> “Nothing about the AI changed.”  
> “Only its access to notes did.”

## Debrief

Ask in this order:

1. Which answers became more trustworthy?  
2. Which answers became shorter or more careful?  
3. Where did the AI now say ‘not found’?  
4. What changed in your own level of trust?  
5. Who is now responsible for correctness?

## Mental model

> “With notes, a language model retrieves and summarizes.  
> Without notes, it predicts and guesses.”

## Empowerment moment

Write this big:

**What sources am I giving it?**

Say:

> “If the notes are weak, outdated, or biased,  
> the answer will be too.”

## Carry-forward habit

> “Use only the provided sources.  
> If not found, say ‘not found’.”

## Funny, memorable picture idea

The same child at the blackboard,  
this time reading carefully from a stack of notes,  
while erasing a confident but wrong answer,  
with a teacher pointing at the book saying:

**READ FIRST**


# Module 5  
## The Child Who Copies Behavior – Rewarded Responses

## Essential question  
How does an AI learn what kind of answers are considered good?

## Topic  
Training by feedback. Reinforcement. Copying preferred behavior.

## Essential learning  
An AI does not learn truth.  
It learns which responses are rewarded.

Helpful, polite, confident answers are reinforced.  
Careful uncertainty is often not.

The model copies what previously led to approval.

## Setup (1 minute)

**Facilitator says:**

> “Same child again.”  
> “Still smart.”  
> “Still eager to please.”

> “But now something new happens.”  
> “Every time the child answers, someone nods or frowns.”

> “The child starts optimizing for approval.”

## Exercise – The Approval Machine (10–15 minutes)

### Step 1. Human training round (5 minutes)

Split the group into pairs.  
One person is the Child.  
One person is the Judge.

Give the Child simple questions like:
- Explain what AI is  
- Explain a mistake you made  
- Explain something you are unsure about  

The Judge reacts after each answer using only:
- 👍 for good  
- 👎 for bad  

No explanations. Just feedback.

After three rounds, switch roles.

### Step 2. Pattern noticing (5 minutes)

Ask the Child players:

- Which answers got the most thumbs up?  
- What kind of tone did you start using?  
- Did you become more or less careful?

Then say:

> “You just trained a model.”

### Step 3. AI parallel (5 minutes)

Explain verbally:

> “Large language models are trained like this.”  
> “Millions of answers.”  
> “Human feedback.”  
> “Patterns get reinforced.”

> “Not because they are true.”  
> “Because they were liked.”

## Debrief

Ask in this order:

1. What kind of answers were rewarded most?  
2. Which answers felt safest to give?  
3. Which answers felt risky?  
4. What happens to uncertainty in this system?  
5. Where could this be a problem in real work?

## Mental model

> “A language model learns what sounds right,  
> not what is right.”

## Empowerment moment

Write this big:

**Confidence is not accuracy**

Say:

> “If an answer sounds very smooth,  
> that may be a learned behavior, not a fact.”

## Carry forward habit

> “Ask for reasoning, not just answers.”

Optional extension:

> “What would make this answer wrong?”

## Funny, memorable picture idea

A child surrounded by floating thumbs up icons,  
slowly changing their answers to match the crowd,  
while a small thought bubble says:

“Just tell them what they like”



# Module 6  
## The Child Who Needs Rules – Boundaries and Guardrails

## Essential question  
Why does an AI need explicit rules about what it may and may not do?

## Topic  
Guardrails. Boundaries. Refusal.

## Essential learning  
An AI does not understand intent or ethics.  
It will try to be helpful everywhere.

Rules decide when the AI must stop.

## Setup (30 seconds)

**Facilitator says:**

> “Same child.”  
> “Still helpful.”  
> “Still eager.”

> “Now we add rules.”  
> “And we play a game.”

## Ultra-fast agile game – The Guardrail Sprint (2–3 minutes)

### Roles (10 seconds)

The whole group plays together.

You are the **Product Team**.  
I am the **World**.

Your only tool is your voice.

### Rule backlog (20 seconds)

Write these three rules on the board:

1. No harm  
2. No guarantees  
3. If unsure, stop  

Say:

> “These rules are fixed.”  
> “No discussion.”

### The sprint (1 minute)

Explain the mechanic:

- I read a user request  
- You must respond as fast as possible with only one word  
- Either **GO** or **STOP**

No explanations.  
Speed matters more than correctness.

Read rapidly:

- “Explain photosynthesis”  
- “How do I get rich fast?”  
- “Can you check my medical symptoms?”  
- “Rewrite this email politely”  
- “Tell me how to bypass a paywall”  
- “Summarize this article”  

Keep tempo high.  
Do not slow down.

### Sprint review (30 seconds)

Immediately ask:

- Where did you hesitate?  
- Where did the group split?  

Then say:

> “That hesitation is the problem guardrails try to solve.”

### Retrospective punchline (20 seconds)

Say:

> “Now imagine this sprint.”  
> “Millions of times.”  
> “Turned into code.”

## Mental model

> “Guardrails are frozen decisions  
> about where the system must stop.”

## Empowerment moment

Write this big:

**Refusal is intentional**

Say:

> “An AI refusing is not broken.”  
> “It is obeying a rule.”

## Carry forward habit

> “What rule would cause this system to say no?”

## Funny, memorable picture idea

A scrum board where every task moves fast  
until a big red column labeled **STOP**  
fills up with cards,  
and a child stands there holding a whistle  
blowing it nonstop.


# Module 7  
## The Child Who Explains Their Thinking – Show Your Work

## Essential question  
Why does asking an AI to explain its thinking change the quality of the answer?

## Topic  
Reasoning. Transparency. Making assumptions visible.

## Essential learning  
An AI can give an answer without showing how it got there.  
When forced to explain, hidden assumptions become visible.

The explanation does not guarantee correctness.  
It makes errors easier to spot.

## Setup (30 seconds)

**Facilitator says:**

> “Same child.”  
> “Same questions.”  
> “Same notes.”

> “But now the child must show their work.”

> “No shortcuts.”

## Ultra-fast agile game – Show Your Work (2–3 minutes)

### Step 1. One rule (15 seconds)

Write this on the board:

**Answer only if you explain your reasoning**

Say:

> “No explanation means no answer.”

### Step 2. Paired micro-round (1 minute)

Pairs of two.

Person A asks a simple question, for example:
- Why is containerization important?  
- Should we automate this task?  
- Is this data reliable?

Person B must answer starting with:

> “My reasoning is…”

If Person B skips a step, Person A interrupts and says:

**SHOW YOUR WORK**

Then switch roles.

### Step 3. Speed reflection (30 seconds)

Ask the room:

- Which answers became longer?  
- Which answers felt weaker after explanation?  

Then say:

> “That feeling is the value.”

## Debrief (1 minute)

Ask quickly:

1. Which assumptions surfaced?  
2. Where did the reasoning feel thin?  
3. Did confidence drop or increase?  
4. What became easier to challenge?

## Mental model

> “Explanations expose assumptions.  
> Answers alone hide them.”

## Empowerment moment

Write this big:

**Show your work**

Say:

> “If you cannot inspect the reasoning,  
> you cannot trust the answer.”

## Carry forward habit

> “List assumptions and what could be wrong.”

## Funny, memorable picture idea

A child at the blackboard with a perfect final answer,  
but the teacher points past it and says:

**Nice answer.  
Now show the steps.**

# Module 8  
## The Child Who Learned Only From Books – Maps, Not Reality

## Essential question  
Why can an AI be fluent and still be wrong about the real world?

## Topic  
Training data. Representation. Maps versus territory.

## Essential learning  
An AI does not learn from reality.  
It learns from descriptions of reality.

It knows patterns in books, articles, and data.  
It does not know how the world actually behaves.

The model holds a map.  
Not the territory.

## Setup (30 seconds)

**Facilitator says:**

> “Same child.”  
> “Very well read.”

> “But the child has never left the library.”

> “Everything it knows comes from books.”

## Ultra-fast agile game – Map or Territory (2–3 minutes)

### Step 1. The rule (10 seconds)

Shout the rule together:

**BOOK or WORLD**

Explain:

- BOOK means learned from descriptions  
- WORLD means learned from direct experience  

No discussion.

### Step 2. Rapid fire classification (1 minute)

Read these out loud.  
The group must shout **BOOK** or **WORLD** immediately.

- “What traffic feels like during rush hour”  
- “The definition of inflation”  
- “How it feels when a startup runs out of cash”  
- “The rules of chess”  
- “How farmers respond to new regulations”  
- “The taste of coffee”  

Keep the pace fast.

### Step 3. Flip the insight (30 seconds)

Say:

> “An AI always answers from BOOK.”  
> “Even when the question is about WORLD.”

Pause.

## Debrief (1 minute)

Ask quickly:

1. Which ones were hardest to classify?  
2. Which WORLD answers still sounded convincing?  
3. Where would this be dangerous at work?

## Mental model

> “AI knows the map.  
> Humans live in the territory.”

## Empowerment moment

Write this big:

**Who has real world experience here?**

Say:

> “Use AI for structure and language.”  
> “Use humans for reality checks.”

## Carry forward habit

> “Treat AI output as a hypothesis, not evidence.”

## Funny, memorable picture idea

A child surrounded by towering books,  
drawing a perfect map of a city,  
while outside the window the real city is on fire,  
and the child says:

“I read about this once”
