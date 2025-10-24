# Feature Prioritization Matrix - QuestLabs Companion

**Purpose**: Rank 12 core features based on user needs, technical feasibility, and project constraints
**Framework**: Value vs. Effort Matrix + PACT Alignment + Research Data
**Created**: 2025-10-16
**Last Updated**: 2025-10-23 (Based on 14 survey responses)
**For**: Oct 14 Task - Feature Prioritization
**Team**: Dong Zhang + Zhi Kang

---

## 🔄 **Update Log - Oct 23, 2025**

**Survey Data Collected**: 14 valid responses (Oct 16-23)

**Major Changes Based on User Research**:
1. ⬆️ **Long-Term Goal Tracking**: P1 → **P0** (79% high interest, highest score)
2. ⬆️ **Encouragement Reactions**: P1 → **P1** (64% high interest, validated)
3. ⚠️ **NEW FEATURE - Push Notifications/Reminders**: Added as **P1** (64% forget to reflect)
4. ✅ **Daily Check-In**: P0 validated (79% want <2 min)
5. ✅ **Progress Dashboard**: P0 validated (71% prefer visual tracking)
6. ✅ **Cohort Space**: P0 validated (64% want peer accountability)

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

## 🎯 The 13 Core Features (Updated Oct 23)

Based on Proposal + Survey Findings:

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
13. **Push Notifications/Reminders** ⚠️ NEW (Added based on survey: 64% forget to reflect)

---

## 📈 Feature Scoring Matrix (Updated with Survey Data)

**Formula**: Priority Score = (User Value × 2 + Strategic Fit) - Tech Effort

**Survey-Based User Value Updates**:
- User Value 5 = >70% high interest (4-5 rating) or critical need
- User Value 4 = 50-70% high interest
- User Value 3 = 30-50% high interest
- User Value 2 = <30% high interest

| # | Feature | User Value (Updated) | Tech Effort | Strategic Fit | Priority Score | Priority Tier |
|---|---------|---------------------|-------------|---------------|----------------|---------------|
| 2 | **Daily Check-In** | 5 (79% want <2min) | 2 | 5 | **13** | 🔴 P0 (Must Have) |
| 1 | **Goal Framework (Long-term)** | 5 (79% interest ⬆️) | 3 | 5 | **12** | 🔴 P0 (Must Have) ⬆️ |
| 6 | **Cohort Space** | 5 (64% need peers) | 3 | 5 | **12** | 🔴 P0 (Must Have) |
| 5 | **Progress Dashboard** | 5 (71% visual) | 3 | 4 | **11** | 🔴 P0 (Must Have) |
| 13 | **Push Notifications** | 4 (64% forget ⚠️NEW) | 2 | 4 | **10** | 🟠 P1 (High Priority) ⚠️ |
| 11 | **Emoji Reactions** | 4 (64% interest) | 1 | 5 | **10** | 🟠 P1 (High Priority) |
| 7 | **Quest Board (BINGO)** | 4 (estimated) | 2 | 5 | **10** | 🟠 P1 (High Priority) |
| 12 | **Milestone Celebrations** | 4 (50% want) | 2 | 4 | **9** | 🟡 P2 (Medium Priority) |
| 3 | **Weekly Planning** | 4 | 2 | 4 | **9** | 🟡 P2 (Medium Priority) |
| 8 | **Wheel of Life** | 4 | 3 | 3 | **8** | 🟡 P2 (Medium Priority) |
| 4 | **Reflection Journal** | 3 (50% prompts) | 3 | 4 | **7** | 🟢 P3 (Nice to Have) |
| 9 | **Affect-Agency Grid** | 3 | 4 | 3 | **5** | 🟢 P3 (Nice to Have) |
| 10 | **SEL Timeline** | 3 | 4 | 2 | **4** | ⚪ P4 (Future Phase) |

**Key Changes**:
- ⬆️ **Long-Term Goal Framework** upgraded from P1 to **P0** (79% high interest, tied for #1)
- ⚠️ **Push Notifications/Reminders** added as **P1** (new feature based on 64% forget barrier)
- ⬆️ **Milestone Celebrations** upgraded from P2 to **P2** (50% want, higher than expected)
- ✅ All P0 features validated by survey data (>64% support)

---

## 🔴 P0 - Must Have (MVP Core)

**Total P0 Features: 4** (upgraded from 3 based on survey)

---

### Feature #2: Daily Check-In (<2 min)

**Score: 13 (Highest Priority)**

**Why P0**:
- ✅ **User Value = 5**: Core habit-building mechanism, <2min fits user constraints
- ✅ **Strategic Fit = 5**: Enables all other features (feeds data to dashboard, trends, cohort)
- ✅ **Tech Effort = 2**: Simple form with 3 sliders + optional text

**User Research Support** ✅ **VALIDATED**:
- Survey Q: "How much time would you spend on daily check-in?"
- **RESULT: 79% (11/14) want <2 minutes** (50% <1min, 29% 1-2min)
- **Strongest validation in entire survey**

**🎯 Design Requirement: Attendance Restart Weekly** (Meeting discussion point, Oct 24)
- **Principle**: Weekly Progress Model (no cumulative streaks)
- **Mechanism**: Track weekly check-in % (e.g., 5/7 = 71%), reset every Monday
- **Rationale**: Reduces re-entry barrier during busy weeks (exams, etc.)
- **Anti-gamification**: No "broken streak" guilt, every Monday is fresh start
- **Messaging**: Supportive (not guilt-inducing) - "3 check-ins this week ❤️"
- **Threshold**: ≥3 check-ins/week = "engaged" (not requiring 7/7 perfection)
- **See**: `Weekly_Restart_Mechanism_Discussion.md` for full analysis

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

### Feature #1: Three-Layer Goal Framework (Long-term Goals) ⬆️ **UPGRADED TO P0**

**Score: 12** (tied with Cohort Space)

**Why P0** (Upgraded from P1):
- ✅ **User Value = 5** ⬆️: **79% (11/14) rated 4-5 interest** - HIGHEST of all features surveyed
- ✅ **Strategic Fit = 5**: Core to "present awareness → future possibilities" motto
- ✅ **Tech Effort = 3**: Requires goal hierarchy logic + UI for 3 levels

**User Research Support** ✅ **STRONGEST FEATURE VALIDATION**:
- Survey Q: "Rate your interest: Long-term goal tracking (3 months+)"
- **RESULT: 79% high interest (4-5 rating), Average score 4.1**
- **Tied with Daily Check-In for highest interest**
- Motivation data: 64% motivated by "Achieving long-term goals"

**Why This Matters**:
- Users want to see how daily actions connect to future aspirations
- Validates three-layer framework (vision → quarterly → weekly → daily)
- Differentiates from simple habit trackers

**🎯 Design Requirement: Long-Term Process Management** (Meeting discussion point, Oct 24)
- **Core principle**: Connect daily actions to long-term vision
- **Three-layer framework**: Vision (3 years) → Quarterly goals → Weekly actions → Daily check-in
- **User need**: 79% high interest + 64% motivated by "Achieving long-term goals"
- **Design focus**: Make goal hierarchy visible and trackable
- **Dashboard integration**: Show "Which long-term goal did today's work support?"

**Implementation Scope**:
```
Screens:
1. Future Visioning (one-time setup, 3-year goals)
2. Quarterly Goal Setting (every 3 months)
3. Weekly Actions (every week, linked to quarterly goals)
4. Goal Progress Dashboard (completion rates over time)

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
→ Daily Check-In asks "Which goals did you work on today?"
```

**Wireframe Priority**: **Week 1-2** (Oct 21-Nov 1) - **Upgraded priority**

---

### Feature #6: Cohort Space (Aggregated Peer Progress)

**Score: 12**

**Why P0**:
- ✅ **User Value = 5**: Core differentiator from solo apps (Fabulous failed without social)
- ✅ **Strategic Fit = 5**: Enables accountability without anxiety (privacy-first design)
- ✅ **Tech Effort = 3**: Moderate (aggregation logic + real-time updates)

**User Research Support** ✅ **VALIDATED**:
- Survey Q: "How important is peer accountability?"
- **RESULT: 64% (9/14) choose "Very" or "Somewhat important"**
- Privacy data: 71% need "Control what I share", 43% reject "Public rankings"
- Support types: 50% want "Celebrating milestones", 43% want "Encouragement reactions"
- Game Mechanics Research: Strava's aggregated visibility = 43% persistence boost

**🎯 Design Requirement: User Privacy Protection** (Meeting discussion point, Oct 24)
- **Principle**: Aggregated data only, no individual exposure
- **Survey validation**: 71% need "Control what I share", 43% reject "Public rankings"
- **Implementation**: Show group trends ("4/5 checked in today") NOT individual names/scores
- **Privacy controls**: Granular settings for what to share with cohort
- **Anti-gamification**: No leaderboards, no comparative rankings
- **Cohort visibility**: Anonymous progress indicators only

**🎯 Design Requirement: Small Cohort (5-10 people)** (Meeting discussion point, Oct 24)
- **Recommended size**: 5-10 members per cohort (based on competitive research)
- **Rationale**: Small groups increase accountability + trust
- **Survey support**: 50% prefer "Knowing members personally" (easier in small groups)
- **Privacy alignment**: Smaller groups = more comfortable sharing (71% need control)
- **Competitive insight**: QuestLabs real program uses small cohorts effectively
- **Implementation**: Cap cohort size at 10, encourage 5-8 optimal

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

**User Research Support** ✅ **VALIDATED**:
- Survey Q: "Which format do you prefer for tracking progress?"
- **RESULT: 71% (10/14) prefer visual formats** (57% graphs/charts, 14% mix)
- **0% want text-only journals** - visual tracking is non-negotiable
- Motivation: 79% (11/14) motivated by "Seeing my own progress over time" (#1 motivator)

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

**Total P1 Features: 4** (added Push Notifications based on survey)

---

### Feature #13: Push Notifications/Reminders ⚠️ **NEW FEATURE**

**Score: 10**

**Why P1** (New feature added based on survey findings):
- ✅ **User Value = 4**: **64% (9/14) say "Forget to do it" is their #1 barrier**
- ✅ **Strategic Fit = 4**: Critical for habit formation (without reminders, users won't build daily habit)
- ✅ **Tech Effort = 2**: Low complexity (push notification system)

**User Research Support** ⚠️ **CRITICAL GAP IDENTIFIED**:
- Survey Q: "What's the BIGGEST challenge preventing regular reflection?"
- **RESULT: 64% (9/14) select "I forget to do it" - TOP BARRIER**
- Second barrier: "Don't have time" (36%)
- **Current proposal has NO reminder/notification feature → this is a gap**

**Why This Matters**:
- Habit formation research: Reminders increase adherence by 40-60%
- Without reminders, even motivated users won't maintain daily check-in
- Low technical effort, high user value

**Implementation Scope**:
```
Features:
1. Daily reminder notification (user-customizable time)
2. Smart reminders (skip if already checked in today)
3. Gentle nudges (not aggressive/guilt-inducing)
4. Reminder settings (time, frequency, message customization)

Notification Examples:
- "Time for your daily reflection 🌟" (7:00 PM)
- "You've checked in 5 days this week! Keep it up 💪" (Friday)
- "Your cohort is waiting for you ❤️" (if user hasn't checked in)

User Controls:
- Enable/disable reminders
- Set preferred time(s)
- Choose notification tone
- Pause for vacation/busy periods

Integration:
→ Triggered at user-set time daily
→ Disabled if Daily Check-In completed
→ Can link directly to Check-In screen
```

**Wireframe Priority**: **Week 3** (Nov 4-8) - **Settings screen + notification UI**

**Design Principles**:
- ✅ Supportive, not guilt-inducing
- ✅ User has full control (easy to disable)
- ✅ Smart (doesn't nag if already done)
- ❌ No streak-shaming ("You broke your 10-day streak!")

---

### Feature #1: Three-Layer Goal Framework ⬇️ **MOVED TO P0**

(See P0 section above - upgraded based on 79% survey interest)

---

### Feature #11: Emoji Reactions (Encouragement System)

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
- ✅ **User Value = 4**: **64% (9/14) rated 4-5 interest** - validated by survey
- ✅ **Strategic Fit = 5**: Low-friction support (Fogg Behavior Model: high ability → high action)
- ✅ **Tech Effort = 1**: Simple (just a button + counter)

**User Research Support** ✅ **VALIDATED**:
- Survey Q: "Rate your interest: Give/receive encouragement reactions from peers"
- **RESULT: 64% (9/14) high interest (4-5 rating), Average score 3.9**
- Support types: 43% (6/14) want "Giving/receiving encouragement reactions"
- Research: 5x participation rate vs. text comments

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

**Score: 9** (upgraded based on survey)

**Why P2**:
- ✅ **User Value = 4** ⬆️: **50% (7/14) want "Celebrating milestones together"**
- ✅ **Strategic Fit = 4**: Positive reinforcement (no punishment)
- ✅ **Tech Effort = 2**: Animation + notification logic

**User Research Support** ✅ **VALIDATED**:
- Survey Q: "What support from group would be most helpful?"
- **RESULT: 50% (7/14) select "Celebrating milestones together"** (tied for #1)
- Higher than expected - users want positive recognition

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
- ⚠️ **User Value = 3**: **50% (7/14) rated 4-5 interest** - moderate demand
- ✅ **Strategic Fit = 4**: Fill-in-the-blank prompts reduce "blank page" anxiety
- ⚠️ **Tech Effort = 3**: Prompt system + text storage

**User Research Support** ⚠️ **MODERATE VALIDATION**:
- Survey Q: "Rate your interest: Structured reflection prompts (fill-in-the-blank)"
- **RESULT: 50% (7/14) high interest (4-5 rating), Average score 3.2**
- Reflection tool preference: 79% want "structure" (clear or some structure)
- However, 29% say "Don't know what to reflect on" (prompts help this)
- **Conclusion**: Useful for segment of users, but not universal need → P3 appropriate

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

## 🔍 Validation with User Survey ✅ **COMPLETED OCT 23**

**Survey Data**: 14 valid responses collected Oct 16-23

**Validation Results**:

| Feature | Survey Question | Result | User Value Update | Priority Change |
|---------|----------------|--------|-------------------|-----------------|
| **Daily Check-In** | Time willingness | **79% want <2min** ✅ | 5 (kept) | P0 ✅ VALIDATED |
| **Long-term Goal Tracking** | Interest rating | **79% high interest** ✅ | 4→**5** ⬆️ | P1→**P0** ⬆️ |
| **Progress Dashboard** | Visual preference | **71% prefer visual** ✅ | 5 (kept) | P0 ✅ VALIDATED |
| **Cohort Space** | Peer accountability | **64% important** ✅ | 5 (kept) | P0 ✅ VALIDATED |
| **Emoji Reactions** | Interest rating | **64% high interest** ✅ | 4 (kept) | P1 ✅ VALIDATED |
| **Reminders/Notifications** | Biggest challenge | **64% forget** ⚠️ | 4 (NEW) | **P1** ⚠️ ADDED |
| **Milestone Celebrations** | Group support | **50% want** ✅ | 3→**4** ⬆️ | P2 (upgraded score) |
| **Reflection Journal** | Interest rating | **50% high interest** | 3 (kept) | P3 ✅ VALIDATED |
| **Quest Board (BINGO)** | Not directly tested | N/A | 4 (estimated) | P1 (keep based on research) |
| **Weekly Planning** | Not directly tested | N/A | 4 (kept) | P2 (keep) |
| **Wheel of Life** | Not directly tested | N/A | 4 (kept) | P2 (keep) |
| **Affect-Agency Grid** | Not tested | N/A | 3 (kept) | P3 (keep) |
| **SEL Timeline** | Not tested | N/A | 3 (kept) | P4 (keep) |

**Survey Impact Summary**:
1. ⬆️ **Long-Term Goal Framework** → P0 (79% = highest interest)
2. ⚠️ **Push Notifications** → P1 (new feature, 64% need)
3. ⬆️ **Milestone Celebrations** → User Value +1 (50% want)
4. ✅ **All P0 features validated** with >64% support
5. ✅ **All P1 features validated** with >50% interest or critical need

**Update Process Applied** (Oct 23):
1. ✅ Calculated % of users rating each feature 4-5/5 (high interest)
2. ✅ Applied threshold: >70% high interest → User Value 5 (P0 candidate)
3. ✅ Applied threshold: 50-70% → User Value 4 (P1 candidate)
4. ✅ Recalculated Priority Scores using formula
5. ✅ Adjusted P0/P1/P2 assignments based on new scores
6. ✅ Added new feature (Reminders) based on critical gap

---

## 💡 Strategic Insights

### Core Design Requirements (From Oct 24 Meeting Discussion)

Four key principles guide our feature design:

**1. Long-Term Process Management** ⭐
- Three-layer goal framework connects daily actions to 3-year vision
- Survey validation: 79% high interest in long-term goal tracking
- Feature impact: Long-Term Goal Framework upgraded to P0

**2. User Privacy Protection** 🔒
- Aggregated cohort data only, no individual exposure
- Survey validation: 71% need "Control what I share", 43% reject rankings
- Feature impact: Cohort Space shows group trends, not individual scores

**3. Small Cohort (5-10 people)** 👥
- Recommended cohort size: 5-10 members (competitive research)
- Survey support: 50% prefer "Knowing members personally"
- Feature impact: Cap cohort size, encourage face-to-face relationships

**4. Attendance Restart Weekly** 🔄
- Weekly progress model (no cumulative streaks)
- Reduces re-entry barrier during busy weeks (exams, etc.)
- Feature impact: Daily Check-In tracks weekly %, resets every Monday
- See: `Weekly_Restart_Mechanism_Discussion.md` for full analysis

---

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

---

## 📊 Updated Feature Summary (Oct 23, 2025)

**Based on 14 survey responses (Oct 16-23)**

### Priority Distribution:

**🔴 P0 - Must Have**: **4 features** (upgraded from 3)
1. Daily Check-In (<2 min) - Score 13
2. Long-Term Goal Framework ⬆️ - Score 12
3. Cohort Space (Aggregated) - Score 12
4. Progress Dashboard (Visual) - Score 11

**🟠 P1 - High Priority**: **4 features** (added Reminders)
1. Push Notifications/Reminders ⚠️ NEW - Score 10
2. Emoji Reactions - Score 10
3. Quest Board (BINGO) - Score 10
4. ~~Goal Framework~~ ⬇️ (moved to P0)

**🟡 P2 - Medium Priority**: **3 features**
1. Milestone Celebrations ⬆️ - Score 9 (upgraded)
2. Weekly Planning - Score 9
3. Wheel of Life - Score 8

**🟢 P3 - Nice to Have**: **2 features**
1. Reflection Journal - Score 7
2. Affect-Agency Grid - Score 5

**⚪ P4 - Future Phase**: **1 feature**
1. SEL Timeline - Score 4

**Total Features**: **13** (added 1 new feature based on survey)

---

## ✅ Next Steps (Updated Oct 23)

**For Oct 23 Morning Meeting**:
- [x] Present survey findings (14 responses)
- [x] Discuss feature priority updates
- [x] Get team approval for Long-Term Goals → P0
- [ ] Discuss adding Reminders to roadmap

**After Meeting (Oct 25)**:
- [ ] Start wireframing P0 features first:
  - Daily Check-In
  - Dashboard (Dong's responsibility)
  - Long-Term Goal Framework ⬆️ (new P0)
  - Cohort Space

**For Wireframing (Oct 21-Nov 15)**:
- [ ] Week 1-2: P0 features (4 features)
- [ ] Week 3: P1 features (4 features, including Reminders settings)
- [ ] Week 4-5: P2 features (3 features)

---

**File Created**: 2025-10-16
**Last Updated**: 2025-10-23
**Framework**: (User Value × 2 + Strategic Fit) - Tech Effort
**Data Source**: 14 survey responses + competitive research
**Total Features Evaluated**: 13 (added Reminders)
**P0 (Must Have)**: 4 features ⬆️
**P1 (High Priority)**: 4 features (includes new Reminders)
**P2 (Medium Priority)**: 3 features
**P3 (Nice to Have)**: 2 features
**P4 (Future)**: 1 feature

**Survey Validation**: ✅ All P0 features validated with >64% user support
**Critical Gap Identified**: ⚠️ Reminders/Notifications added as P1 (64% forget to reflect)


