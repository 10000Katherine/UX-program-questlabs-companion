# Feature Prioritization Matrix - QuestLabs Companion

**Purpose**: Rank 12 core features based on user needs, technical feasibility, and project constraints
**Framework**: Value vs. Effort Matrix + PACT Alignment + Research Data
**Created**: 2025-10-16
**For**: Oct 14 Task - Feature Prioritization
**Team**: Dong Zhang + Zhi Kang

---

## 📊 Prioritization Framework

### Three-Dimensional Scoring

Each feature rated on:
1. **User Value** (1-5): How much users need this (from survey + research)
2. **Technical Effort** (1-5): Development complexity (1=easy, 5=hard)
3. **Strategic Fit** (1-5): Alignment with "anti-gamification" philosophy

**Final Priority Score** = (User Value × 2 + Strategic Fit) - Effort
*Higher score = Higher priority*

---

## 🎯 The 12 Core Features

Based on Proposal (`F25_3375_S1_G5_Quest Labs_Proposal.md` lines 172-194):

1. Three-Layer Goal Framework (Vision → Quarterly → Weekly)
2. Daily Check-In (<2 min)
3. Weekly Planning (5-10 min)
4. Structured Reflection Journal
5. Progress Dashboard (Trend graphs)
6. Cohort Space (Aggregated peer progress)
7. Quest Board (BINGO-style task grid)
8. Wheel of Life visualization
9. Affect-Agency Grid (Polak's model)
10. SEL Timeline (Social-Emotional Learning trends)
11. Encouragement Reactions (Emoji system)
12. Milestone Celebrations

---

## 📈 Feature Scoring Matrix

| # | Feature | User Value | Tech Effort | Strategic Fit | Priority Score | Priority Tier |
|---|---------|-----------|-------------|---------------|----------------|---------------|
| 2 | **Daily Check-In** | 5 | 2 | 5 | **13** | 🔴 P0 (Must Have) |
| 6 | **Cohort Space** | 5 | 3 | 5 | **12** | 🔴 P0 (Must Have) |
| 5 | **Progress Dashboard** | 5 | 3 | 4 | **11** | 🔴 P0 (Must Have) |
| 1 | **Goal Framework** | 4 | 3 | 5 | **10** | 🟠 P1 (High Priority) |
| 7 | **Quest Board (BINGO)** | 4 | 2 | 5 | **10** | 🟠 P1 (High Priority) |
| 11 | **Emoji Reactions** | 4 | 1 | 5 | **10** | 🟠 P1 (High Priority) |
| 3 | **Weekly Planning** | 4 | 2 | 4 | **9** | 🟡 P2 (Medium Priority) |
| 8 | **Wheel of Life** | 4 | 3 | 3 | **8** | 🟡 P2 (Medium Priority) |
| 12 | **Milestone Celebrations** | 3 | 2 | 4 | **8** | 🟡 P2 (Medium Priority) |
| 4 | **Reflection Journal** | 3 | 3 | 4 | **7** | 🟢 P3 (Nice to Have) |
| 9 | **Affect-Agency Grid** | 3 | 4 | 3 | **5** | 🟢 P3 (Nice to Have) |
| 10 | **SEL Timeline** | 3 | 4 | 2 | **4** | ⚪ P4 (Future Phase) |

---

## 🔴 P0 - Must Have (MVP Core)

### Feature #2: Daily Check-In (<2 min)

**Score: 13 (Highest Priority)**

**Why P0**:
- ✅ **User Value = 5**: Core habit-building mechanism, <2min fits user constraints
- ✅ **Strategic Fit = 5**: Enables all other features (feeds data to dashboard, trends, cohort)
- ✅ **Tech Effort = 2**: Simple form with 3 sliders + optional text

**User Research Support**:
- Survey Q: "How much time would you spend on daily check-in?"
- Expected: 60-70% choose "Under 1 minute" or "1-2 minutes"

**Implementation Scope**:
```
Screens:
1. Daily Check-In Main (3 rating sliders: Emotional/Relational/Academic)
2. Quest Selection (checkboxes: which goals worked on today)
3. Optional Quick Note (text field, <100 chars)

Data captured:
- 3 numerical ratings (1-5 scale)
- Quest IDs (which of 5 quests user worked on)
- Optional reflection text
- Timestamp

Integration:
→ Feeds Progress Dashboard
→ Updates Quest Board grid
→ Triggers Cohort Space updates
```

**Wireframe Priority**: **Week 1** (Oct 21-25)

---

### Feature #6: Cohort Space (Aggregated Peer Progress)

**Score: 12**

**Why P0**:
- ✅ **User Value = 5**: Core differentiator from solo apps (Fabulous failed without social)
- ✅ **Strategic Fit = 5**: Enables accountability without anxiety (privacy-first design)
- ✅ **Tech Effort = 3**: Moderate (aggregation logic + real-time updates)

**User Research Support**:
- Survey Q: "How important is peer accountability?"
- Expected: 50-60% choose "Very" or "Somewhat important"
- Game Mechanics Research: Strava's aggregated visibility = 43% persistence boost

**Implementation Scope**:
```
Screens:
1. Progress Board (group milestone bar + anonymous activity feed)
2. Encouragement Wall (emoji reactions + short messages)
3. Milestone Celebrations (group achievements)

Data displayed (privacy-preserving):
✅ "4/5 cohort members checked in today"
✅ "Someone reached 75% on Quest Board"
✅ Total emoji reactions count
❌ Never show: individual names, scores, or content

Integration:
→ Receives data from Daily Check-In
→ Receives Quest Board completion %
→ Sends encouragement to individuals (anonymized)
```

**Wireframe Priority**: **Week 2** (Oct 28-Nov 1)

---

### Feature #5: Progress Dashboard (Trend Graphs)

**Score: 11**

**Why P0**:
- ✅ **User Value = 5**: Users want to "see patterns" (survey expected: 70% prefer visual tracking)
- ✅ **Strategic Fit = 4**: Shows growth without gamification (journey narrative)
- ✅ **Tech Effort = 3**: Moderate (charting library integration)

**User Research Support**:
- Survey Q: "Which format do you prefer for tracking progress?"
- Expected: 60-70% choose "Visual graphs" or "Mix of visuals and text"

**Implementation Scope**:
```
Screens:
1. Dashboard Home (3 trend line charts: Emotional/Relational/Academic over time)
2. Quest Board Summary (weekly completion % bar chart)
3. Correlation Insights (optional: "Your emotional wellness ↑ when academic progress ↑")

Visualizations:
- Line charts (7-day, 30-day, 90-day views)
- Bar charts (Quest Board weekly comparison)
- Progress indicators (completion rates)

Data sources:
→ Daily Check-In ratings (3 dimensions)
→ Quest Board completion %
→ Weekly Planning goal achievement
```

**Wireframe Priority**: **Week 1-2** (Oct 21-Nov 1) - **Dong Zhang's Section 2 responsibility**

---

## 🟠 P1 - High Priority (MVP+)

### Feature #1: Three-Layer Goal Framework

**Score: 10**

**Why P1**:
- ✅ **User Value = 4**: Connects daily actions to long-term vision (key value prop)
- ✅ **Strategic Fit = 5**: Core to "structured guidance" philosophy
- ✅ **Tech Effort = 3**: Requires goal hierarchy logic + UI for 3 levels

**Implementation Scope**:
```
Screens:
1. Future Visioning (one-time setup, 3-year goals)
2. Quarterly Goal Setting (every 3 months)
3. Weekly Actions (every week, linked to quarterly goals)

Hierarchy:
Long-term Vision (3 years)
  ├── Quarterly Goal 1
  │   ├── Weekly Action 1
  │   └── Weekly Action 2
  └── Quarterly Goal 2
      └── Weekly Action 3

Integration:
→ Weekly Actions link to Quest Board
→ Progress Dashboard shows goal completion %
```

**Wireframe Priority**: **Week 3** (Nov 4-8)

---

### Feature #7: Quest Board (BINGO-style Grid)

**Score: 10**

**Why P1**:
- ✅ **User Value = 4**: Visual progress satisfaction (BINGO research: filling squares = dopamine)
- ✅ **Strategic Fit = 5**: Non-competitive gamification (no leaderboards)
- ✅ **Tech Effort = 2**: Simple grid UI + state management

**Implementation Scope**:
```
Screens:
1. Quest Board Main (5×5 or 5×7 grid)
2. Edit Quests (customize 5 categories)
3. Quest History (weekly archive)

Grid Logic:
- 5 quest categories (customizable)
- 7 days per week = 35 squares OR
- 5 days per week = 25 squares (with 2 "free" days)

Integration:
→ Auto-fills from Daily Check-In quest selection
→ Shares completion % to Cohort Space
→ Feeds completion rate to Progress Dashboard
```

**Wireframe Priority**: **Week 2** (Oct 28-Nov 1) - **Detailed in BINGO_UI_Application_Design.md**

---

### Feature #11: Emoji Reactions (Encouragement System)

**Score: 10**

**Why P1**:
- ✅ **User Value = 4**: Lightweight interaction (research: 5x participation vs. comments)
- ✅ **Strategic Fit = 5**: Low-friction support (Fogg Behavior Model: high ability → high action)
- ✅ **Tech Effort = 1**: Simple (just a button + counter)

**Implementation Scope**:
```
Screens:
1. Encouragement Wall (in Cohort Space)
2. Emoji Reaction Bar (on anonymous activity feed)

Emoji Set:
❤️ Love/Support
👏 Encouragement
🌟 Inspiration
💪 Motivation
🎉 Celebration

Interaction:
- One-tap to react
- See total count (not individual names)
- Optional: "You received 12 reactions this week!"

Integration:
→ Attached to Cohort Space activity feed
→ Notifications (optional): "Your cohort sent you 5 👏"
```

**Wireframe Priority**: **Week 2** (Oct 28-Nov 1)

---

## 🟡 P2 - Medium Priority (Post-MVP)

### Feature #3: Weekly Planning (5-10 min)

**Score: 9**

**Why P2 (not P1)**:
- ✅ **User Value = 4**: Important for goal alignment, but daily check-in is more critical
- ✅ **Strategic Fit = 4**: Supports structured reflection
- ⚠️ **Tech Effort = 2**: Low complexity, but lower urgency than core features

**Implementation Scope**:
```
Screens:
1. Weekly Review (past week's trends, top 3 insights)
2. Weekly Planning (set 3-5 specific actions for coming week)
3. Progress Comparison (this week vs. last week)

Timing: Suggested on Sunday evening or Monday morning

Integration:
→ Pulls data from past week's Daily Check-Ins
→ Sets weekly goals that link to Quest Board
→ Feeds into Goal Framework (weekly → quarterly connection)
```

**Wireframe Priority**: **Week 4** (Nov 11-15)

---

### Feature #8: Wheel of Life Visualization

**Score: 8**

**Why P2**:
- ✅ **User Value = 4**: Familiar self-assessment tool (from real QuestLabs)
- ⚠️ **Strategic Fit = 3**: Less tied to daily habit than Quest Board
- ⚠️ **Tech Effort = 3**: Moderate (radar chart rendering)

**Implementation Scope**:
```
Screens:
1. Wheel of Life Assessment (8 dimensions, rate 1-5)
2. Wheel Visualization (radar chart)
3. Historical Comparison (overlay this month vs. last month)

8 Dimensions (from UI_referrence/WheelOfLife.jpg):
- Digital Diet
- Organization
- Friends
- Family
- School/Work
- Fun
- Growth
- Health

Integration:
→ Initial setup (onboarding)
→ Monthly re-assessment
→ Feeds into Progress Dashboard
```

**Wireframe Priority**: **Week 3-4** (Nov 4-15) - **Dong Zhang's Section 2 responsibility**

---

### Feature #12: Milestone Celebrations

**Score: 8**

**Why P2**:
- ✅ **Strategic Fit = 4**: Positive reinforcement (no punishment)
- ⚠️ **User Value = 3**: Nice-to-have, but core features more critical
- ✅ **Tech Effort = 2**: Animation + notification logic

**Implementation Scope**:
```
Milestone Triggers:
Individual:
- First Daily Check-In ✅
- 7-day streak 🔥
- Full BINGO week (25/25 squares) 🎉
- Completed Quarterly Goal 🌟

Cohort:
- All 5 members checked in same day 🎊
- Group reached 100 total reflections 💯
- Cohort maintained for 4 weeks ❤️

Celebration Format:
- Animation (confetti, fireworks)
- Sound (optional, short chime)
- Message (encouraging, non-competitive)
- Badge (visual only, no points)

Integration:
→ Triggers from Daily Check-In, Quest Board, Cohort Space
→ Appears as modal overlay
→ Shareable to Cohort (optional)
```

**Wireframe Priority**: **Week 5** (Nov 18-22)

---

## 🟢 P3 - Nice to Have (V2.0)

### Feature #4: Structured Reflection Journal

**Score: 7**

**Why P3**:
- ⚠️ **User Value = 3**: Some users prefer quick check-ins over writing
- ✅ **Strategic Fit = 4**: Fill-in-the-blank prompts reduce "blank page" anxiety
- ⚠️ **Tech Effort = 3**: Prompt system + text storage

**Implementation Scope**:
```
Screens:
1. Reflection Prompt Selection (choose from 20+ prompts)
2. Fill-in-the-Blank Journal (structured writing)
3. Reflection Timeline (chronological view of past entries)

Example Prompts:
- "Today I felt ___ because ___"
- "I'm grateful for ___"
- "One thing I learned about myself: ___"
- "Tomorrow I want to focus on ___"

Tagging:
- Emotion tags (joy, anxiety, calm, etc.)
- Theme tags (relationships, work, health)

Integration:
→ Optional add-on to Daily Check-In
→ Feeds into SEL Timeline (if implemented)
→ Shareable to Cohort (with permission)
```

**Wireframe Priority**: **Week 6+** (Nov 25+) or **V2.0**

---

### Feature #9: Affect-Agency Grid (Polak's Model)

**Score: 5**

**Why P3**:
- ⚠️ **User Value = 3**: Academic model, less intuitive for general users
- ⚠️ **Strategic Fit = 3**: Interesting but not core to anti-gamification
- ❌ **Tech Effort = 4**: Complex (quadrant calculation + plotting)

**Implementation Scope**:
```
Screens:
1. Affect-Agency Assessment (2 dimensions: Positive/Negative Affect × High/Low Agency)
2. Quadrant Visualization (4 states: Hopeful, Empowered, Anxious, Apathetic)
3. Historical Trajectory (movement between quadrants over time)

Quadrants:
        High Agency
            |
  Hopeful   |   Empowered
------------|-------------
  Anxious   |   Apathetic
            |
   Low Affect ← → High Affect

Integration:
→ Derived from Daily Check-In emotional + goal progress ratings
→ Shown in Progress Dashboard (if user opts in)
```

**Wireframe Priority**: **V2.0** (after user feedback on simpler visualizations)

---

## ⚪ P4 - Future Phase (V3.0+)

### Feature #10: SEL Timeline (Social-Emotional Learning Trends)

**Score: 4**

**Why P4**:
- ⚠️ **User Value = 3**: Overlaps with Progress Dashboard line charts
- ❌ **Strategic Fit = 2**: More "data visualization" than "growth support"
- ❌ **Tech Effort = 4**: High (time-series analysis + multi-dimensional charting)

**Implementation Scope**:
```
Screens:
1. SEL Timeline (line chart with 3 overlaid trends)
2. Event Markers (annotate significant moments)
3. Correlation Analysis ("Your wellness ↑ when relationships ↑")

Data Sources:
- Daily Check-In ratings (Emotional/Relational/Academic)
- Reflection Journal tags (emotion keywords)
- Weekly Planning reflections

Complexity:
- Requires significant historical data (30+ days)
- Advanced analytics (correlation detection)
- May confuse users with too much data

Recommendation: Defer to V3.0, focus on simpler Progress Dashboard first
```

**Wireframe Priority**: **V3.0** (after 3-6 months of user data)

---

## 📊 Value vs. Effort Matrix (Visual)

```
High Value │
     5     │  #2           #6
           │  Daily        Cohort
           │  Check-In     Space
     4     │  #5           #1 #7 #11
           │  Dashboard    Goal/BINGO/Emoji
           │
     3     │  #3 #8 #12    #4
           │  Weekly/      Journal
           │  Wheel/Mile
     2     │               #9
           │               Affect-
           │               Agency
     1     │               #10
           │               SEL
           │               Timeline
  Low      └──────────────────────────────
           Low  1    2    3    4    5  High
                    Technical Effort

Legend:
🔴 P0 (Must Have): #2, #5, #6
🟠 P1 (High): #1, #7, #11
🟡 P2 (Medium): #3, #8, #12
🟢 P3 (Nice to Have): #4, #9
⚪ P4 (Future): #10
```

---

## 🎯 Phased Implementation Roadmap

### **Phase 1: MVP (Weeks 1-8)** - P0 + P1
**Goal**: Functional app with core habit-building + social accountability

**Must Have** (P0):
- [ ] Daily Check-In
- [ ] Progress Dashboard
- [ ] Cohort Space

**High Priority** (P1):
- [ ] Goal Framework
- [ ] Quest Board (BINGO)
- [ ] Emoji Reactions

**Deliverables**:
- Users can check in daily
- Users can see their trends
- Users can encourage cohort anonymously
- Users can track goals visually

---

### **Phase 2: Enhancement (Weeks 9-12)** - P2
**Goal**: Deeper engagement + richer visualizations

**Medium Priority** (P2):
- [ ] Weekly Planning
- [ ] Wheel of Life
- [ ] Milestone Celebrations

**Deliverables**:
- Users can plan weekly actions
- Users can assess life balance
- Users celebrate achievements

---

### **Phase 3: Advanced Features (V2.0)** - P3
**Goal**: Power-user features + advanced insights

**Nice to Have** (P3):
- [ ] Reflection Journal
- [ ] Affect-Agency Grid

**Deliverables**:
- Users can write structured reflections
- Users can track emotional positioning

---

### **Phase 4: Analytics (V3.0+)** - P4
**Goal**: Long-term trend analysis

**Future Phase** (P4):
- [ ] SEL Timeline with correlation insights

---

## 🔍 Validation with User Survey

Once survey data is collected (Oct 11), update scores based on:

**Survey Question Mapping**:

| Feature | Corresponding Survey Question |
|---------|-------------------------------|
| Daily Check-In | "How much time would you realistically spend?" |
| Cohort Space | "How important is peer accountability?" + "What support from group?" |
| Progress Dashboard | "Which format do you prefer?" (visual vs. text) |
| Goal Framework | "Rate your interest: Long-term goal tracking (3 months+)" |
| Quest Board | Survey doesn't directly test this—use BINGO research |
| Emoji Reactions | "Rate your interest: Give/receive encouragement reactions" |
| Weekly Planning | "How often do you intentionally reflect?" |
| Wheel of Life | Not directly tested—use real QuestLabs validation |
| Reflection Journal | "Rate your interest: Structured reflection prompts" |

**Update Process** (Oct 11):
1. Calculate % of users rating each feature 4-5/5 (high interest)
2. If >70% high interest → boost User Value by +1
3. If <40% high interest → reduce User Value by -1
4. Recalculate Priority Scores
5. Adjust P0/P1/P2 assignments if needed

---

## 💡 Strategic Insights

### Why These Priorities Make Sense:

**P0 (Must Have)** focuses on **habit loop**:
```
Daily Check-In → Generates Data
       ↓
Progress Dashboard → Shows Patterns
       ↓
Cohort Space → Provides Motivation
       ↓
User Returns Tomorrow → Habit Formed
```

**P1 (High Priority)** adds **structure + delight**:
```
Goal Framework → Gives direction ("why am I doing this?")
Quest Board → Makes progress tangible (visual satisfaction)
Emoji Reactions → Makes support effortless (5x participation)
```

**P2 (Medium Priority)** adds **depth**:
```
Weekly Planning → Enhances intentionality
Wheel of Life → Adds holistic perspective
Celebrations → Reinforces positive behavior
```

**P3-P4 (Nice to Have / Future)** are **power features**:
- Serve smaller user segments
- Require more development time
- Can be added iteratively based on feedback

---

## 📋 Decision-Making Criteria

When in doubt, ask:

1. **Does this enable the core habit loop?** → P0
2. **Does this differentiate us from competitors?** → P1
3. **Do users explicitly request this?** → Check survey
4. **Can we launch without this?** → If yes, lower priority
5. **Does this align with anti-gamification?** → If no, reject or redesign

---

## ✅ Next Steps

**For Oct 14 Task**:
- [ ] Present this matrix to team
- [ ] Discuss any disagreements on scores
- [ ] Finalize P0 + P1 features for wireframing
- [ ] Assign features to team members:
  - Dong Zhang: Dashboard (#5), Wheel of Life (#8), Quest Board (#7)
  - Zhi Kang: Daily Check-In (#2), Cohort Space (#6), Goal Framework (#1)

**After Survey Analysis (Oct 11)**:
- [ ] Update User Value scores based on survey %
- [ ] Recalculate Priority Scores
- [ ] Adjust roadmap if needed

**For Wireframing (Oct 21+)**:
- [ ] Start with P0 features (weeks 1-2)
- [ ] Add P1 features (weeks 2-3)
- [ ] Design P2 features (weeks 4-5)

---

**File Created**: 2025-10-16
**Framework**: Value×2 + Strategic Fit - Effort
**Total Features Evaluated**: 12
**P0 (Must Have)**: 3 features
**P1 (High Priority)**: 3 features
**P2 (Medium Priority)**: 3 features
**P3 (Nice to Have)**: 2 features
**P4 (Future)**: 1 feature


