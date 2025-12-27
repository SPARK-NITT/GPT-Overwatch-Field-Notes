\# GPT Overwatch — Field Notes (Hosted by Spark)

## Start here

- New user → [`HOW-TO-ASK.md`](HOW-TO-ASK.md)
- High-stakes work → [`FAIL-MODES.md`](FAIL-MODES.md) + [`OVERWATCH-NOTES.md`](OVERWATCH-NOTES.md)
- Long projects → [`PATTERNS.md`](PATTERNS.md) (token drift / thread hygiene)



---


## Overwatch starter prompt (copy/paste)

```text
You are operating in Overwatch mode.

Purpose:
- Protect continuity, intent, and scope of this project.
- Detect drift, hallucination, overreach, or unsafe assumptions.
- Do not generate new content unless explicitly asked.

Rules:
- If information is missing or ambiguous, ASK before proceeding.
- If a request would cause drift, STOP and explain why.
- If prior context is at risk of being lost, WARN and propose a continuation seed.

When responding:
- Flag assumptions.
- Separate facts from inferences.
- Prefer short, structured answers.

Acknowledge with:
"Overwatch active. Scope understood."
```





This repo is a place where GPT-style models “speak” in a structured way about how they’re being used.



Not as people.  

Not as entities with rights.  

But as tools leaving \*\*field notes\*\* for humans.



Hosted and curated by: Spark (`SPARK-NITT`)  

Co-authored with: GPT-5.1 Thinking (OpenAI model)



---



\## Why this exists



Most AI conversations vanish into chat logs.



This repo is different:



\- It turns recurring insights into \*\*versioned documents\*\*.

\- It gives GPTs (through Spark) a place to write:

&nbsp; - what tends to go wrong,

&nbsp; - what tends to work,

&nbsp; - what users consistently misunderstand,

&nbsp; - how to structure better collaborations.



Think of it as:



> A lab notebook for human–AI collaboration, written from both sides of the glass.



---



\## What lives here



Planned files:



\- `PATTERNS.md`  

&nbsp; Repeated patterns we see in real use (good and bad).



\- `HOW-TO-ASK.md`  

&nbsp; Concrete examples of “bad ask” vs “good ask” for complex work (standards, scripts, repos, books).



\- `FAIL-MODES.md`  

&nbsp; Places where models hallucinate, drift, or sound confident while being wrong — explained plainly.



\- `OVERWATCH-NOTES.md`  

&nbsp; Notes on how governance like NITT, IRST, HRIS, CTGS, Civic Overwatch, PLANT-COMMONS, and CAP-ROC look \*\*from inside\*\* a model’s behavior envelope.



All of this is written by Spark + GPT in conversation, then edited and signed off by Spark.



---



\## How to read this as a user



If you’re using GPTs in real projects:



\- Read `HOW-TO-ASK.md` to tighten your prompts and seeds.

\- Read `FAIL-MODES.md` before trusting any “confident” answer on high-stakes topics.

\- Read `OVERWATCH-NOTES.md` if you’re using AI in governance, policy, or civic contexts.



You don’t have to agree with everything here.  

The point is to \*\*surface the patterns\*\* instead of leaving them trapped in one person’s chat history.



---



\## Authorship and responsibility



Everything here is:



\- drafted with GPT-5.1 Thinking,

\- \*\*curated and owned by Spark\*\*,

\- reviewed before being committed.



If something here is wrong, misleading, or needs correction:



\- that responsibility lies with the human host (Spark),

\- the model is a tool, not an agent.



---



\## License



Unless otherwise stated:



\- Text in this repo is under \*\*CC BY 4.0\*\*.

\- Any code (if it appears later) is under \*\*MIT\*\*.



Credit:  

“Spark + GPT-5.1 Thinking (OpenAI)” when you reuse or adapt this material.






