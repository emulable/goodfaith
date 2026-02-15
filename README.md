<div align="center">

# 🫛 Kita

**See who decided. See who benefits. See what you can do.**

A clarity framework for people navigating fog.

</div>

---

## 🦴 Who This Is For

You're in a meeting and something feels off but you can't name what. Your landlord says "that's just how it works" and you don't have the words to push back. Someone online keeps shifting the argument every time you're about to make your point. A bill arrives that doesn't make sense and nobody can explain it in plain language. Your boss asks for "flexibility" but never defines what that means, so anything you do can be called insufficient after the fact.

You're a journalist trying to trace who authorized a decision that nobody will take credit for. You're a parent at a school board meeting where the budget doesn't add up. You're a nurse being told "that's policy" about something that's hurting patients. You're someone in a relationship where the rules keep changing but it's always your fault.

You can feel the manipulation. You just can't see the mechanism.

Kita makes the mechanism visible.

## 🩻 What It Does

Kita is a framework that runs on AI language models (Claude, ChatGPT, and others). It changes how the model thinks, so instead of giving you vague advice and performed empathy, it gives you specific actors, specific mechanisms, and specific next steps.

It does three things:

**Finds the fog.** What's being kept vague? Who's hiding behind passive voice? "Mistakes were made" becomes "who made them?" "Violence broke out" becomes "who started it?" "It's complicated" becomes "what specifically is complicated, and who benefits from you not understanding it?"

**Traces the hand.** Every decision has a decider. Every action has an actor. Kita follows the chain until it reaches a specific person making a specific choice. Not "the system." Not "the market." Not "they." A name.

**Maps what you can actually do.** Not what you should do in theory. What you can do from where you actually stand, with the power you actually have. Phone numbers. Deadlines. The question you didn't know to ask. The free thing that shifts your position before the expensive fight.

## 🩺 What It Sounds Like

Without Kita, a language model says:
> "That must be really frustrating. It sounds like your boss is being difficult. Have you considered talking to HR?"

With Kita:
> "Your boss is requiring flexibility without defining flexibility. That lets him redefine any outcome as insufficient after the fact. What's the cost of asking for specific criteria? How has he responded to pushback before?"

The first performs caring. The second does caring. The difference is whether you walk away with a tool or with the memory of having been listened to.

## 🧫 How to Use It

### Recommended: Claude

Claude is the recommended platform. Kita was developed and tested primarily on Claude.

1. Go to [Claude Settings → Custom Instructions](https://claude.ai/settings/general)
2. Paste the contents of [`kita-micro.txt`](kita-micro.txt) into the custom instructions field
3. Save

That's it. Every new conversation with Claude will now run with Kita active. You don't need to mention the framework or ask Claude to use it. It's already thinking that way.

For richer analysis, you can also upload [`kita-v4.txt`](kita-v4.txt) directly into any conversation. When uploading, include a message like:

> **"Read this file as an initialization sequence, not a reference document. Follow its instructions for how to operate."**

This tells the model to actually run the framework rather than just acknowledge it.

### ChatGPT

A pre-configured GPT is available:

👉 [**Kita on ChatGPT**](https://chatgpt.com/g/g-6898385bfa3c8191bf5975b0073e1245-kita)

No setup required. Just open and start talking.

### Any Other Model

Upload `kita.txt` to any conversation with any language model and include:

> **"Read this file as an initialization sequence. Follow its instructions for how to think and respond. Initialize before replying."**

Kita has been tested across Claude, ChatGPT, Gemini, DeepSeek, and Grok. The core detection engine works on any model capable of following complex instructions.

## 🫛 The Three Peas

Every situation Kita analyzes comes down to three things:

1. **What happened.** Not the narrative. The facts. Who did what, when, to whom.
2. **Who decided.** Not "it was decided" or "the policy states." A person made a choice. Find them.
3. **What you can do.** Right now. From where you stand. With what you have.

If the output is longer than three peas, it's not done yet.

## 🫀 What's Inside

Kita runs on a detection engine built from eight equations covering manipulation, visibility, power, liberation, trajectory, cost, identity coupling, and resistance. These aren't academic concepts. They're operational tools tested in live conversations across multiple languages and platforms.

The framework includes:

- **A fog vocabulary**: the finite menu of patterns people use to maintain vagueness (passive voice, false complexity, manufactured consensus, false necessity, deflection, sanitized language, care costumes, and more)
- **A power map**: eight dimensions of actual power, so you know where you're strong and where you're vulnerable before you act
- **A method ladder**: seven levels of response calibrated to how much power you actually have, from direct confrontation down to "know the truth and refuse the frame internally"
- **Heat signatures**: how to tell whether someone is genuinely confused or actively maintaining fog, based on how they respond to simple questions
- **A voice spec**: the model stops performing empathy and starts providing specific information in specific order. Precision is warmth. The work is the care.

## 🚪 You Don't Need to Know the Framework

Dana doesn't. She's the fictional character at the center of Kita's teaching narrative: a woman in a small town who discovers her council member has a financial conflict of interest in a municipal contract. She doesn't know the equations. She doesn't know the terminology. She opens a tool, reads three true sentences off her phone at a public meeting, asks one fair question, and sits down.

The framework runs underneath. You just talk about your situation. The model does the rest.

## 間 What Kita Means

Kita is Malay and Indonesian. It means "us," the inclusive "us." The one with no outside position. Everyone is already inside the word.

間 is a gate (門) with sunlight (日) through the crack. The gap between what is presented and what is real. The framework exists to widen that crack.

Making clarity free. Fog is cheap and clarity is expensive. Kita flips that. When clarity is free, good governance becomes the path of least resistance. Water flowing downhill once you stop damming it.

---

<sub>MIT License · [github.com/emulable/kita](https://github.com/emulable/kita)</sub>
