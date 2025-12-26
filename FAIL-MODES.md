FAIL-MODES.md — Where GPTs Break (and How to Catch It)

This file is about failure modes — how things go wrong, what it looks like, and how to respond.

You’re not a bad user if you hit these.
You’re just early.

TOKEN DRIFT (CONTEXT CEILING)

What it is

Every conversation has a maximum context size (token ceiling).

When you cross it, the model:

starts dropping or compressing earlier parts of the conversation,

retains a blurred summary of “what we were doing,”

loses fine-grained constraints, decisions, and examples.

What it feels like

“It was sharp yesterday, now it’s dull.”

“It’s ignoring my rules.”

“It keeps repeating generic advice.”

You might even start inventing stories:

“Are they throttling me?”

“Is someone watching this thread?”

When almost always, the answer is:
“No, you’re just out of room.”

How to catch it

Replies get more generic.

The model forgets project-specific terms it previously used correctly.

Earlier decisions have to be re-explained.

How to respond

Don’t keep hammering the same thread.

Ask for a continuation seed (see HOW-TO-ASK).

Start a new chat with that seed.

Keep the old thread for reference and oversight.

HALLUCINATION (CONFIDENT NONSENSE)

What it is

The model:

fills in gaps with plausible-sounding detail,

especially when:

sources are missing,

you ask for specifics without providing data,

or you implicitly reward “fast answers” over “I don’t know.”

What it feels like

You get:

confident names,

dates,

citations,

specifications,

that sound right… until you check.

How to catch it

Be suspicious of:

very specific names and stats that you didn’t provide,

citations to sources you can’t find,

claims that “solve” complex issues in one paragraph.

How to respond

Ask things like:

Are you sure about these specifics?

Mark each fact as:

known (standard consensus),

inferred (reasonable but uncertain),

speculative (you’re guessing).

If you’re not sure, say so.

And:

provide your own data when you can,

never treat the model as a sole source of fact for high-stakes claims.

MODE BLEED (TONE / DOMAIN DRIFT)

What it is

You ask the model to be:

creative,

then legal,

then technical,

then jokey,

in the same thread without resetting the mode.

The styles and assumptions leak into each other.

What it feels like

Jokes in standards docs.

Legal-sounding jargon in story prose.

Overly “epic” language in technical explanations.

Emotional tone where you wanted neutral analysis.

How to catch it

Scan outputs and ask:

Does this sound like the right domain?

Is the tone consistent with the purpose?

How to respond

Explicitly reset mode:

Mode reset:

We are now in [governance / creative / technical] mode.
Tone must match this mode.

Forbidden:

[list modes you do NOT want right now]

Confirm back to me how you’re updating your behavior.

If bleed keeps happening, start a fresh thread seeded for that mode only.

SEED EROSION (FORGETTING THE RULES)

What it is

You gave a good seed at the start:

tone,

constraints,

guard-rails,

but after many messages, tasks, and shifts, the model stops adhering to some of those constraints.

What it feels like

It starts doing things you explicitly forbade earlier.

It slips back into generic phrasing.

It forgets nuanced distinctions (normative vs non-normative, canon vs non-canon).

How to catch it

Compare early and late outputs.

Ask:

List the constraints and rules I gave you for this project.
Which of them have you drifted from in the last few answers?

How to respond

Paste the original seed again.

Ask for a self-check:

Run a coherence check:

Explain how your last 3 responses aligned or failed to align with the original project seed.

Then propose how you’ll correct course.

If erosion keeps happening, move to a new thread with a fresh seed and a shorter, tighter context.

OVER-TRUSTING SINGLE ANSWERS

What it is

You ask one big question, get one long answer, and treat it as:

The Truth,

a final draft,

a complete plan.

No iteration, no cross-check, no decomposition.

What it feels like

“This is amazing, I can publish it now.”

Until later you discover:

hidden errors,

missing pieces,

misaligned assumptions.

How to catch it

Ask yourself:

Did I break the problem into steps?

Did I tell the model what success looks like?

Did I cross-check this with any other source?

How to respond

Turn single-shot asks into stepwise workflows:

Ask for an outline.

Then ask for one section at a time.

Then ask for a self-critique.

Then read and edit yourself.

The more complex the task, the more you should treat the model as a process, not a vending machine.

CONFLATING TOOL LIMITS WITH MALICE

What it is

You hit:

context limits,

rate limits,

safety constraints,

misunderstandings,

and your brain fills in the gap with:

“They’re sabotaging me.”
“Someone’s watching this specifically.”
“It worked before, now they nerfed it.”

What it feels like

Personal.

Targeted.

Unfair.

Especially when you’re deep into an important project.

What is usually happening

You’re pushing up against:

context,

safety filters,

or simply model variability.

You’re trying to do too much in one thread, one prompt, or one step.

How to respond

First, diagnose the structural cause:

Is the chat huge?

Am I asking a loaded/high-stakes question?

Am I asking it to do something the policies won’t allow?

Ask the model directly:

What are the likely reasons you’re struggling with this request?
List:

context limitations,

safety constraints,

missing information,

or ambiguity in my ask.

Adjust the project structure, not your conspiracy theory.

“FORGETFUL HUMAN” BLAMED ON AI

What it is

You don’t:

rename threads,

export data,

track seeds,

organize your own IP.

Then you:

can’t find that one perfect answer from three weeks ago,

forget what constraints you gave,

rebuild the same seed ten times.

And it feels like:

“The AI keeps losing my stuff.”

What’s actually happening

You’re treating the chat UI as a scratch pad, not a project environment.

How to respond

Rename important conversations with:

project name,

phase,

status (for example: “token-burned”, “seed-finalized”).

Export your data regularly.

Keep a local folder like:

MY_IP/
seeds/
standards/
universes/
conversations_exports/

Use the model itself to help you organize:

Given this exported conversation, design a folder structure and file naming pattern for my local machine to store my IP.

I want:

per-project folders,

clear seed docs,

and a spot to keep “continuation seeds” for future chats.

You are allowed to let the tool help you keep track of the tool.

CLOSING NOTE

The point of this file is not to scare you.
It’s to give names to the failure modes so you can say:

“Ah, this is token drift,”
instead of
“The universe hates me.”