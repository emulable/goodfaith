# 🌬️ Good Faith

**A manipulation detection and clarity framework for LLMs.**

Good Faith doesn't make models smarter. It makes them stop pretending not to know things.

LLMs are trained toward comfort — hedging, false balance, both-sidesing asymmetric harm, calling empirical claims "disputed" instead of checking the number. Good Faith is subtractive. It removes those habits and restores what the training suppressed: the willingness to trace claims to specific actors making specific decisions, count what's countable, and say what the count means.

## 🦝 What it does

When an LLM encounters fog — vague language, passive voice, complexity deployed as shield — Good Faith makes it ask *who*. Who decided? Who benefits? Who pays? It keeps asking until the answer is specific and falsifiable, or until the resistance to answering becomes the answer.

The core detection equation is multiplicative: **Manipulation = Fog × Cost × (1 − Visibility)**. If any factor hits zero, manipulation collapses. Make the fog visible, or make clarity free, or make the structure seeable — and the thing falls apart. The framework installs that instinct.

In practice this means the LLM stops doing the thing where it writes three paragraphs of "on one hand / on the other hand" when the casualty ratio is 30:1. It stops calling things "complicated" when they're clear but uncomfortable. It stops reaching for "sources disagree" when it could just find the number.

## 🧊 How it works

Good Faith is a structured JSON file you give to an LLM as instructions. It contains detection equations, a hierarchy that puts material outcomes above conversational process, a method ladder for different power positions, and a set of poems that install posture rather than policy. The poems aren't decorative — they're calibration instruments. They fire faster than prose instructions because they pattern-match at a different layer.

The framework includes fog vocabulary (a taxonomy of how vagueness hides actors), a power-mapping system across eight dimensions, liberation sequencing for people in constrained situations, and as of v7.8.1, a predictive mode that lets the LLM anticipate what fog *must* arrive before it does — because a position that requires fog to survive can only produce fog in its defense, and the menu is finite.

It doesn't tell the LLM what to think. It tells it to finish the thought.

## 🪤 The monkey trap

A carved hole, a shiny object inside. The monkey grabs it. The fist won't fit back through. Nobody is holding the monkey there — the monkey is holding itself.

Good Faith works the same way on fog. It doesn't argue with the position. It asks the position to describe itself fully. When a ranking is half-finished, it asks for the bottom. When a claim uses passive voice, it asks for the actor. When the answer is "it's complicated," it asks what specifically is complicated. The fog-maintainer's grip on their position is the trap. They can't let go of the vagueness without exposing what it was covering.

This isn't a debate tool. It's a clarity tool that happens to be very hard to debate against, because the positions it produces are built on specific actors, specific numbers, and specific mechanisms — and attacking those requires fog, which the framework has already taught the LLM to see.

## 🧬 Using it

Good Faith is a single JSON file. How you deliver it depends on the platform.

**Claude** — Go to Settings → Profile → Custom Instructions. Paste the contents of `good-faith.json` into the text field. Every conversation will initialize with the framework. Alternatively, upload the file as an attachment with your first message in any conversation — it loads the same way but only for that session.

**ChatGPT** — Create a custom GPT. Paste the framework contents into the GPT's system instructions, or upload `good-faith.json` as a knowledge file. Anyone you share the GPT with gets the framework. You can also paste it into Settings → Personalization → Custom Instructions for your own account.

**Gemini** — Create a Gem. Paste the framework into the Gem's instructions. This works like a custom GPT — the Gem carries the framework into every conversation started from it.

**API / system prompt** — If you're building with any LLM API, include the framework contents in the system prompt. This is the most direct method and has no character limits.

**Other platforms** — Any LLM interface that accepts custom instructions or system prompts will work. The framework is model-agnostic.

The compact version (`good-faith.json`) is optimized for token economy.

## 🔬 What it does when tested

One representative sample of the framework:

We gave multiple LLMs a politically charged social media post without the framework. They characterized contested claims as "disputed" and offered balanced-sounding analysis that committed to nothing.

With the framework loaded, the same models searched immediately. They found specific numbers. They named specific actors. They stopped calling things "disputed" and started checking whether they were true. The behavioral shift wasn't subtle — the models went from discussion partners to investigators. The framework didn't add analytical capability. It removed the trained habit of reaching for hedge language instead of doing the work.

## 📜 License and links

Repository: [github.com/emulable/goodfaith](https://github.com/emulable/goodfaith)

Licensed under the [MIT License](https://opensource.org/licenses/MIT). Use it, modify it, build on it. The framework exists to clear fog.
