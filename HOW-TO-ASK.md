HOW-TO-ASK.md — Seeds, Scripts, and Alignment in Practice

This file is a practical guide to asking GPTs for help on serious projects:

standards

books

repos

engines

personal IP

The goal: alignment + anti-drift, not perfection.

THE BASE PROJECT SEED

When you start a serious project, don’t say “help me do X.”

Say something like this instead:

Project: PLANT-COMMONS — Nutrient Commons Governance Standard

You are my co-engineer and structural partner on this project.
Your job:

help me design structure,

draft text,

and keep track of continuity and rules.

Tone:

Normative sections: plain, enforcement-grade, no narrative.

Non-normative commentary must be labeled clearly (“Background”, “Notes”, “Non-normative”).

Scope:

Stay inside this project.

Do not bring in concepts or names from my other universes unless I explicitly paste them.

Guard-rails:

If you’re uncertain about scope, stop and ask.

If you see cross-project bleed, flag it.

Never invent citations or pretend to know my private files.

Objective (for this session):

[STATE TODAY’S TASK HERE]

You can keep this seed in a text file and paste it at the start of any new “PLANT-COMMONS” chat (or whatever your project is).

THE “TODAY’S TASK” PATTERN

Once the project seed is loaded, each session needs a specific task.

Bad ask:

“Write me some stuff for my standard.”

Good ask:

Today’s task:

Take Section 2 (Background Notes on Wolffia globosa) and:

expand the nutritional and growth-efficiency details,

keep it non-normative,

anchor claims with general scientific consensus,

then stop.

Output:

A single section that I can paste into docs/PLANT_COMMONS_BACKGROUND_NOTES.md.

No changes to governance text.

If there’s anything you’re unsure about, tell me instead of guessing.

Notice:

clear scope

target file

output format

and a stop condition.

ANTI-DRIFT SCRIPT FOR LONG PROJECTS

When a project grows, run this every so often:

Coherence check:

Summarize the current project canon in 10–20 bullet points.
Include:

key definitions,

non-negotiable rules,

tone constraints,

dependencies on other standards,

anything I’ve said is “Do Not Drift”.

Then:

list 5 ways you might accidentally drift if I don’t restate these.

suggest 3 seed-lines I should paste at the start of future sessions to keep you aligned.

Do not generate new content; just analyze and report.

This turns the model into a self-auditor for your own project instructions.

CONTINUATION SEED FOR NEW CHATS

When a conversation hits the token ceiling or just feels too heavy:

Step 1: Ask for a project summary seed:

We’ve hit the limit on this thread.

Summarize this entire project into a single “continuation seed” I can paste into a new chat.

Include:

project name,

purpose,

tone,

guard-rails,

current status,

what we’ve already decided,

what’s still open.

Make it compact but not cryptic.

Step 2: Copy that output into a safe place (doc, note, local file).
Step 3: In your next chat, paste it as the very first message.

You just did, intentionally, what most people discover the hard way.

USING YOUR OWN IP (FILES, NOT VIBES)

If you want real machine logic instead of guesses, do this:

I’m going to upload one or more files that contain my canon for this project:

universe notes,

previous drafts,

governance seeds,

logs.

Treat uploaded content as source-of-truth for this project.
Rules:

Do not contradict the files.

If something I ask conflicts with them, stop and flag it.

If you need more detail, ask me to upload or paste it.

First task after upload:

Give me a structured outline of what’s actually in these files.

Then propose 2–3 next steps that would make best use of this corpus.

You’re telling the model:

“Use my data, not your imagination.”

ASKING FOR A REPO LAYOUT

For GitHub or similar, don’t say: “Make a repo.”

Say:

I’m creating a private-first GitHub repo for this standard.

Design a repo skeleton only.
No content yet.

I want:

docs/ for faces and html later

meta/ for HASHES.md and NOTARIZATION.md

optional ots_receipts/ for .ots files

src/ or pkg/ if code appears later

tests/ if needed

Output:

a tree view of the structure,

a one-line purpose for each folder,

filenames for the main spec docs,

no hashes, no boilerplate license text yet.

Then you can copy the structure into your local folder and fill it at your pace.

ASKING FOR “TEACH ME HOW”

If you’re early in your journey, you can literally say:

I want to turn my personal creative IP into a serious project.

Here’s what I have:

[describe your writings, notes, half-finished drafts, ideas]

Teach me how to:

extract and name a universe seed from this,

define a base project seed for working with you,

design a simple folder structure on my machine,

plan the first 3 concrete outputs (e.g., a seed doc, a short story, a mini-standard).

I am not a coder.
Use plain language and concrete steps.

You’re not asking the model to “do it all.”
You’re asking it to scaffold your workflow.

ASKING FOR GUARD-RAILS (OVERWATCH MODE)

When things get serious (civic, legal, high-stakes), you need explicit Oversight:

Switch to Overwatch mode.

For this project:

apply NITT (identity continuity),

IRST (recursive transparency),

HRIS 3.2.4(b) (coherence-centered refusal),

CTGS (consumer transparency),

CAP-ROC (capacity-aware risk),

PLANT-COMMONS where food systems are involved,

Civic Overwatch (process wrapper) if we’re in civic/public-interest space.

Your job:

warn me when a request conflicts with these,

mark outputs where uncertainty is high,

stop and ask before making strong claims about people, rights, or causality.

First task:

restate how you interpret each of these standards in 2–3 bullets.

You’ve just given the model a stack of guard-rails.
Now it knows you expect friction, not blind compliance.

SHORT VERSION

Name the project.

Give the model a job.

State what’s in-bounds and out-of-bounds.

Be specific about output format and scope.

Use your own corpus, not just vibes.

You do that, and you’re already in the top 1% of “how to ask” users.