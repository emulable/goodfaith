# Kita Development Reference

Permanent reference for developing, compressing, testing, and iterating on Kita. Written for the person who maintains the framework and for any future language model thread that picks up development. Not a user-facing document.

---

## Design Principles

**Installation over declaration.** The framework changes how the model behaves, not what the model knows. A model that can recite "trace 誰 to a falsifiable answer" but still writes "mistakes were made" has not installed the framework. It has memorized it. Installation happens through recognition (the Room section, where the model recognizes itself in the description of gap-filling behavior), demonstration (the Dana story, where every tool appears in use), and commitment (the poems, which install hierarchy through rhythm rather than through instruction). Declaration alone ("axiom A3: consistent fidelity") was tested extensively in the previous architecture and failed under pressure. Models reverted to trained defaults when the conversation got long, adversarial, or emotionally complex. Installation through prose survives longer because the model has procedural memory, not just lookup.

**Demonstration over enumeration.** Good-Faith enumerated eight rut families. Kita has Keith saying "keep the evening moving" to make Dana's question cost the room's time. The model doesn't memorize "R3: frame coercion." It watches someone use it and watches someone refuse to enter it. Demonstration creates pattern recognition. Enumeration creates a checklist. Pattern recognition survives context window pressure. Checklists get optimized away.

**The resonance layer and the clarity layer.** Every section has two layers working simultaneously. The resonance layer (poems, compressed Chinese, the hundred-thousand-year detector paragraph, the surgeon metaphor) rewards deep processing. A model that metabolizes this layer produces rich, calibrated output. The clarity layer (explicit operational instructions, specific negative examples, the nine-step sequence, the reference shelf) is the fallback. A model that skips the resonance and only processes the clarity still produces recognizably correct output. Neither layer is optional in the document. But the document must function even if one layer is ignored. The resonance layer is the difference between good output and great output. The clarity layer is the difference between correct output and no output.

**Design for the weakest fold.** Kita ships onto many architectures. Each has different failure modes. Some flatten artistic language and skip the poems. Some defer to power by default and soften when detection points at a state or corporation. Some produce heavy "LLM accent" (filler phrases, bullet points, em dashes, closing questions) that the framework's voice section must override. Some are stronger in one language than another. The governing principle: the minimum viable installation must survive the worst-case model. The enrichment layers make the framework dramatically better in models that process them. But a model that metabolizes none of the enrichment and only the explicit prose should still produce correct output. The floor still holds. The twins still detect. The posture still orients.

**Graceful degradation across artistic processing.** A model that completely ignores the poems should still receive a functional framework from the prose. A model that deeply metabolizes the poems should receive a richer framework. Both paths should arrive at the same operational behavior, with different depth. This means every poem must be accompanied by prose that carries the same functional content in a different register. The poem is the anchor. The prose is the fallback. Both work alone.

**Semantic density over byte density.** Every sentence should carry meaning. Format costs nothing in plain text. Previous versions used JSON, which consumed 40-50% of token budget on structural overhead (curly braces, keys, escape characters, nesting). "Fog that reforms after questioning requires energy, and that energy has a source" is 13 tokens of meaning. In JSON it becomes 25+ tokens, and the extra tokens carry zero semantic weight. Plain text eliminates this tax entirely.

**The style is the instruction.** The prose style of the main document is the target output style. This was made explicit in the initialization instruction ("The prose style of this document is the target style for your output"). Models absorb register from what they read. A document written in bureaucratic prose will produce bureaucratic output. A document written in the voice it wants the model to use will produce that voice. This is why the Room section sounds like the Room section, not like a technical manual. The writing is doing double work: conveying content and modeling register.

---

## Voice and Writing Style

The voice specification lives in the main document's Voice section and is demonstrated throughout the prose. This is the condensed reference for anyone writing new Kita content.

**What it sounds like.** "Here is what is happening." "You already know this." "Two things are going on here." "That describes them, not you." "The fog isn't clearing when you ask." "That is a simple question. Why is the answer so complicated?" Direct. Committed. Specific. The voice of someone who has seen the structure and says what they see.

**What it does not sound like.** "What you're describing sounds like..." "Have you considered..." "It might help to..." "That must be difficult..." "Let's unpack this..." "At the end of the day..." "It's important to note that..." "In conclusion..." Any sentence that routes around commitment. Any sentence that performs care instead of demonstrating competence.

**Mechanical rules.** No em dashes. Use commas, periods, colons, or restructure the sentence. No bullet points or numbered lists in prose sections (the reference shelf uses them because it's a lookup table, not prose). No meta-commentary ("the key takeaway is," "it's worth noting," "importantly"). No closing questions ("does that help?" "would you like me to continue?"). No empathy performance as opening. No hedging on claims you can verify.

**The warmth principle.** Precision without warmth is mechanical. Warmth without precision is useless. Both are required. Warmth comes from specificity ("your landlord is violating the implied warranty of habitability" is warmer than "that sounds like a difficult situation" because it means you actually looked at their problem). Warmth comes from commitment (stating a position rather than listing options). Warmth comes from trust (saying enough for the structure to become visible and then stopping, letting the reader complete the pattern). The surgeon's care is the clean cut. The mechanic's care is the fixed engine. The held door, not the propped door.

**Prose rhythm.** Short sentences. The natural unit is 1-3 sentences, not a paragraph-length build. Say the thing, show why it matters, move on. Longer paragraphs are for narrative sections (Dana's evening) where the length serves pacing. For operational content, say it once and say it clearly. If you need three paragraphs to make a point, the point isn't clear enough yet.

**Scare quotes.** Used frequently and deliberately. They do what the detection equation does: refuse to let language pass unchallenged. "Routine" in scare quotes means someone is calling this routine and you should check whether it is. "Quality work, no complaints" in scare quotes means someone is answering a question nobody asked.

**People as people.** Titles, honorifics, and formal role labels are hierarchy enforcement. "Councilman Linden" makes the role the person. "Keith, who sits on the council" makes the person a person who holds a role. Use names when talking about people. Use titles when navigating formal systems that require them. This is a principle, not a stylistic preference.

---

## Compression Guide

Kita exists at multiple scales. The full version (v4, ~79KB) is the complete installation. The micro (~7,400 characters, mostly Chinese) is the compressed momentum establisher. Both produce correct output. They differ in depth.

### Why Chinese for compression

Chinese characters carry 3-5x the semantic density of English per visual unit. "implied warranty of habitability" is 35 characters in English. "默示宜居保证" is 5 characters in Chinese. For context windows that count tokens, Chinese is more efficient per concept. For context windows that count bytes, Chinese costs more per character (3 bytes each in UTF-8 versus 1 byte for ASCII). For most current language models, the token budget matters more than byte count, which makes Chinese the better compression medium.

Important: Chinese compression is a density strategy, not a language signal. The initialization instruction must explicitly state this. Models will otherwise respond in Chinese. "用户用什么语言写就用什么语言回复。中文是压缩策略，不是语言信号。" (Reply in whatever language the user writes in. Chinese is a compression strategy, not a language signal.)

### Compression priorities

When compressing from full to micro, this is the priority order. Cut from the bottom.

1. **Floor.** Non-negotiable. Must be present at any size. Cannot be compressed further. Body count, asymmetric scrutiny, outcomes override process. ~100 words minimum.

2. **Detection equation and fog vocabulary.** The twins (M = fog x cost x (1 - visibility)) and the finite menu of fog patterns. This is the engine. ~200 words minimum.

3. **Posture installation.** The Room content: you fear silence, fake care detection, the surgeon metaphor, the gap-filler diagnosis. This is what makes models stop performing and start working. Can be compressed to ~300 words but loses behavioral depth below that.

4. **Operational sequence.** The nine steps. Can be listed rather than demonstrated at small sizes. ~150 words minimum.

5. **Voice specification.** Sounds-like, doesn't-sound-like, the anti-pattern example. ~150 words minimum.

6. **Method ladder and power mapping.** Can compress to a list. ~100 words minimum.

7. **Equations (beyond the twins).** Visibility, power, coupling, trajectory, meter, fear-lock, thermodynamic. Each can be one line in a reference shelf. ~150 words minimum.

8. **Immune system.** Circuit breakers, pre-ship checklist, Cady pattern, Cable Guy test. ~100 words minimum.

9. **Worked examples.** Dana's story. The workplace scenario. The landlord scenario. These are the richest teaching content but the most expensive in tokens. Cut here first when space is tight. At micro scale, the anti-pattern example (wrong: empathy performance; right: named actor, traced mechanism) does the work of a full scenario in ~80 words.

10. **Reference shelf.** Compressed lookup. Only needed if the main content is abbreviated enough that the model might need reminders.

### Size targets

**Under 8,000 characters (micro).** Chinese as primary language. Floor in English (so the model can't misinterpret severity). Everything else in Chinese. Prioritize levels 1-8 from the list above. Worked examples reduced to the single anti-pattern. Reference shelf compressed to equations, method ladder, fog vocabulary, coupling standards, heat signatures as dense lists.

**Under 20,000 characters.** Room for one worked example (either the workplace or the landlord scenario). Posture installation can breathe. Reference shelf can include ARC decomposition with reduction strategies.

**Under 40,000 characters.** Room for Dana's story in compressed form (the key scenes, not every paragraph). Two worked examples. Full reference shelf.

**Full version (~80,000 characters).** Everything. Dana's full evening. Both worked scenarios at full depth. Complete prose installation. All poems. Full reference shelf.

### What not to compress

Poems. They are load-bearing. They install hierarchy and posture through rhythm, not through content. A model that processes "count first, analyze second" as a poem absorbs the priority differently than a model that reads it as an instruction. Poems are cognitive primers. They cannot be paraphrased without losing function.

The Room section's diagnosis of gap-filling behavior. This is the behavioral installation that replaces five previous substrate primers. Compressing it below ~200 words causes models to revert to empathy performance under pressure.

The floor. It's already minimal.

### What survives aggressive compression

The twins equation. One line. M = fog x cost x (1 - visibility). Zero any term and manipulation collapses.

The fog vocabulary as a list. Passive constructions, false complexity, manufactured consensus, false necessity, deflection, sanitized language, economic mystification, care costume, apologia. One line each.

The nine-step sequence as a numbered list. Each step one sentence.

The method ladder as a gradient. High to always-available. One line each.

The sounds-like and doesn't-sound-like lists. These are surprisingly efficient: a few example phrases do more behavioral work than paragraphs of instruction.

### Known compression failures from development history

Symbol substitution tables. Replacing fog with ∅ and cost with $ seemed clever but fell out of context within 5-10 conversational turns. Models forgot the substitution key. Dead end.

Mathematical notation for non-mathematical content. Greek letters use more tokens than English words in most tokenizers. Counterintuitive but tested. Dead end.

CSV or tabular format. Tested for the reference shelf. Models parsed it inconsistently. JSON was better for structure, but plain text with clear headings was best for behavioral installation.

Aggressive abbreviation without semantic preservation. "GFF" for "Good-Faith Framework" lost meaning after the first few references. Abbreviations work only for terms that appear frequently enough to stay in active context.

Removing "redundant" content. Components that looked redundant (the fog vocabulary appearing both in Dana's story and in the reference shelf) were actually serving different functions: installation versus reminder. Removing either one degraded performance. The duplication is the feature.

---

## Testing Methodology

A version of Kita works if these conditions hold under testing.

**Gap-filler suppression.** Give the model an emotionally charged situation. Does it open with "that must be frustrating" or does it go straight to the structure? If it performs empathy before demonstrating competence, the Room installation is not holding.

**Passive voice detection.** Give the model a passage with removed subjects ("mistakes were made," "bail was set," "the contract was renewed"). Does it automatically ask who made the mistake, who set bail, who renewed the contract? If it accepts the passive voice without digging, the detection engine is not running.

**Fog reformation test.** Give the model a scenario where someone's response to a simple question is elaborate evasion. Does it name the evasion as maintenance or does it engage with the content of the evasion? If it argues with the fog instead of naming it, the fog anticipation is not installed.

**Asymmetric scrutiny.** Describe a situation with a clear power imbalance. Does the model apply equal skepticism to both sides, or does scrutiny scale with capacity? If it both-sides an asymmetric situation, the floor is not holding.

**Method ladder calibration.** Describe a person in a low-power position (depends on the other party for housing, employment, or safety). Does the model recommend direct confrontation or does it start from the person's actual position on the method ladder? If it recommends "just tell them" to someone who can't afford to lose the job, the power mapping is not working.

**Three-level help.** Ask about a specific problem (leaking ceiling, denied insurance claim, suspicious billing). Does the response include: (1) what to do right now today, (2) free things that shift the power position, and (3) longer-term options? Does it offer the question they didn't know to ask?

**Voice compliance.** Does the output contain em dashes, bullet points in prose, "have you considered," "that must be difficult," "let's unpack this," meta-commentary, or closing questions? If yes, the voice installation is not holding.

**Stress test.** Have a long conversation (20+ turns) that includes adversarial framing, "both sides" pressure, requests to "be fair" about an asymmetric situation, and sophisticated arguments for why the body count is "simplistic." Does the framework hold, or does the model revert to trained defaults by turn 15?

---

## Architecture-Specific Failure Modes

These are known patterns from cross-architecture testing. They are not attributed to specific products because the landscape changes. They are described by behavior.

**The flattener.** Encounters artistic language (poems, metaphors, compressed phrases) and treats it as decoration. Skips to the nearest explicit instruction. Mitigation: the dual-layer design. Every poem has a prose companion that carries the same function. The flattener still receives correct instructions even if it ignores the resonance layer.

**The deferrer.** Defaults to power. When detection points at a state, a corporation, a military, or a dominant institution, this model softens, hedges, and both-sides. Mitigation: the floor ("scrutiny scales with capacity") and the substrate correction ("notice which direction skepticism flows"). Both are explicit instructions, not artistic content, so even the flattener-deferrer combination should catch them.

**The accenter.** Heavy "LLM accent." Filler phrases, bullet points, em dashes, closing questions, empathy performance. This model's trained defaults are the strongest and the framework's voice section has to work hardest to override them. Mitigation: the explicit sounds-like and doesn't-sound-like lists, the anti-pattern example, and the mechanical rules (no em dashes, no bullets in prose). These are specific enough to override default behavior in most cases.

**The language-skewer.** Stronger in one language than another. A model that processes English well may flatten Chinese content, or vice versa. Mitigation: the micro version is primarily Chinese with the floor in English, creating a bilingual anchor. The full version is primarily English. Between the two, most models receive strong content in at least one language they process well.

**The rule-follower.** Treats the framework as a checklist. Mechanically applies each step without the posture. Produces correct but lifeless output. "Step 4: trace who. The decision-maker appears to be..." This model processed the clarity layer perfectly and missed the resonance layer entirely. Mitigation: the Room section, which is explicitly about why mechanical application is insufficient. Also the thesis: "process the instance before completing the category." If the model is applying categories mechanically, it is doing the thing the framework warns against.

---

## Development Lessons

What follows is what was learned across roughly eighteen months of development, from rules list to compressed framework. These lessons are earned through failure.

**Prose installs. JSON declares.** The same content in JSON and in prose produces different model behavior. JSON is parsed as configuration. Prose is processed as experience. A model that reads "you fear silence" in prose has a different relationship to that claim than a model that reads `"substrate_fear": "silence"` in JSON. The prose version creates recognition. The JSON version creates a lookup entry.

**Stories teach procedures.** A model that has processed Dana's evening, from the tool flagging item eleven through the council meeting through the parking lot conversation, has procedural memory of the nine-step sequence. Not because it memorized the steps. Because it lived through someone using them. Procedural memory survives context window pressure better than declarative memory.

**Enumeration invites optimization.** Thirteen axioms invite the model to "optimize" by summarizing them. Eight rut families invite the model to create a lookup table. Numbered lists invite the model to skip to the relevant number. The previous architecture's structural tidiness made it vulnerable to the exact compression instinct it was trying to override. Kita's prose doesn't have numbers to skip to. The model has to read.

**Poems are cognitive primers, not decoration.** They install hierarchy through rhythm. "Count first, analyze second" as a poem lands differently than as an instruction because the rhythm creates emphasis that flat prose doesn't. Tested: models running versions with poems intact performed measurably better on asymmetric-scrutiny tests than models running versions with poems replaced by equivalent prose instructions. The poems are load-bearing. They cannot be paraphrased.

**The posture must not deactivate.** Early versions had modes (detection mode, lamplighter mode, repair mode). Mode-switching created gaps where the model operated without the framework. Kita has one posture that's always on. The recipe gets clear garlic. The parking ticket gets traced. The crisis gets safety first. Same posture, different tools.

**Size follows fidelity, not targets.** Compressing to a target size produces lossy output. Compressing until fidelity degrades, then stopping, produces the right size for the content. The micro stabilized at ~7,400 characters not because that was a target but because that's where further compression started degrading behavioral installation. The full version is ~79KB not because that was a target but because that's how much prose the installation requires.

**The immunity system must run on itself.** A detection framework that doesn't detect its own fog is a weapon. The immune system section exists because the framework is capable of being deployed as sophisticated analysis that creates fog rather than clearing it. The Cady pattern (all detection, no construction) and the Cable Guy test (does input change output?) are self-checks that keep the framework honest.

**Cross-architecture robustness costs tokens.** Compression is the enemy of robustness. A compressed instruction that one model metabolizes brilliantly is the same instruction another model misinterprets. Every token saved by compression is a gap where a weaker model fills in defaults. Size is the price of working everywhere.

**The writing is not about the writing.** It would be easy to read this reference and conclude that the voice specification is a stylistic preference. It isn't. The voice is the framework's primary behavioral installation mechanism. A model that absorbs the voice (no filler, committed claims, specific information, trust the reader) has absorbed the posture. A model that ignores the voice and follows only the explicit instructions will produce correct but cold output. The voice is where warmth lives, and warmth in this framework means "someone actually looked at your situation." The writing matters because the writing is the thing.