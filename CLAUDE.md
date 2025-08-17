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
- **Lists**: Always leave an empty line above a list
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
This workshop isabout helping educators make informed decisions about AI
integration based on learning science, not about promoting or restricting AI
use. The goal is thoughtful, evidence-based practice that prioritizes student
learning over technological novelty.


# Active Processing Blocks - Complete Guide
## AI in Education Workshop

---

## Part 1: Understanding AI in Education (2 blocks)

### **Block 1: Reality Check (5 min)**
**Purpose:** Connect AI concepts to personal experience and distinguish augmentation from replacement

**Setup:** Simple reflection and pair-share

**Process:**
1. (1 min) Each person writes: "One way I currently use AI in my work"
2. (2 min) Share with neighbor, discuss specific example
3. (2 min) Together, categorize: 
   - Augmentation (AI helps thinking)
   - Replacement (AI does thinking)

**Facilitator prompts:**
- "Don't overthink - just one real example from your life"
- "Is AI helping you think better or thinking for you?"

**Expected outcomes:**
- Personal connection to material
- Recognition of the augmentation/replacement distinction
- Awareness of own AI use patterns

---

### **Block 2: Spot the Problem (5 min)**
**Purpose:** Apply Weidlich's framework intuitively before learning it formally

**Setup:** One flawed study example displayed

**The flawed study:**
> "Group A used ChatGPT for essay writing. Group B didn't. Group A scored higher. Conclusion: ChatGPT improves writing."

**Process:**
1. (2 min) Individual reading and note problems
2. (1 min) Circle/underline issues on handout
3. (2 min) Table discussion - compare identified problems

**Problems to surface:**
- What exactly did Group A do? (undefined treatment)
- What exactly did Group B do? (undefined control)
- Did students learn to write better? (performance vs. learning)
- Were other variables different? (confounding)

**Facilitator guidance:**
- "What's missing from this study?"
- "Would you accept this conclusion? Why not?"

**Bridge to next section:**
- "These instincts you have are exactly what Weidlich formalized..."

---

## Part 2: Evidence-Based Learning Principles (1 block)

### **Block 3: Pick Your Technique (10 min)**
**Purpose:** Connect abstract techniques to concrete personal practice

**Setup:** Individual work, then pair-share

**Process:**
1. (3 min) **Individual selection**
   - Review the 3 techniques just presented
   - Choose ONE that fits your teaching context
   - Consider: Which addresses your biggest challenge?

2. (4 min) **Write specific example**
   - From your actual course (next week if possible)
   - No AI involved yet - just the technique
   - Include: What students do, what you do, why this helps

3. (3 min) **Pair explanation**
   - Find one neighbor
   - Each person: 90 seconds to explain choice
   - Partner asks: "What made you choose this over the others?"

**Sample outputs:**
- Retrieval Practice: "Start each class with 3-minute brain dump of last week's content"
- Worked Examples: "Show complete problem solution before similar practice"
- Elaborative Interrogation: "Students explain WHY each step in the process matters"

**Facilitator notes:**
- Circulate and listen for good examples
- Note which techniques are most popular
- Prepare to reference these in Part 3

---

## Part 3: Designing AI-Enhanced Learning (4 blocks)

### **Block 4: Design Time (25 min)**
**Purpose:** Create one complete, implementable AI-enhanced activity

**Materials needed:**
- Design framework handout (4 questions)
- Blank paper for drafting
- Pens/pencils

#### **Phase 1 - Individual Draft (10 min)**
**Silent work time - protect this!**

**Task:** Answer four framework questions
1. What should students learn? (specific objective)
2. Which technique will you use? (from Part 2)
3. What specific role will AI play? (limited, defined)
4. How will you assess learning? (after intervention)

**Facilitator behavior:**
- Circulate silently
- Only intervene if someone looks stuck
- Use sticky notes for quiet questions

**Common struggles and solutions:**
- Too broad objective → "Make it smaller"
- Vague AI role → "What specifically does AI do?"
- Assessment during activity → "What about next week?"

#### **Phase 2 - Pair Refinement (10 min)**
**Structured peer consultation**

**Process:**
1. Find ONE partner (not a group)
2. Partner A explains (5 min):
   - Read through 4 answers
   - Partner B listens, asks clarifying questions only
   - No suggestions yet
3. Partner B explains (5 min):
   - Same process reverses
   - Focus on clarity, not judgment

**Question prompts for listeners:**
- "Can you tell me more about...?"
- "What would that look like in practice?"
- "How is that different from what you do now?"

#### **Phase 3 - Quick Polish (5 min)**
**Individual finalization**

**Task:**
- Return to own design
- Make adjustments based on partner questions
- Create one clean version
- Star (*) the part you're most excited about

---

### **Block 5: Speed Dating Feedback (10 min)**
**Purpose:** Get rapid, focused feedback without presentation anxiety

**Setup:** 
- Pairs stay at tables with their designs visible
- Visitors rotate every 2 minutes
- Timer visible to all

**Rotation schedule:**
- Rounds 1-2: "What's your learning objective?"
- Rounds 3-4: "What exactly does AI do here?"
- Round 5: "How do you assess this?"

**Rules:**
- Visitors ask their assigned question ONLY
- Designers answer in 30 seconds
- Visitors can ask ONE follow-up
- No advice giving - questions only

**Facilitator management:**
- Call rotations clearly
- Model first question if needed
- Keep energy up: "Switch! Find someone new!"

**Debrief thought:**
Each designer now has 5 perspectives on their clarity

---

### **Block 6: Harvest Key Insights (10 min)**
**Purpose:** Collective sense-making and pattern recognition

**Setup:** Table discussion → whole group share

**Process:**
1. (5 min) **Table discussion**
   - Prompt: "What surprised you most about this design process?"
   - Each table identifies ONE key surprise
   - Choose spokesperson

2. (3 min) **Rapid share-out**
   - Each table: 30 seconds maximum
   - Spokesperson shares the ONE surprise
   - No elaboration, just the insight

3. (2 min) **Pattern identification**
   - Facilitator notes patterns on board
   - "I'm hearing several groups mention..."
   - Connect back to morning principles

**Common insights that emerge:**
- "Harder to define AI's role than expected"
- "Assessment is the tricky part"
- "My technique didn't need AI"
- "AI works better for some techniques"

**Closing connection:**
- "Notice how we keep coming back to method vs. medium..."

---

## Facilitation Tips Across All Blocks

### **Time Management**
- Use a visible timer (phone/screen/timer cube)
- Give warnings: "One minute remaining"
- Have a clear sound for transitions
- Build in 30-second buffers

### **Energy Management**
- Vary sitting/standing
- Change partner configurations
- Use different processing types
- Watch for energy dips (especially after lunch)

### **Differentiation Strategies**
- **Fast finishers:** "Add a challenge variation to your design"
- **Struggling participants:** "Start with just next Monday's class"
- **Resistant participants:** "Design what NOT to do with AI"
- **Experienced AI users:** "Focus on the assessment challenge"

### **Materials Checklist**
- [ ] Framework handout (one per person)
- [ ] Flawed study example
- [ ] Blank paper for design work
- [ ] Sticky notes for insights
- [ ] Timer (visible to all)
- [ ] Board/flip chart for harvesting

### **Common Pitfalls to Avoid**
- Don't let pair shares become group discussions
- Don't allow advice-giving in speed dating
- Don't extend input to "finish the thought"
- Don't skip processing to "save time"
- Don't let one person dominate pair work

### **Recovery Strategies**
If running behind:
- Shorten pair shares by 1 minute
- Reduce speed dating rotations to 3
- Skip one elaboration in input

If running ahead:
- Add "find one more partner" to pair shares
- Include "write one question you still have"
- Do a bonus round of speed dating

If energy is low:
- Stand and stretch (30 seconds)
- Share with someone across the room
- Do a walking partner exchange

---

## Assessment of Success

### **Participants should be able to:**
- ✓ Distinguish augmentation from replacement
- ✓ Identify flaws in media comparison studies
- ✓ Apply one technique to their teaching
- ✓ Design one complete AI-enhanced activity
- ✓ Explain their design choices clearly

### **Red flags that processing isn't working:**
- 🚩 Silence during pair shares
- 🚩 Same people talking repeatedly
- 🚩 Confusion about instructions
- 🚩 Off-topic discussions
- 🚩 Rushing through without thinking

### **Signs of success:**
- ✅ Animated pair discussions
- ✅ "Aha" moments visible
- ✅ References back to earlier content
- ✅ Specific examples from own courses
- ✅ Questions that show deep thinking