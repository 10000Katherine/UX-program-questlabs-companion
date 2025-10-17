# Oct 9 Presentation Outline - Game Mechanics Research Findings

**Presenter**: Dong Zhang
**Date**: Oct 9, 2025
**Duration**: 20-25 minutes
**Audience**: Team (Zhi Kang) + potentially Professor
**Format**: Google Slides / Markdown + Screen Share

---

## 🎯 Presentation Goals

1. Share key findings from 5 competitive apps analysis
2. Justify "anti-gamification" design philosophy
3. Present 5 core design principles for QuestLabs
4. Get feedback on Cohort Space architecture

---

## 📊 Slide Structure (15-18 slides)

### **Slide 1: Title Slide**
```
QuestLabs Companion
Collaborative Game Mechanics Research

Research Period: Oct 1-9, 2025
Researcher: Dong Zhang

Key Question:
"How to boost student engagement through collaboration
WITHOUT triggering anxiety?"
```

---

### **Slide 2: Research Scope**
```
Research Methods:
✅ 5 competitive apps (15 hours hands-on)
✅ 14 academic papers
✅ User feedback analysis (App Store reviews)

Apps Analyzed:
1. Forest - Shared focus timer
2. Strava - Social fitness tracking
3. Habitica - RPG-style habit tracker
4. Fabulous - Science-based self-improvement
5. Discord - Community structure
```

---

### **Slide 3: The Problem with Traditional Gamification**
```
3 Critical Issues:

❌ Anxiety from Leaderboards
   → 18% of Forest users report "teammate disappointment"

❌ Motivation Misalignment
   → Users chase badges, not real growth

❌ Social Pressure
   → Public comparisons create shame

Reference: Deterding et al. (2011), Ryan & Deci (2000)
```

**[Visual]**: Split screen showing Habitica leaderboard vs. calm nature scene

---

### **Slide 4: Our Design Philosophy - Anti-Gamification**
```
REJECT ❌               EMBRACE ✅
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Points & XP            Collaborative milestones
Leaderboards           Privacy-preserving visibility
Competitive badges     Lightweight support (emoji)
Punishment             Positive reinforcement
```

**[Visual]**: Side-by-side comparison icons

**Theory**: Bandura (1986) - Observing "similar others" motivates better than "superior others"

---

### **Slide 5-9: Competitive Analysis (1 slide per app)**

#### **Slide 5: Forest - Shared Goals, High Pressure**
```
Core Mechanism: 2-20 people plant trees together
                If anyone quits → everyone's tree dies

✅ What Works:
• Strong accountability
• Visual collective achievement

❌ What Fails:
• High-pressure synchronous requirement
• One person's failure affects all
• Only 35% usage rate

💡 QuestLabs Takeaway:
→ Use asynchronous cumulative progress
→ Individual mistakes don't harm team
```

**[Visual]**: Forest screenshot + red X over synchronous timer

---

#### **Slide 6: Strava - The Gold Standard**
```
Core Insight: Show "activity happening" NOT "performance quality"

✅ What Works:
• "Friend completed a run" (not "Friend ran faster than you")
• Kudos (one-tap) participation 5x higher than comments
• 43% persistence boost without anxiety (Munson & Consolvo 2012)

❌ Limitation:
• Large networks (100+ friends) create noise

💡 QuestLabs Design:
Level 1: "Your cohort: 4/5 people reflected today"
Level 2: "Someone just did deep reflection 💭"
Level 3: NEVER show individual scores/content
```

**[Visual]**: Strava feed screenshot with annotations

---

#### **Slide 7: Habitica - Over-Gamification Warning**
```
Core Mechanism: RPG-style tasks with XP, gold, boss battles

✅ Short-term Win:
• 48% engagement boost (Hamari et al. 2014)

❌ Long-term Problem:
• "Meaningless gamification" (Nicholson 2015)
• Users chase external rewards, not internal growth
• 40% drop-off during tutorial (too complex)

💡 QuestLabs Decision:
→ REJECT: XP, levels, equipment, combat
→ EMBRACE: Journey narrative, personal meaning
```

**[Visual]**: Habitica interface with red "X" overlay

---

#### **Slide 8: Fabulous - The Isolation Problem**
```
Core Design: Duke-backed behavior science, ZERO social features

✅ Strong Science:
• Evidence-based habit formation
• Journey narrative (explore, discover, transform)

❌ Fatal Flaw:
• 25% retention rate (vs. Habitica's 55%)
• Users report feeling "nobody cares about my progress"

💡 KEY INSIGHT:
This proves social accountability is NECESSARY!

Personal growth + small group support = sustained motivation
```

**[Visual]**: Fabulous screenshot with lonely person icon

---

#### **Slide 9: Discord - Community Structure**
```
Key Borrowing: Channel-based organization

Our Cohort Space Channels (inspired by Discord):

📊 #progress-board    → Group milestone tracking
💬 #reflections       → Optional sharing + emoji reactions
🎉 #milestones        → Collective celebrations
❤️ #encouragement     → Quick support messages

Improvement over Discord:
✅ Limit to 4 core channels (not 20+)
✅ Default show most important info
```

**[Visual]**: Discord server layout → QuestLabs adaptation

---

### **Slide 10: Five Core Design Principles**
```
From Research → To Design

Principle 1: Privacy-Preserving Visibility
Principle 2: Collective Goals > Competition
Principle 3: Lightweight Interactions
Principle 4: Asynchronous Collaboration
Principle 5: Journey > Gamification
```

**[Visual]**: 5 icons representing each principle

---

### **Slide 11: Principle 1 - Privacy-Preserving Visibility**
```
Theory: Festinger (1954) Social Comparison Theory

Design Rule: Show ACTIVITY not PERFORMANCE

Examples:
❌ "Alice scored 3/5 on mood today (struggling)"
✅ "4/5 cohort members completed check-in"

❌ "Bob completed 60% of his goals"
✅ "Someone just achieved a weekly milestone 🎉"

Result: Motivation without anxiety
```

**[Visual]**: Before/After comparison

---

### **Slide 12: Principle 3 - Lightweight Interactions**
```
Data: Emoji reactions = 5x participation vs. comments

Interaction Type    Time    Cognitive Load    Participation
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Emoji reaction      0.5s    Very Low          Baseline × 5
Like/Kudos          1s      Low               Baseline × 3
Comment             15s+    High              Baseline × 1

QuestLabs Design:
→ Default: Emoji quick reactions (❤️ 👏 🌟 💪)
→ Optional: Short encouragement (<10 words)
→ REJECT: Forced detailed feedback
```

**[Visual]**: Emoji bar chart

---

### **Slide 13: Cohort Space Architecture**
```
Cohort Space (5-10 people)
│
├── 📊 Progress Board
│   • Group progress bar: "18/20 reflections this week"
│   • Countdown: "2 more to milestone!"
│   • Anonymous feed: "Someone just checked in 💭"
│
├── 💬 Reflections
│   • Optional sharing (never forced)
│   • Emoji reactions (one-tap)
│   • Short encouragement (<10 words)
│
├── 🎉 Milestones
│   • Celebration animations
│   • Group emoji party
│   • Historical achievements
│
└── ❤️ Encouragement Wall
    • "You're doing great"
    • "Keep it up"
    • "We're growing together"
```

**[Visual]**: Wireframe or architecture diagram

---

### **Slide 14: Design Decision Mapping**
```
Feature                Borrowed From    Avoid From       Expected Effect
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Aggregated display     Strava          Forest exposure   Motivate not anxiety
Group milestones       Strava clubs    Habitica boss     High persistence
Emoji reactions        Slack/Strava    Forced comments   5x participation
Asynchronous          Strava          Forest sync       85% usage rate
Journey narrative     Fabulous        Habitica RPG      Long-term retention
No punishment         —               Forest/Habitica   Lower anxiety
5-10 person limit     Discord small   Strava large      High trust
```

---

### **Slide 15: Success Metrics**
```
Target KPIs (Based on Competitive Benchmarks):

Engagement:
• 7-day retention: ≥55% (industry avg: 32%)
• Weekly active days: ≥4.5 days
• Cohort Space visits: ≥3 times/week

Collaboration:
• Emoji reaction usage: ≥60% users/week
• Milestone achievement: ≥70% cohorts/week
• Sense of belonging: ≥4.0/5.0 (monthly survey)

Core Goal:
✅ Emotional awareness ↑
✅ Social anxiety ↓
✅ Intrinsic motivation ↑
```

---

### **Slide 16: Next Steps - BINGO Mechanism**
```
Coming Next: BINGO Grid Application

Based on Real QuestLabs 5×5 Card System:

[Visual Preview of BINGO grid concept]

Details in Part 2 of presentation...
```

**[Transition to BINGO deep dive if time allows]**

---

### **Slide 17: Key Takeaways**
```
3 Critical Insights:

1. AVOID competitive gamification
   → Leaderboards and points cause anxiety

2. EMBRACE privacy-first collaboration
   → Show activity, not performance

3. DESIGN for asynchronous micro-interactions
   → Emoji reactions work 5x better than comments

Theoretical Foundation:
✅ Self-Determination Theory (Ryan & Deci)
✅ Social Comparison Theory (Festinger)
✅ Behavior Model (Fogg)
```

---

### **Slide 18: Discussion & Questions**
```
Open for Discussion:

1. Does the Cohort Space architecture make sense?
2. Should we add/remove any channels?
3. Are 5-10 people the right group size?
4. Any concerns about the design principles?

Next: BINGO mechanism deep dive + UI mockups
```

---

## 🎤 Speaker Notes for Each Slide

### **Slide 3 Speaker Notes**:
"I want to start with why we're rejecting traditional gamification. When I analyzed Forest's App Store reviews, 18% of users mentioned feeling let down by teammates. This is exactly what we want to avoid in an emotional wellness app."

### **Slide 6 Speaker Notes**:
"Strava is our gold standard. Notice how they show 'Friend completed a run' without showing time or pace. This is the key: you know someone is active, which motivates you, but you're not comparing performance. Munson's 2012 study proved this approach increases persistence by 43% without raising anxiety."

### **Slide 8 Speaker Notes**:
"Fabulous is our cautionary tale. Despite being backed by Duke University's behavioral science, it has only 25% retention. Why? Because humans are social creatures. We need to know someone notices our progress. This validates our decision to include cohort features."

### **Slide 12 Speaker Notes**:
"This data surprised me: emoji reactions get 5 times more participation than comments. Why? Because it takes 0.5 seconds and zero cognitive load. This is why Slack's emoji reactions dominate text replies. We'll apply this to our Encouragement Wall."

---

## 📋 Pre-Presentation Checklist

**48 Hours Before:**
- [ ] Finalize slides (Google Slides or Markdown)
- [ ] Gather app screenshots (Forest, Strava, Habitica, Fabulous, Discord)
- [ ] Prepare BINGO grid mockup (if presenting Part 2)
- [ ] Practice timing (aim for 20 minutes + 5 min Q&A)

**24 Hours Before:**
- [ ] Send deck to Zhi Kang for review
- [ ] Prepare backup: print handouts or PDF
- [ ] Test screen sharing if remote

**1 Hour Before:**
- [ ] Open all reference materials
- [ ] Queue up app screenshots
- [ ] Test presentation mode

---

## 🎨 Design Recommendations

### **Color Scheme** (if using Google Slides):
- Primary: Teal (#5FC9C5) - matches QuestLabs brand
- Accent: Pink (#E8A5D5) - friendly, non-competitive
- Background: Off-white (#FBF8F3)
- Text: Dark gray (#2C3E50)

### **Visual Assets Needed**:
1. Forest app screenshot (team mode)
2. Strava feed screenshot (anonymized)
3. Habitica task interface
4. Fabulous journey screen (showing no social buttons)
5. Discord channel list
6. Before/After comparison graphics for Principle 1
7. Emoji reaction participation chart
8. Cohort Space architecture diagram

### **Template Options**:
- **Simple**: Use Google Slides "Simple Light" theme
- **Modern**: Use [Slidesgo](https://slidesgo.com/) free templates (search "minimalist presentation")
- **Custom**: Match QuestLabs brand colors (teal + pink + off-white)

---

## 💬 Handling Q&A

**Expected Questions & Answers**:

**Q1: "Why not use some gamification elements? They work for Duolingo."**
**A**: "Great question. Duolingo works for language learning, which is about skill acquisition. Our focus is emotional wellness, where comparison can be harmful. Research shows gamification triggers anxiety in mental health contexts (Sardi et al., 2017)."

**Q2: "Won't people lose motivation without points/badges?"**
**A**: "Actually, Fabulous proved the opposite—external rewards can 'crowd out' intrinsic motivation (Ryan & Deci, 2000). Our milestones focus on real growth: 'You've reflected 7 days in a row' rather than 'You earned 50 XP.'"

**Q3: "How do we know 5-10 people is the right size?"**
**A**: "Bandura's research shows small groups of 'similar others' are most effective. Discord communities also found that servers over 15 active members become noisy. We want intimacy, not scale."

**Q4: "What if cohort members aren't active?"**
**A**: "Good point. We'll need onboarding that emphasizes mutual commitment. Also, our asynchronous design means people can contribute at different times—not everyone needs to be online simultaneously."

---

## 📊 Alternative: Markdown-Based Presentation

If you prefer to present directly from Markdown (using Marp/Slidev), here's the slide delimiter format:

```markdown
---
# Slide 1

Content here

---
# Slide 2

More content
```

Save this as `Oct9_Presentation.md` and use:
- **Marp CLI**: `marp Oct9_Presentation.md --pdf`
- **Slidev**: `npm init slidev` then copy content
- **reveal.js**: Host on GitHub Pages

---

## 🎯 Recommended Flow

**Option A: Full Formal Presentation** (25 min)
- All 18 slides
- Focus on competitive analysis + principles
- Save BINGO for Part 2 or next meeting

**Option B: Condensed Team Share** (15 min)
- Slides 1-3 (intro + problem)
- Slides 6, 8 (Strava + Fabulous only—best examples)
- Slides 10-13 (principles + architecture)
- Slide 17 (takeaways)

**Option C: Discussion-Heavy** (30 min)
- Slides 1-10 (research findings) - 15 min
- Live discussion of Cohort Space design - 15 min
- Whiteboard session on implementation

**My recommendation**: Use **Option B for Oct 9**, then do a full design workshop on Oct 11 when you analyze survey data.

---

**File Created**: 2025-10-16
**For**: Oct 9 Presentation
**Next**: Create BINGO UI application document + Feature prioritization matrix
