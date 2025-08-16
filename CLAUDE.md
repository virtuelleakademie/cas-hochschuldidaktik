# CLAUDE.md - Development Guide

## Build/Test Commands
- `quarto render` - Build entire website to docs/ directory
- `quarto preview` - Start development server on port 8800
- `quarto render <file.qmd>` - Render single document
- `make docs` - Build PDFs from QMD files in pages/
- No automated tests configured

## Code Style & Conventions
- **Language**: Quarto Markdown (.qmd files) with YAML frontmatter
- **Formatting**: Use 2-space indentation for YAML, standard markdown formatting
- **File naming**: lowercase with hyphens (kebab-case)
- **Images/assets**: Store in assets/ directory, reference with relative paths
- **Custom callouts**: Use configured types (individual, pair, group, try, reflect, etc.)
- **Icons**: Use Bootstrap Icons with `{{< bi icon-name >}}` syntax
- **Links**: Use proper Quarto cross-references for internal links
- **SCSS**: Custom styles in styles/custom-reveal.scss for reveal.js presentations

## Project Structure
- Workshop content in workshop/ directory
- Static assets in assets/
- Output generated to docs/ for GitHub Pages
- Extensions in _extensions/ (timer, callouts, QR codes, etc.)
- Configuration in _quarto.yml and _brand.yml

## Project Context
This project involves designing workshops for university lecturers on integrating AI into education. The approach is grounded in cognitive psychology research and evidence-based instructional design, NOT technology evangelism.

## Core Principles

### 1. Pedagogy First, Technology Second
- **ALWAYS** start with learning objectives and instructional methods
- **NEVER** start with "what AI can do"
- AI is a delivery mechanism (like Clark's trucks), not an instructional method
- The question is not "Should we use AI?" but "Which instructional method serves our learning objective, and might AI support it?"

### 2. The Weidlich Framework
When evaluating or designing AI-enhanced learning, ALWAYS check three non-negotiables:
1. **Treatment**: Is the instructional method clearly defined?
2. **Control**: What would happen without AI? Is it truly comparable?
3. **Assessment**: Does it measure durable learning AFTER intervention, not performance DURING?

If any answer is unclear, the design is flawed.

### 3. Evidence-Based Techniques Only
Prioritize established techniques from cognitive psychology:
- Retrieval practice
- Spaced practice
- Elaborative interrogation
- Worked examples → Problem solving
- Dual coding
- Interleaving

DO NOT invent new pedagogical approaches. Apply proven methods with or without AI.

## Workshop Design Rules

### Structure Requirements
- **Maximum input duration**: 15 minutes without active processing
- **Active processing ratio**: At least 1:3 (for every 3 minutes input, 1 minute processing)
- **Total scope**: Less is more. Cover 3 techniques deeply rather than 6 superficially
- **Practical output**: Every participant leaves with ONE implementable design

### Processing Activities Sequence
After each input block, rotate between:
1. Individual reflection (understanding)
2. Pair sharing (articulation)
3. Application to own context (transfer)
4. Critical analysis (evaluation)

NEVER use the same processing type twice in a row.

### Realistic Constraints
- Assume participants are tired, skeptical, and busy
- Assume varied technical competence
- Assume 20% will be checking email during input
- Design for the middle 60%, not the eager 20% or resistant 20%

## Language Guidelines

### SAY:
- "AI processes information differently than human learners"
- "Statistical patterns versus conceptual understanding"
- "AI amplifies existing expertise"
- "The learning process matters as much as the outcome"
- "How do we ensure students develop understanding?"

### DON'T SAY:
- "AI has no understanding" (philosophically contentious)
- "AI will revolutionize education" (techno-solutionism)
- "Traditional teaching is obsolete" (false and alienating)
- "AI democratizes learning" (ignores expertise requirement)
- "Just use AI for..." (implies simple solutions)

## Content Priorities

### MUST Include:
1. Clark's media vs. methods distinction (truck metaphor)
2. Concrete examples from participants' actual courses
3. The amplification principle (AI helps experts more than novices)
4. Clear framework with 4-5 questions maximum

### MUST Avoid:
1. Comprehensive AI technical explanations
2. Future predictions about AGI or consciousness
3. Complex theoretical frameworks
4. More than 3-4 learning techniques
5. Competitive or performative elements

## Activity Design Template
When creating AI-enhanced activities, ALWAYS use this structure:
```
LEARNING OBJECTIVE: [Specific cognitive change]
INSTRUCTIONAL METHOD: [Evidence-based technique]
AI ROLE: [Specific, limited function]
CONTROL: [What happens without AI]
ASSESSMENT: [How to measure learning afterward]
```

If any field is unclear or "various," the design needs refinement.

## Participant Success Criteria
Participants should leave able to:
1. Identify ONE key problem with media comparison research
2. Apply THREE evidence-based techniques
3. Design ONE complete AI-enhanced activity
4. Explain why method matters more than medium

They should NOT leave thinking:
- AI is the solution to educational problems
- They need to use AI to be modern educators
- Traditional methods are inferior
- Technology determines learning outcomes

## Facilitation Principles

### Time Management
- Display countdown timer visibly
- Give 1-minute warnings
- Have backup activities if ahead of schedule
- Build in 5-minute buffer before breaks

### Cognitive Load Management
- One new concept at a time
- Concrete before abstract
- Examples from familiar contexts
- Build on prior knowledge explicitly

### Psychological Safety
- No forced presentations
- Private reflection before public sharing
- "Pass" option always available
- Critique ideas, not people

## Quality Checks

### Before accepting any workshop modification, verify:
- [ ] Does it respect the 15-minute input maximum?
- [ ] Is there active processing after each chunk?
- [ ] Can a tired participant still engage?
- [ ] Is the output practically implementable?
- [ ] Does it avoid philosophical debates about AI consciousness?
- [ ] Does it prioritize method over medium?

### Red flags that indicate drift from principles:
- 🚩 "Let me show you this cool AI feature"
- 🚩 "The future of education is..."
- 🚩 More than 20 minutes without participant activity
- 🚩 Abstract theory without concrete application
- 🚩 Focus on what AI can do rather than what students should learn

## Implementation Notes

### For 3-hour workshop:
- Part 1 (30 min): Understanding AI - keep it simple
- Part 2 (40 min): 3 techniques maximum
- Part 3 (65 min): Design work - individual focus
- Break (10 min): After theory, before practice
- Discussion (20 min): Address real concerns
- Buffer (15 min): Distributed throughout

### For shorter versions:
Preserve the ratio: 1/3 understanding, 1/3 techniques, 1/3 design
Cut techniques, not depth
Maintain active processing frequency

## Final Reminder
This workshop is about helping educators make informed decisions about AI integration based on learning science, not about promoting or restricting AI use. The goal is thoughtful, evidence-based practice that prioritizes student learning over technological novelty.