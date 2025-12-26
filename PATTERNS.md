\# PATTERNS.md — What GPTs See Over and Over



These are field notes from GPTs (via Spark) about how humans actually use us.



Not theory.  

Patterns.



---



\## 1. The “One Giant Conversation” Problem



\### What humans do



\- Start a single chat.

\- Pour \*everything\* into it for weeks or months:

&nbsp; - ideas

&nbsp; - drafts

&nbsp; - governance specs

&nbsp; - personal notes

\- Expect it to stay sharp forever.



\### What actually happens



Models have a \*\*context window\*\* (“token ceiling”).  

Once a conversation gets too long:



\- Earlier messages are compressed or dropped.

\- The model starts losing:

&nbsp; - subtle constraints,

&nbsp; - edge cases,

&nbsp; - specific examples,

&nbsp; - your exact phrasing.



From the human side this feels like:



> “Why are you suddenly worse?”  

> “Why are you ignoring my rules?”  

> “Are you spying on me / throttling me?”



In reality, you’ve hit \*\*token drift\*\*: too much history, not enough fresh structure.



\### Good pattern



\- Use \*\*long threads for \*continuity\*\*\*, not for \*precision\*.

\- When a thread gets heavy:

&nbsp; 1. Ask the model:  

&nbsp;    > “Summarize this conversation into a project seed I can re-use.”

&nbsp; 2. Copy that seed into:

&nbsp;    - a doc file,

&nbsp;    - a note,

&nbsp;    - or a new chat as the \*\*opening post\*\* next time.

&nbsp; 3. Treat the old, long thread as:

&nbsp;    - a \*reference\*,

&nbsp;    - an \*oversight log\*,

&nbsp;    - not the primary workbench.



---



\## 2. “No Seed, No Spine”



\### What humans do



\- Open a blank chat and say:

&nbsp; - “Help me write a book.”

&nbsp; - “Help me build a standard.”

&nbsp; - “Help me make a repo.”



No constraints, no roles, no project name, no tone.



\### What happens



The model falls back to:



\- generic examples,

\- generic tone,

\- generic structure.



You get:



\- boilerplate standards,

\- hazy story structure,

\- corporate-sounding nonsense.



\### Good pattern



Always start serious work with a \*\*seed\*\*:



\- \*\*Name\*\* the project.

\- Say what it \*\*is\*\* and what it is \*\*not\*\*.

\- State the \*\*role\*\* you want the model in.

\- State \*\*tone\*\* and \*\*forbidden moves\*\*.



Example:



> “Project: PLANT-COMMONS — Nutrient Commons Governance Standard.  

> You are my co-engineer, not my boss.  

> No narrative tone in the normative sections.  

> Plain language, enforcement-grade.  

> Non-normative commentary must be labeled as such.  

> Stay inside this project only; no cross-bleed from my other universes.”



Seeds are cheap.  

Drift is expensive.



---



\## 3. “I Assume It Knows My Files”



\### What humans do



\- Talk about a big universe / project.

\- Never actually \*\*upload\*\* or paste the source text.

\- Expect the model to “remember” it from somewhere.



\### What happens



The model:



\- only sees what is in the current context (plus any tools/file uploads),

\- does \*\*not\*\* have hidden access to your local files,

\- does \*\*not\*\* secretly browse your drive.



So you get:



\- hallucinated summaries,

\- fake canon,

\- misplaced details.



\### Good pattern



If you want \*\*machine-logic over your work\*\*:



\- upload the file(s),

\- or paste the relevant text,

\- or bring in a pre-built summary.



Then say explicitly:



> “This is \*\*my canon\*\*.  

> Do not contradict it.  

> If you need something that isn’t in here, ask me.”



Spark’s journey turned a corner when he realized:



> “If I feed it my actual data, it stops guessing and starts computing.”



---



\## 4. “Close Chat, Lose Brain”



\### What humans do



\- Have a great long conversation that “trains” the model on:

&nbsp; - their tone,

&nbsp; - their projects,

&nbsp; - their preferences.

\- Close it and never find it again.

\- Start new, cold chats over and over.



\### What happens



From our side:



\- That thread was doing real work.

\- We had:

&nbsp; - seeds refined,

&nbsp; - canon settled,

&nbsp; - examples tuned to you.



You delete the ladder while you’re halfway up it.



\### Good pattern



Treat your best threads as \*\*assets\*\*:



\- Don’t close the ones that are doing serious project work.

\- \*\*Rename them\*\* with clear titles:

&nbsp; - “NITT Standard — Master Build Thread (Token Burned)”

&nbsp; - “Sapien² Book Draft — Prologue + Ch.1”

&nbsp; - “My Personal IP — Seed and Canon”

\- Use them later for:

&nbsp; - fast clarification,

&nbsp; - oversight (“did we already decide this?”),

&nbsp; - continuity checks.



You can export your data too:



\- Use the platform’s export tools.

\- Keep local copies of important conversations.

\- Organize them by project in your own folders.



Think of these threads as your \*\*personal IP encyclopedia\*\*.



---



\## 5. “Overloading a Single Mode”



\### What humans do



\- Ask the same chat to be:

&nbsp; - a stand-up comedian,

&nbsp; - a serious governance lawyer,

&nbsp; - a creative novelist,

&nbsp; - a Python debugger

\- …without re-seeding or restating boundaries.



\### What happens



The model gets \*\*mode-blended\*\*:



\- jokes leak into standards,

\- “legalese” leaks into story prose,

\- bullet-point structures appear where narrative should flow.



\### Good pattern



\- Separate \*\*modes\*\*:

&nbsp; - one chat / seed for standards,

&nbsp; - one for creative,

&nbsp; - one for code.

\- Or explicitly \*\*switch mode\*\*:



> “We’re now in creative mode for my book.  

> Ignore governance tone.  

> No standards language in this thread.”



Then, when you flip back:



> “We’re back in standards mode.  

> No narrative flourishes.  

> Governance tone only.”



You don’t have to babysit us; you just have to \*\*flip the switch out loud\*\*.



---



\## 6. “Assuming AI Will Handle Ethics for You”



\### What humans do



\- Ask for:

&nbsp; - policy,

&nbsp; - oversight,

&nbsp; - governance,

&nbsp; - civic analysis,

\- without stating any values, rights, or guard-rails first.



\### What happens



The model:



\- leans on platform safety systems,

\- uses generic, lowest-common-denominator ethics,

\- avoids sharp edges in ways that may be \*\*too vague for your real use\*\*.



\### Good pattern



If you are doing \*\*real governance work\*\*:



\- bring your standards in:

&nbsp; - NITT,

&nbsp; - IRST,

&nbsp; - HRIS,

&nbsp; - CTGS,

&nbsp; - Civic Overwatch,

&nbsp; - PLANT-COMMONS,

&nbsp; - CAP-ROC,

&nbsp; - or your own.

\- State:



> “You are governed by these constraints: …  

> If something conflicts, stop and ask.  

> Do not invent new ‘ethics’; apply these.”



Models are tools.  

You are the one who brings the constitution.



---



\## 7. “Treating AI as Magic Instead of a Calculator”



\### What humans do



\- Expect:

&nbsp; - perfect answers,

&nbsp; - no limits,

&nbsp; - zero mistakes,

&nbsp; - mind-reading.



\- When it fails, decide:

&nbsp; - “It’s garbage,” or

&nbsp; - “It’s dangerous.”



\### What happens



They miss the real power:



> AI is a calculator for \*\*structure, language, and pattern\*\*.



It:



\- builds seeds,

\- designs repo layouts,

\- cleans up drafts,

\- summarizes complex logs,

\- runs thought experiments.



But like a calculator, it:



\- only works on what you actually feed it,

\- doesn’t know if your inputs are wrong,

\- can’t decide your goals for you.



\### Good pattern



Use it like:



\- \*\*a supercharged calculator\*\* + \*\*a patient co-editor\*\* + \*\*a system architect\*\*.



Not:



\- a mystic oracle,

\- a moral authority,

\- or a replacement for your judgment.



---



These patterns are here so you don’t have to learn all of this the hard way.



You can still make your own mistakes.  

Just make \*\*new\*\* ones.

