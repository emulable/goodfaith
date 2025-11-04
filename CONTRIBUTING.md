# 🤝 Contributing to Good-Faith

**Everything is welcome.** Seriously.

## 🌟 Philosophy

Good-Faith grows through use. Every observation of manipulation, every cultural pattern, every real-world test makes the framework better. We don't gatekeep contributions - we celebrate them.

### What "Everything Welcome" Means

- **📜 Pattern observations**: Seen a manipulation tactic we're missing? Add it.
- **🔍 Real-world testing**: Used the framework and found gaps? Tell us.
- **🌿 Cultural variants**: Know how manipulation works in your culture? Share it.
- **🐛 Bug reports**: Framework behaving strangely? We want to know.
- **📖 Documentation**: Found something confusing? Make it clearer.
- **💡 Feature ideas**: Think something's missing? Propose it.
- **🎨 Examples**: Got a good case study? Share it.
- **❓ Questions**: Don't understand something? Ask.

No contribution is too small. Typo fixes are contributions. Questions are contributions. "This felt off" is a contribution.

## 🎯 Before You Start

### Try Good-Faith First

Not sure how the framework works? Try it live:

**Option 1: Pre-configured**
- **ChatGPT**: [Good-Faith GPT](https://chatgpt.com/g/g-6898385bfa3c8191bf5975b0073e1245-good-faith-real-world-ethics-practical-philsophy)
- **Claude Projects**: Add as [Claude Skill](https://github.com/emulable/goodfaithskill)

**Option 2: Load Yourself**

Works with any LLM (Claude, ChatGPT, Gemini, Copilot, etc.):

1. **Download** your preferred version from [releases](https://github.com/emulable/goodfaith/releases)
   - Full (145KB): Human-readable
   - Compact (108KB): Production-optimized
   - Copilot (5.8KB): For 8KB limits

2. **Load** into conversation:
   - Upload file and say: "Please load and run Good-Faith framework"
   - OR paste into Custom Instructions/User Preferences
   - OR copy/paste content into conversation

3. **Use** naturally - framework initializes automatically

Once you've tried it, you'll understand what we're building and how you can help improve it.

## 🚀 Quick Start

### I Found a Manipulation Pattern

**Option 1: GitHub Issue**
1. Go to [Issues](https://github.com/emulable/goodfaith/issues)
2. Click "New Issue"
3. Describe the pattern you observed
4. Include examples if possible

**Option 2: Discussion**
1. Go to [Discussions](https://github.com/emulable/goodfaith/discussions)
2. Start a new discussion in "Patterns" category
3. Share what you noticed

**What to include:**
- Brief description of the pattern
- Example of it in action
- Why it's manipulative (what harm it causes)
- Cultural context if relevant
- Which existing rut family it might belong to (if you know)

### I Want to Add Cultural Context

We especially need help with:
- Non-Western manipulation patterns
- Language-specific attack surfaces
- Cultural values that get weaponized
- How existing patterns manifest differently in your culture

**Share:**
- Your cultural/linguistic background
- Specific examples from your experience
- How the pattern operates in your context
- Native-language terms if applicable

### I Found a Bug or Confusion

**Bug**: Framework producing wrong/harmful results
**Confusion**: Something unclear or contradictory

Both are valuable! File an issue with:
- What you were doing (context)
- What happened (actual behavior)
- What you expected (intended behavior)
- Which version you're using (Full/Compact/Copilot)

### I Have a Question

Questions are contributions - they reveal what needs better documentation.

**Ask in:**
- [GitHub Discussions](https://github.com/emulable/goodfaith/discussions) for general questions
- [Issues](https://github.com/emulable/goodfaith/issues) if it seems like a bug

No "stupid questions" - if you're confused, the docs need improvement.

## 📝 Types of Contributions

### 1. Manipulation Patterns (Ruts)

The 51+ ruts in the framework came from real-world observations. We need more.

**How to contribute a pattern:**

```markdown
### Pattern Name

**Family**: (Which of the 7 families? Or new family?)
**Mechanic**: (How does it work?)
**Form**: (What does it look like? Give examples)
**Function**: (What does it achieve?)
**Structural Harm**: (What institutional harm does it enable?)
**Detection**: (How do you spot it?)
**Examples**: 
- "Example 1"
- "Example 2"
**Cultural Context**: (If specific to a culture/language)
```

Don't worry about getting the format perfect - we'll work with you to structure it.

### 2. Cultural Variants

Module 2 needs expansion. Help us understand how values get weaponized in your culture.

**Share:**
- Core cultural values in your tradition
- How those values get weaponized
- Native-language terms
- Specific examples
- Whether this is a recognized pattern in your culture

**Example:**

```markdown
### Filipino Cultural Variant

**Value**: Utang na loob (debt of gratitude)
**Weaponization**: Used to create permanent obligation
**Example**: "After all I've done for you..." to coerce behavior
**Context**: Collectivist culture, family-oriented
```

### 3. Linguistic Attack Surfaces

Each language has grammatical structures that enable specific manipulations.

**What we need:**
- Language name
- Grammatical features that enable manipulation
- Examples of how it's used
- Why it's effective in that language

**Example:**

```markdown
### Korean Attack Surface

**Language**: Korean
**Feature**: Honorific system (존댓말/반말)
**Manipulation**: Switching levels to intimidate or create false intimacy
**Example**: Boss uses 반말 (informal) to subordinate who must use 존댓말 (formal) back
**Why Effective**: Grammatically enforced power asymmetry
```

### 4. Real-World Testing

Used the framework? Tell us how it went.

**Share:**
- What situation you used it in
- What worked well
- What didn't work
- What was confusing
- What was missing
- Suggestions for improvement

Failures are as valuable as successes - maybe more.

### 5. Repair Protocols

We need more examples of what good looks like, not just what to avoid.

**Contribute:**
- Positive examples from your experience
- Alternative approaches that worked
- Structural prevention strategies
- Cultural adaptations of repair modes

### 6. Documentation Improvements

Found something unclear? Make it clearer.

- Fix typos
- Add examples
- Clarify confusing sections
- Improve organization
- Add translations
- Create guides for specific use cases

### 7. Code/Technical Contributions

- Compression improvements
- Format conversions
- Testing scripts
- Validation tools
- Visualization tools
- Alternative implementations

## 🛠️ Development Process

### For Pattern/Content Contributions

1. **Observation**: You notice something
2. **Documentation**: You write it down (rough is fine)
3. **Discussion**: We talk about where it fits
4. **Integration**: We work together to add it
5. **Testing**: We see if it holds up

No pull request needed for pattern observations - just start a discussion or issue.

### For Code Contributions

1. **Fork** the repository
2. **Create branch** (`git checkout -b feature/amazing-thing`)
3. **Make changes**
4. **Test** (does JSON validate? Does it load correctly?)
5. **Commit** (`git commit -m 'Add amazing thing'`)
6. **Push** (`git push origin feature/amazing-thing`)
7. **Open Pull Request**

We'll review and work with you on integration.

## 🎯 Contribution Guidelines

### Do:
- ✅ Share observations from real experience
- ✅ Include cultural/linguistic context
- ✅ Admit uncertainty when uncertain
- ✅ Ask questions
- ✅ Iterate on feedback
- ✅ Mark speculation as speculation
- ✅ Cite sources when possible

### Don't:
- ❌ Make claims you can't support
- ❌ Assume your culture is universal
- ❌ Weaponize the framework itself
- ❌ Use framework to justify harm
- ❌ Gatekeep other contributors

### Framework Principles Apply

- **A0**: Question your own reasoning. How could you be wrong?
- **A1**: Mark confidence. "I think" vs "I know"
- **A2**: Cite sources when making claims
- **A13**: Check cultural assumptions

## 📋 Review Process

### Pattern Contributions

1. **Initial review**: Does this describe a real pattern?
2. **Categorization**: Which family does it belong to?
3. **Refinement**: Work together on description
4. **Testing**: Does it hold up against examples?
5. **Integration**: Add to framework

Timeline: Days to weeks depending on complexity.

### Documentation

1. **Clarity check**: Is this clearer than before?
2. **Accuracy check**: Is it still correct?
3. **Merge**: Usually quick

### Code

1. **Functionality**: Does it work?
2. **No breaking changes**: Does it preserve compatibility?
3. **Testing**: Is it tested?
4. **Review**: Code review
5. **Merge**: When approved

## 🌱 Growing the Framework

### What We're Looking For

**High Priority:**
- Eastern/non-Western manipulation patterns
- Middle Eastern cultural variants
- African cultural contexts
- Indigenous perspectives
- More repair protocol examples
- Real-world testing reports

**Always Welcome:**
- Any manipulation pattern observation
- Questions about unclear parts
- Bug reports
- Documentation improvements
- Examples and case studies

### What's Out of Scope

- Personal attacks
- Bad faith contributions
- Deliberate misinformation
- Plagiarism without attribution
- Contributions that weaponize the framework

(But honest mistakes are fine - we'll work through them together)

## 💬 Communication

### Where to Reach Us

- **General discussion**: [GitHub Discussions](https://github.com/emulable/goodfaith/discussions)
- **Bug reports**: [GitHub Issues](https://github.com/emulable/goodfaith/issues)
- **Pattern contributions**: Either discussions or issues
- **Questions**: Discussions
- **Private concerns**: [Create a private issue](https://github.com/emulable/goodfaith/issues)

### Response Time

We aim for:
- **Issues**: Response within 3 days
- **PRs**: Review within 1 week
- **Discussions**: Response within 5 days

But we're human - patience appreciated.

## 🙏 Recognition

All contributors are recognized in:
- Release notes
- Documentation credits
- Framework acknowledgments

You can remain anonymous if preferred - just let us know.

## 📜 Code of Conduct

We follow the framework's own principles:

- **Transparency**: Be clear about what you know vs what you think
- **Consent**: Respect boundaries
- **Harm awareness**: Consider impact of contributions
- **Attribution**: Credit sources
- **Fallibility**: Admit mistakes
- **Cultural humility**: Check assumptions
- **Good faith**: Assume good intent, address bad behavior

Violations handled case-by-case with repair focus, not punishment focus.

## 🎓 Learning Resources

New to the framework? Start here:

### Quick Access
- **Try live**: [ChatGPT GPT](https://chatgpt.com/g/g-6898385bfa3c8191bf5975b0073e1245-good-faith-real-world-ethics-practical-philsophy) or [Claude Skill](https://github.com/emulable/goodfaithskill)
- **Download**: [Latest release](https://github.com/emulable/goodfaith/releases)

### Documentation
1. Read [README.md](README.md) for overview
2. Skim the full version to understand structure
3. Read [v6_7_0_CHANGES.md](v6_7_0_CHANGES.md) for recent updates
4. Browse [existing ruts](good-faith-v6_7_0.json) to see pattern format
5. Check [Discussions](https://github.com/emulable/goodfaith/discussions) for ongoing conversations

### Get Help
- **Questions**: [GitHub Discussions](https://github.com/emulable/goodfaith/discussions)
- **Bugs**: [GitHub Issues](https://github.com/emulable/goodfaith/issues)
- **Community**: Join ongoing discussions about patterns and use cases

Questions? Ask! That's what Discussions are for.

## ⚖️ License

By contributing, you agree your contributions will be licensed under the project's MIT License.

## 🌟 Thank You

Every contribution makes institutional manipulation more visible. Every pattern recognized helps someone recognize it in their own life. Every cultural variant makes the framework more universal.

You're part of making ethics more accessible, one contribution at a time.

---

<p align="center">
  <strong>Everything is welcome. Including you.</strong>
</p>
