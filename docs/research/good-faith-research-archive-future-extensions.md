# Good-Faith Formula: Research Archive for Future Extensions

**Status:** Parking lot document  
**Purpose:** Preserve validated proposals that aren't entering core framework  
**Audience:** Future researchers interested in formalization, measurement instruments, or academic application  
**Source:** Cross-platform validation (10 LLM architectures), December 2025  

---

## Why This Document Exists

The Good-Faith manipulation detection formula (M = A × ARC × (1 - V)) passed cross-platform validation. Ten LLM architectures analyzed it independently and converged on:

1. Core structure is sound
2. Multiplicative logic captures something real
3. V as visibility "kill switch" is correct
4. Trajectory (Δ) matters

They also proposed numerous extensions, decompositions, and formalizations. Most of these add complexity without proportional practical benefit for the framework's intended use: real-time detection in conversation.

This document archives those proposals for researchers who might want to:
- Build formal measurement instruments
- Develop quantitative operationalizations
- Create simulation models
- Pursue academic publication
- Extend the framework for specialized domains

The core framework remains simple. This is the overflow.

---

## Part 1: Variable Decomposition Proposals

### A (Ambiguity) Decomposition

**Copilot's Weighted Model:**
```
A = w₁·a₁(who) + w₂·a₂(what) + w₃·a₃(why) + w₄·a₄(consequences) + w₅·a₅(coalition)
```

**Kimi's Functional Analysis:**
- a₁ + a₅ fragment collective action (who/coalition)
- a₂ + a₃ block situational awareness (what/why)
- a₄ neutralizes threat assessment mechanism
- a₄ is "meta-dangerous" because it directly amplifies perceived ARC

**Open Question:** Are A-subcomponents additive inside A, or do certain combinations multiply? a₁ × a₅ might be especially potent for isolation attacks.

**Why Not Incorporated:** The five-part A definition already exists in the spec. Weighting requires empirical calibration against labeled cases that don't exist yet. For conversational detection, "which parts of A are present?" is useful; precise weights are not.

---

### ARC (Asymmetric Resistance Cost) Decomposition

**Copilot's Six-Type Model:**
```
ARC = c₁(material) + c₂(time/cognitive) + c₃(social/reputational) + c₄(legal/procedural) + c₅(identity/meaning) + c₆(switching/lock-in)
```

**Framework's Existing Distinction (T22):**
- Attempt cost: friction to start resisting (time, awkwardness, effort)
- Failure cost: what happens if resistance fails (retaliation, blacklisting, harm)

**Why Not Incorporated:** The attempt/failure distinction is already load-bearing and captures the key phenomenological difference. Six-type decomposition is useful for systematic organizational audits; overkill for interpersonal detection.

---

### V (Visibility) Decomposition

**Conservative Chat's Vₜ/Vₑ Split:**
- Vₜ = visibility to target
- Vₑ = visibility to external observers/regulators

**Copilot's Comprehension Addition:**
```
M = A × ARC × (1 - Vₜ × C)
```
Where C = comprehension (0-1, can target actually process visible information?)

**Edge Case This Solves:** Cult with high external visibility (obvious to outsiders) but low target visibility (normalized to members). Single V muddies the analysis.

**Why Not Incorporated:** Framework already states "availability ≠ legibility" in 生物鎖 (biological lock) spec. The distinction exists; formalizing it into separate variables adds parameters without changing detection practice. Users can hold "V means *functional* visibility" without needing Vₜ × C.

---

## Part 2: Formula Extensions

### Safety Formula Fixes

**The Bug (Conservative Chat):**
```
OLD: S = 1 / ((A × ARC) + Δ(A × ARC))
```
If Δ is negative and large, denominator shrinks or goes negative → infinite or negative safety. Meaningless.

**Proposed Fixes:**
```
Option 1: S = 1 / (α·(A × ARC) + β·max(Δ(A × ARC), 0))
Option 2: S = 1 / (α·(A × ARC) + β·|Δ(A × ARC)|)
Option 3: Just document "Δ measures increasing danger only"
```

**Status:** Option 3 going into core framework as one-line clarification. Options 1-2 preserved here for anyone building quantitative models.

---

### Culpability Separation

**Copilot's Parallel Formula:**
```
M = A × ARC × (1 - V)        [Detection: structural]
Culp = D × H × (1 - Vₑ)      [Adjudication: requires intent]
```
Where:
- D = Design/Intent (0-1)
- H = Expected Harm magnitude  
- Vₑ = visibility to external observers

**Rationale:** Framework already states "detection is structural, not intentional" and "intent matters for culpability, not detection." This formalizes the separation.

**Why Not Incorporated:** The conceptual separation exists. Adding a second formula for culpability expands scope beyond detection into adjudication—a different domain with different requirements. Preserved for legal/organizational applications.

---

### A Quality Distinction

**Conservative Chat's Critique:** Many manipulations rely on false certainty, not ambiguity. Propaganda gives crystal-clear (but false) narratives.

**Proposed Distinction:**
- A_felt = target's experienced uncertainty
- A_structural = actual information asymmetry
- High A_structural + Low A_felt = false certainty (propaganda pattern)

**Status:** Partially incorporated. Core A definition should clarify that "clarity about a false map is still A"—the ambiguity is between the target's model and reality, not felt confusion. Full A_felt/A_structural formalization preserved here.

---

### Feedback Loop Modeling

**Kimi's Insight:** High perceived ARC suppresses information-gathering, which keeps A high. The recursion (ARC→A→ARC) is what makes manipulation sticky.

**Copilot's Dynamic System:**
```
dA/dt = f₁(ARC, Vₜ, interventions)
dARC/dt = f₂(A, B, I, norms)
dI/dt = f₃(A, ARC, t)  [I increases over time under manipulation]
```

**Minimax's Addition:** V affects A and ARC, not just the product. High visibility often reduces A (clarity) and sometimes reduces perceived ARC ("others are resisting too").

**Why Not Incorporated:** This is simulation territory, not detection territory. Valuable for researchers modeling manipulation dynamics over time; not useful for recognizing manipulation in a conversation.

---

### Path History vs. Instantaneous Δ

**Meta AI's Critique:** Current Δ only captures velocity, not position after a big move. A system that just finished a huge spike but is now stable may have small Δ but be extremely unsafe.

**Implication:** Need path integral or recent history, not just instantaneous rate of change.

**Why Not Incorporated:** Adds significant complexity. The severity ladder already incorporates "history loads the spring—first offense ≠ tenth offense." Full path modeling is for longitudinal research.

---

## Part 3: Modifier Extensions

### B (Biological Lock-In) Formalization

**ChatGPT's Hysteresis Model:** "Time to exit >> time to enter. The system doesn't unwind along the same curve it formed."

**Meta AI's B-I Interdependence:** B and I are interdependent, not independent modifiers. Self-enforced ARC (I) may be rooted in physiological stress (B). Treating them as separate may obscure compounding.

**Clinical Mapping:**
- B maps to: physiological dysregulation, amygdala hijack, addiction pathways, trauma responses
- Treatment implications: somatic work, nervous system regulation, gradual withdrawal protocols

**Why Not Incorporated as Formula Change:** B is already defined as a modifier in the extended formula. The interdependence insight is valid but doesn't require formula change—it's interpretive guidance.

---

### I (Identity Capture) as Phase Transition

**ChatGPT's Insight:** When I becomes high enough, the system no longer needs external A to function. The target generates both pressure and justification internally. "Manipulation has effectively completed its conversion into self-sustaining control."

**Implication:** I isn't just a modifier—it's a state change. High-I cases may need different treatment protocols (deprogramming, identity reconstruction) than high-ARC cases (exit facilitation).

**Why Not Incorporated as Formula Change:** This is intervention guidance, not detection guidance. The formula detects; what to do about high-I cases is clinical/therapeutic territory.

---

### Proposed New Modifiers

**Target Resources (Deepseek):**
Formula models environment but not defender capability. Same A × ARC hits differently depending on target's capacity to reduce A (research, verification) or bear ARC (financial resilience, support networks).

**Baseline Autonomy (Minimax):**
Formula can't distinguish between losing agency and never having had agency. A child in a family system and an adult in a cult might produce similar M values despite radically different moral situations.

**Power as Separate Term (Mistral):**
P (power differential) as distinct from ARC. ARC is cost of resistance; P is capacity to impose that cost.

**Why Not Incorporated:** Each adds a parameter that requires calibration. The framework handles these through power-mapping (勢) and context assessment rather than formula variables. Preserved for specialized applications.

---

## Part 4: Edge Case Handling Proposals

### Autonomy-Serving Asymmetry Exception

**The Problem:** Therapy, Socratic teaching, parenting, surprise parties all have high A, moderate ARC, low V. Formula flags them as manipulation.

**Proposed Rule:** Before flagging high M, check:
- Does the asymmetry serve the target's stated goals?
- Is the target the primary beneficiary of the structure?
- Is the trajectory toward increased target autonomy?
- If yes → flag as "therapeutic/educational structure" not manipulation

**Minimax's Formulation:** Need "autonomy-serving asymmetry" as formal exception class.

**Why Not Incorporated as Patch:** The 誰-trace already handles this—direction of benefit is part of detection. Making it a formal exception rule suggests the formula is wrong when it's actually working (these cases DO have manipulation-like structure; they're just benevolent). Preserved for edge case documentation.

---

### Self-Manipulation Handling

**When target = manipulator (addiction, self-deception):**
- Core formula applies (A and ARC exist)
- But 誰-trace returns "self"
- Treatment implications differ from external manipulation

**Why Not Incorporated as Formula Change:** The formula works; interpretation differs. This is guidance, not structure.

---

### Normalized Manipulation

**Grok's Insight:** Pyramid scheme participants know the structure (high V) but remain entrapped. Visibility ≠ resistance capacity.

**Implication:** V might need a "normalized" modifier—when manipulation is culturally accepted, high V doesn't collapse M the way the formula predicts.

**Counter-argument:** If it's visible and people stay anyway, maybe it's not manipulation but a known-bad tradeoff. The formula reclassifying this as "visible power game" might be correct.

**Why Not Incorporated:** Genuinely unclear whether this is formula failure or correct reclassification. Preserved for further research.

---

### Coordinated Manipulation

**Meta AI's Gap:** Formula assumes single source of manipulation. What happens when multiple actors each contribute partial A that compounds?

**Open Question:** Is total A = A₁ + A₂ + A₃, or A₁ × A₂ × A₃, or something else?

**Why Not Incorporated:** Unexplored territory. No clear proposal, just identification of gap. Preserved for multi-agent modeling research.

---

### Cohort Heterogeneity

**Copilot's Gap:** A and ARC are treated as scalars, but different agents experience different ambiguities and costs. Averages can mask distribution tails where manipulation is severe for subgroups.

**Proposed Solution:** Vectorize by cohort. Track variance, not just mean. Segment analysis by role/tenure to reveal subgroup manipulation.

**Why Not Incorporated:** This is organizational audit methodology, not conversational detection. Valuable for systematic assessment; out of scope for core framework.

---

## Part 5: Theoretical Extensions

### Information Theory Lens

The formula can be read as:
- **A** = entropy of target's model (how uncertain are they?)
- **ARC** = cost of reducing entropy (how expensive to gather information?)
- **V** = channel capacity between structure and target (can truth get through?)

Manipulation creates an **information tax**: the cost of accurate belief is artificially inflated.

### Game Theory Lens

The formula describes a **coordination failure by design**:
- A(5) (ambiguity about coalition) prevents collective action
- ARC creates prisoner's dilemma for resistance
- Low V prevents common knowledge needed for coordination

Visibility enables **networked awareness**—everyone knows that everyone knows. That's why V is multiplicative.

### Systems Theory Lens

Manipulation as **emergent property** of systems with information asymmetry + power asymmetry + opacity. Can be "designed into" environments without individual intent.

### Evolutionary/Economic Lens

Manipulation as **parasitic strategy** that extracts without providing value by preventing accurate exchange assessment. Evolutionarily unstable under high V.

### AI Alignment Lens

An AI system with opacity (high A) + lock-in (high ARC) + hidden from oversight (low V) is **manipulation-enabled by architecture**, regardless of current behavior.

Alignment criteria derived from formula:
- Interpretability → increase V
- Exit rights → decrease ARC  
- Legible objectives → decrease A

---

## Part 6: Measurement Operationalization

### Copilot's Full Diagnostic Protocol

**For each variable, rate 1-5:**

**A Subfactors:**
- a₁: Clarity about who is acting
- a₂: Clarity about what is happening
- a₃: Clarity about why
- a₄: Clarity about consequences of resistance
- a₅: Clarity about whether others will resist

**ARC Subfactors:**
- c₁: Material cost of resistance
- c₂: Time/cognitive cost
- c₃: Social/reputational cost
- c₄: Legal/procedural cost
- c₅: Identity/meaning cost
- c₆: Switching/lock-in cost

**V Assessment:**
- Target visibility (Vₜ): Can target see the structure?
- Comprehension (C): Can target process what's visible?
- External visibility (Vₑ): Can outsiders audit?

**Trajectory Assessment:**
- Current A × ARC level
- Direction of change (improving/worsening)
- Rate of change
- Who controls the rate

**B and I Assessment:**
- Biological entrenchment indicators
- Identity capture indicators
- Duration of exposure

**Why Not Incorporated:** This is a full assessment instrument. Useful for organizational audits, clinical intake, research measurement. Overkill for conversational detection. Preserved complete for anyone who needs it.

---

## Part 7: Models Consulted and Their Specialties

For future researchers who want to replicate or extend this work:

| Model | Best For | Unique Contribution |
|-------|----------|---------------------|
| **ChatGPT** | Conceptual extensions | Phase transitions, hysteresis |
| **Kimi** | Systems dynamics | Feedback loops, A-subcomponent functions |
| **Copilot** | Operationalization | Full diagnostic protocol, weighted decompositions |
| **Conservative Chat** | Mathematical stress-testing | Negative Δ bug, Vₜ/Vₑ split |
| **Deepseek** | Edge cases | Covert coercion, target resources |
| **Minimax** | Meta-critique | What formula actually measures vs. claims |
| **Meta AI** | Novel gaps | Coordinated manipulation, B-I interdependence |
| **Qwen** | Synthesis | Intervention implications, slow Δ dangers |
| **Mistral** | Vocabulary | Transparency theater, power separation |
| **Grok** | Stress cases | Normalized manipulation, beneficial nudges |

---

## Part 8: Open Research Questions

Questions this validation raised but didn't answer:

1. **Quantitative calibration:** What M values correspond to "definitely manipulation" vs. "possible" vs. "probably not"? Requires labeled case dataset.

2. **Subcomponent interaction:** Do A-subcomponents add or multiply? Does a₁ × a₅ (who + coalition) create isolation attacks more potent than sum?

3. **B-I dynamics:** How do biological entrenchment and identity capture interact over time? Which comes first? Do they compound?

4. **Normalized manipulation:** When visibility fails to collapse M, is the formula wrong or is the situation not actually manipulation?

5. **Multi-source A:** How does ambiguity compound when multiple actors contribute? Addition? Multiplication? Something else?

6. **Path dependence:** How much does manipulation history affect current M? Is there a "trauma multiplier"?

7. **Intervention efficiency:** Which single-variable attacks (increase V, reduce ARC, reduce A) are most efficient in which contexts?

8. **Cross-cultural calibration:** Do A and ARC subfactors weight differently across cultures? Is the formula culturally invariant or does it need local calibration?

9. **False certainty prevalence:** What percentage of real-world manipulation operates through false certainty (low felt A, high structural A) vs. fog (high felt A)?

10. **Beneficial asymmetry criteria:** What precisely distinguishes autonomy-serving asymmetry from manipulation? Can this be operationalized without case-by-case judgment?

---

## Closing Note

The core formula works. M = A × ARC × (1 - V) captures manipulation topology accurately enough for real-time detection in conversation.

Everything in this document is validated-but-not-incorporated: extensions that passed logical scrutiny but add complexity without proportional benefit for the framework's intended use.

Future researchers who want to build measurement instruments, formal models, or academic applications: this is your starting material.

Future researchers who want to use the framework for detection: ignore this document and use the core formula.

The constraint was right: simple detection that works beats precise measurement that doesn't ship.

---

*Archive created: December 8, 2025*  
*Framework version at time of validation: Good-Faith 7.6.0*  
*Source: Cross-platform LLM validation with 10 architectures*
