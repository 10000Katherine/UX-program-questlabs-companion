# Weekly Restart Mechanism - Design Options Discussion

**Date**: Oct 23, 2025
**For**: Oct 24 Team Meeting
**Context**: Reducing re-entry barriers for students during busy weeks (exams, etc.)
**Goal**: Allow students to resume engagement without "sunk cost" penalty

---

## 🎯 Design Problem

**User Pain Point**:
Students may skip check-ins during busy weeks (midterms, finals). Traditional streak systems create guilt and high re-entry barriers ("I broke my 21-day streak, why bother?").

**Design Goal**:
Enable students to pause during busy periods and restart easily, without feeling they've "lost progress."

---

## 📊 Three Design Options

### **Option A: Weekly Streak Reset**

**Mechanism**:
Streak counter resets every Monday (not cumulative across weeks)

**User Experience**:
```
Week 1: 7/7 days → "Perfect week! 7-day streak 🌟"
Week 2: 3/7 days (midterms) → "3-day streak this week"
Week 3: Monday arrives → Counter resets to 0
        6/7 days → "6-day streak this week 🌟"
```

**Pros**:
- ✅ Fresh start every Monday
- ✅ No long-term streak pressure
- ✅ Still uses familiar "streak" language

**Cons**:
- ⚠️ Still has streak concept (some gamification)
- ⚠️ May feel like "losing progress" on Sunday night
- ⚠️ Doesn't fully eliminate streak anxiety

**Priority**: P1 (affects Daily Check-In design)

---

### **Option B: Flexible Pause Mode**

**Mechanism**:
User can manually pause streak; resumes from where they left off

**User Experience**:
```
Week 1: 7/7 days → "21-day total streak!"
Week 2: User clicks "Pause for midterms"
        → Streak frozen at 21 days ❄️
        → No guilt messages
Week 3: User clicks "Resume" or auto-resume Monday
        → Continues from 21, adds new days
```

**Pros**:
- ✅ User has control
- ✅ Preserves long-term streak (motivating for some)
- ✅ Predictable for planned busy periods

**Cons**:
- ⚠️ Requires user to remember to pause (extra action)
- ⚠️ Still uses cumulative streak (gamification)
- ⚠️ May feel like "cheating" if paused too often
- ❌ Contradicts anti-gamification philosophy

**Priority**: P2 (nice-to-have enhancement)

---

### **Option C: Weekly Progress Model (No Streaks)** ⭐ **RECOMMENDED**

**Mechanism**:
Track weekly check-in rate instead of consecutive days. No cumulative streak.

**User Experience**:
```
Week 1: 7/7 check-ins = 100% → "Amazing week! 🌟"
Week 2: 3/7 check-ins = 43% (midterms)
        → "You checked in 3 times. Take care ❤️"
        → No negative messaging
Week 3: Fresh week starts Monday
        6/7 check-ins = 86% → "Great week! 🌟"
        → No reference to Week 2's low rate
```

**UI Display**:
```
Dashboard shows:
- This week: 5/7 days (71%)
- Last 4 weeks: [100%, 43%, 86%, 71%] (trend chart)
- Total reflections: 47 (lifetime count, not streak)
```

**Pros**:
- ✅ **Zero re-entry barrier** (every Monday is fresh start)
- ✅ **No streak anxiety** (aligns with anti-gamification)
- ✅ **Flexible by design** (3/7 days is still "engaged")
- ✅ **Still shows progress** (weekly % visible)
- ✅ **Supportive messaging** (no guilt)
- ✅ **Cohort-friendly** (can show group's avg weekly %)

**Cons**:
- ⚠️ Less addictive than streaks (but that's intentional!)
- ⚠️ Some users may want traditional streaks

**Priority**: P0 (core design principle for Daily Check-In)

---

## 📋 Comparison Matrix

| Criterion | Option A: Weekly Streak | Option B: Pause Mode | Option C: Weekly Progress ⭐ |
|-----------|------------------------|---------------------|------------------------------|
| **Re-entry barrier** | Low (weekly reset) | Medium (manual action) | **Lowest (automatic)** |
| **Anti-gamification** | Partial (still streaks) | Low (keeps streaks) | **High (no streaks)** |
| **Flexibility** | Moderate | High (manual control) | **Highest (built-in)** |
| **User effort** | None | Pause/resume actions | **None** |
| **Guilt reduction** | Moderate | Low (if forget to pause) | **High** |
| **Cohort alignment** | Moderate | Low | **High (group avg %)** |
| **Survey alignment** | N/A | N/A | **✅ (79% want <2min)** |

---

## 💡 Recommendation: Option C (Weekly Progress Model)

### **Why Option C is Best**:

1. **Aligns with Anti-Gamification Philosophy**
   - No competitive streaks
   - No punishment for "breaking" anything
   - Focus on growth, not numbers

2. **Matches User Needs (Survey Data)**
   - 64% forget to reflect (Option C doesn't penalize forgetting)
   - 79% want quick check-in (weekly % is low-pressure)
   - 43% reject public rankings (weekly % isn't competitive)

3. **Reduces Sunk Cost Fallacy**
   - Missing Week 2 doesn't "break" anything
   - Week 3 is automatically a fresh start
   - No emotional loss from pausing

4. **Supports Real Student Life**
   - Midterms, finals, family emergencies happen
   - 3-5 check-ins/week is sustainable long-term
   - Perfection (7/7) is celebrated, not required

5. **Cohort-Friendly**
   - Can show: "Your cohort averaged 68% this week"
   - Encourages group without pressure
   - Anonymous, aggregated (privacy-first)

---

## 🎯 Proposed Implementation (Option C)

### **Dashboard Display**:
```
📊 This Week (Mon-Sun)
[✅][✅][✅][  ][✅][✅][  ] = 5/7 days (71%)

Recent Weeks:
Week of Oct 14: ████████░░ 86% (6/7)
Week of Oct 7:  ██████████ 100% (7/7) 🌟
Week of Sep 30: ████░░░░░░ 43% (3/7)
```

### **Messaging Examples**:
```
Supportive (not guilt-inducing):
- "5 check-ins this week! You're building a habit 🌱"
- "3 check-ins during a busy week - that's self-care ❤️"
- "Perfect week! 7/7 days 🌟" (celebration, not expectation)

Fresh Start:
- "New week, new possibilities! 🌅" (Monday)
- "Welcome back! No pressure, just progress 💪"
```

### **Milestones** (P2 feature):
```
Celebrate:
- First perfect week (7/7)
- 4 weeks in a row ≥5 check-ins
- 10 total weeks ≥70%

Don't celebrate:
- Total streak days (not tracked)
- "Coming back" after low week (no need, it's normal!)
```

---

## ✅ Design Principles Summary

**Option C embodies**:
- ✅ **Flexibility** (weekly reset)
- ✅ **Low pressure** (no streaks)
- ✅ **Supportive** (positive messaging only)
- ✅ **Realistic** (allows for busy weeks)
- ✅ **Privacy-first** (cohort shows %, not individuals)

**Option C avoids**:
- ❌ Streak anxiety
- ❌ Sunk cost fallacy
- ❌ Guilt messaging
- ❌ Re-entry barriers
- ❌ Gamification addiction

---

## 🗣️ Discussion Questions for Team

1. **Do we agree Option C best fits our anti-gamification philosophy?**
2. **Should we allow users to see "total reflections" count (e.g., 47 total)?**
   - Pro: Shows long-term engagement
   - Con: Could become competitive number
3. **What's the "engaged" threshold? (e.g., ≥3 days/week? ≥5 days/week?)**
4. **Should we show 4-week trend or just current week?**
5. **Any concerns about removing streaks entirely?**
   - Some users may want traditional streak tracking
   - Could we offer it as opt-in advanced feature later (V2.0)?

---

## 📊 Integration with Existing Features

### **Daily Check-In (Feature #2, P0)**:
- Weekly Progress Model is core design detail
- No additional screens needed
- Just changes metrics displayed on Dashboard

### **Progress Dashboard (Feature #5, P0)**:
- Shows weekly % trend chart (replaces streak graph)
- 4-week comparison view

### **Cohort Space (Feature #6, P0)**:
- Displays: "Your cohort averaged 72% check-ins this week"
- Anonymous, no individual rates visible

### **Milestone Celebrations (Feature #12, P2)**:
- Celebrates "Perfect weeks", "Consistent months"
- Never punishes low weeks

---

## 📝 Next Steps

**If team approves Option C**:
1. Update Feature #2 (Daily Check-In) implementation notes
2. Update Dashboard wireframes to show weekly % instead of streaks
3. Define "engaged" threshold (recommend: ≥3 check-ins/week)
4. Write supportive messaging copy
5. Design weekly progress chart UI

**Wireframe Priority**: Week 1 (Oct 25) - affects Dashboard design

---

**Created**: Oct 23, 2025
**For Discussion**: Oct 24 Team Meeting
**Recommendation**: Option C - Weekly Progress Model (No Streaks)
**Rationale**: Best alignment with anti-gamification + lowest re-entry barrier + survey-validated
