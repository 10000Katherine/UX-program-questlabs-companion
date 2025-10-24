# Survey Data Analysis Report - QuestLabs Companion

**Analysis Date**: October 23, 2025
**Analyst**: Dong Zhang
**Total Valid Responses**: **14**
**Survey Period**: October 16-23, 2025
**Survey Link**: https://docs.google.com/forms/d/e/1FAIpQLSecelozNUqU-wZzHfmVYWwrKLkcN-iYRBxQTutOt5N7o5qchw/viewform

---

## 📊 Executive Summary

Based on **14 valid survey responses** from college students aged 18-31+, this analysis validates core design assumptions for QuestLabs Companion and provides data-driven feature prioritization recommendations.

### 🎯 **Top 5 Key Findings**

1. **✅ Quick Check-In Design Validated**: 71% (10/14) want daily check-in **under 2 minutes**
2. **✅ Visual Dashboard is Critical**: 71% (10/14) prefer visual tracking formats
3. **✅ Long-Term Goal Tracking Most Desired**: 79% (11/14) rated 4-5 interest
4. **✅ Privacy-First Cohort Design Confirmed**: 71% (10/14) need control over sharing
5. **⚠️ Reminders Are Critical Missing Feature**: 64% (9/14) forget to reflect

---

## 📋 Section 1: Demographics & Screening

### Total Responses: **14 valid**
- Valid responses: 14
- Test responses removed: 0
- Incomplete responses: 0

### Q1: Student Status
```
Graduate student:           7   (50%)
Full-time undergraduate:    6   (43%)
Part-time undergraduate:    0   (0%)
Recent grad (within 2 yrs): 0   (0%)
Not a student:              1   (7%) - filtered out from analysis
```

**Key Insight**: **93% are current students** (13/14), evenly split between undergrad (46%) and grad students (54%). Sample is representative of target audience.

---

### Q2: Age Range
```
31+:    5   (36%)
27-30:  4   (29%)
24-26:  3   (21%)
21-23:  2   (14%)
18-20:  0   (0%)
```

**Key Insight**: **Mature student population** - 65% are 27+, indicating users value structured personal development. Higher age demographic may correlate with stronger goal-tracking needs.

---

### Q3: Personal Development Program Participation
```
No, but I'm interested:       7   (50%)
Yes, informally:              4   (29%)
Yes, structured program:      3   (21%)
No, not interested:           0   (0%)
```

**Key Insight**: **100% are open to personal development** (no one selected "not interested"). 50% already have cohort experience → users understand collaborative growth concepts.

---

## 📋 Section 2: Current Habits & Pain Points

### Q4: Reflection Frequency
```
Weekly:             6   (43%)
2-3 times/week:     5   (36%)
Daily:              2   (14%)
Rarely or never:    1   (7%)
Monthly or less:    0   (0%)
```

**Analysis**:
- **Active reflectors** (Daily + 2-3x/week): 50% (7/14)
- **Aspirational reflectors** (Weekly): 43% (6/14)
- **Non-reflectors** (Rarely/never): 7% (1/14)

**Key Insight**: **Only 14% reflect daily** → validates need for habit-building features. 43% "Weekly" reflectors are prime target for moving to more frequent engagement.

**Design Implication**: ✅ Daily Check-In is critical (P0) to build consistency habit.

---

### Q5: Biggest Challenges (Select up to 2)

**Note**: This is multi-select, so total > 14 responses

```
Forget to do it:              9   (64%)
I don't have time:            5   (36%)
I don't know what to reflect: 4   (29%)
Feels overwhelming/boring:    4   (29%)
Don't see value/results:      1   (7%)
Prefer talking to writing:    1   (7%)
Other:                        1   (7%)
```

**Top 3 Challenges**:
1. **Forget to do it**: 64% (9/14)
2. **Don't have time**: 36% (5/14)
3. **Don't know what to reflect**: 29% (4/14)

**Key Insight**: **"Forget" is #1 barrier** (64%) → **Push notifications/reminders are essential feature** (currently missing from proposal). "No time" (36%) validates <2 min design.

**Design Implications**:
- ⚠️ **Add "Reminders/Notifications" to P1 priority** (new feature)
- ✅ "Don't know what to reflect" (29%) → Structured prompts validated
- ✅ "Don't have time" (36%) → <2 min check-in design confirmed

---

### Q6: Current Tracking Tools
```
No, I don't track anything:    7   (50%)
Yes, but I stopped using them: 4   (29%)
No, use pen and paper:         2   (14%)
Yes, regularly:                1   (7%)
```

**Apps/Tools Mentioned**:
- **Regular users**: "doc" (1 mention)
- **Stopped users**: "Smiling Mind" (1 mention), "RefTime" (1 mention)

**Key Insight**: **50% don't track anything** + **29% stopped using apps** = **79% have unmet needs**. High abandonment rate validates opportunity for better-designed solution.

---

### Q7: Why Stopped Using Apps (n=4 who stopped)
```
Too time-consuming:      2   (50% of stoppers)
Privacy concerns:        1   (25%)
Felt like chore:         1   (25%)
Too complicated:         1   (25%)
```

**Key Insight**: **"Too time-consuming" is #1 quit reason** (50% of those who stopped) → reinforces <2 min design as competitive advantage.

**Design Implication**:
- ✅ If "Too time-consuming" → Reinforces <2 min design
- ✅ If "Privacy concerns" → Validates privacy-first cohort approach
- ✅ If "Felt like chore" → Must be intrinsically motivating, not obligation

---

## 📋 Section 3: Preferences & Design Validation

### Q8: Time Willingness for Daily Check-In
```
Under 1 minute:         7   (50%)
1-2 minutes:            4   (29%)
3-5 minutes:            2   (14%)
10+ minutes:            1   (7%)
5-10 minutes:           0   (0%)
```

**Analysis**:
- **Quick check-in preference** (<2 min): **79% (11/14)** ← KEY METRIC
- **Moderate time** (3-5 min): 14% (2/14)
- **Long form** (10+ min): 7% (1/14)

**Key Insight**: **79% want <2 min check-in → VALIDATES core design assumption!** This is the strongest validation in the entire survey.

**Design Implication**: ✅✅ Daily Check-In (<2 min) **P0 priority absolutely confirmed**

---

### Q9: Preferred Progress Tracking Format
```
Visual graphs and charts:  8   (57%)
Calendar/streak view:      4   (29%)
A mix of visuals/text:     2   (14%)
Written journal entries:   0   (0%)
Don't care about history:  0   (0%)
```

**Analysis**:
- **Visual preference** (Graphs + Mix): **71% (10/14)** ← KEY METRIC
- **Calendar/Streak**: 29% (4/14)
- **Text preference** (Journal only): 0%
- **Indifferent**: 0%

**Key Insight**: **71% prefer visual/mix → Progress Dashboard P0 priority VALIDATED!** Zero preference for text-only journals → visual design is non-negotiable.

**Design Implication**: ✅✅ Dashboard with trend graphs is **Must Have** (P0). Section 2 visualization work (Wheel of Life, SEL timeline, Affect-Agency grid) is core value.

---

### Q10: Feature Interest Matrix (Rate 1-5)

**Rating Distribution Analysis**:

| Feature | Avg Score | % Rating 4-5 (High Interest) | % Rating 1-2 (Low Interest) | Priority Recommendation |
|---------|-----------|------------------------------|-----------------------------|-----------------------|
| **Long-term goal tracking** | **4.1** | **79% (11/14)** | 14% | ⬆️ **Upgrade to P0** |
| **Encouragement reactions** | **3.9** | **64% (9/14)** | 21% | ⬆️ Consider upgrade to P1 |
| **Progress dashboard** | **3.7** | **64% (9/14)** | 21% | ✅ Keep P0 |
| **Quick daily check-in** | **3.6** | **57% (8/14)** | 21% | ✅ Keep P0 |
| **Peer aggregated progress** | **3.1** | **50% (7/14)** | 29% | ✅ Keep P1 |
| **Structured reflection prompts** | **3.2** | **50% (7/14)** | 29% | ✅ Keep P1 |

**Key Insights**:
- **Most desired**: **Long-term goal tracking** (79% high interest, highest avg 4.1) → **Should upgrade from P1 to P0**
- **Strong social desire**: Encouragement reactions (64% high interest) → validates peer interaction features
- **Dashboard validated**: 64% high interest confirms visualization priority
- **Structured prompts**: 50% interest → appropriate for P1 priority

**Surprise Finding**: 🚀 **Long-term goal tracking scored highest** (79%) - users want to connect daily actions to future aspirations. This aligns perfectly with "present awareness → future possibilities" motto.

---

### Q11: Ideal Reflection Tool Type
```
Give me clear structure (fill-in-blanks):     6   (43%)
Give me some structure + flexibility:         5   (36%)
Just let me rate quickly (minimal writing):   2   (14%)
Complete freedom (blank canvas):              1   (7%)
```

**Key Insight**: **79% (11/14) want structured guidance** (clear structure 43% + some structure 36%). Only 7% want blank canvas → validates fill-in-blank prompts over freeform journaling.

**Design Implication**:
- ✅ Structured Reflection Journal with prompts is validated (P1)
- ✅ Daily Check-In should minimize text input (rating-based)
- ❌ Do NOT create blank-page journal features

---

## 📋 Section 4: Social & Privacy Validation

### Q12: Privacy Comfort in Small Group (Select all that apply)

**Note**: Multi-select question, total > 14

```
Controlling what I share:             10  (71%)
Knowing members personally:            7   (50%)
No public profiles or rankings:        6   (43%)
Anonymous usernames:                   5   (36%)
Only group summaries (not details):    4   (29%)
I wouldn't share at all:               1   (7%)
```

**Top 3 Privacy Needs**:
1. **Controlling what I share**: 71% (10/14)
2. **Knowing members personally**: 50% (7/14)
3. **No public profiles/rankings**: 43% (6/14)

**Key Insight**: **71% need control over sharing** + **43% reject public rankings** → **validates aggregated cohort data design** and **anti-gamification philosophy**.

**Design Implication**:
- ✅ Cohort Space aggregated design VALIDATED (show group trends, not individual details)
- ✅ No leaderboards/badges/rankings (aligns with anti-gamification)
- ✅ Granular privacy controls needed (what to share with cohort)

---

### Q13: Peer Accountability Importance
```
Very important (need others):       5   (36%)
Somewhat important (helps):         4   (29%)
Not very important (independent):   5   (36%)
Not important at all (pressure):    0   (0%)
```

**Analysis**:
- **Social users** (Very + Somewhat): **64% (9/14)** ← KEY METRIC
- **Independent users** (Not very): 36% (5/14)
- **Anti-social** (Not at all): 0%

**Key Insight**: **64% find peer accountability important → VALIDATES Cohort Space as P0/P1 feature.** However, 36% prefer independence → app must work well in solo mode too.

**Design Implication**:
- ✅ Cohort Space is high priority (64% social users)
- ⚠️ Ensure solo mode is fully functional (36% independent users)
- ✅ No one finds accountability "pressure" → collaborative (not competitive) design is correct

---

### Q14: Helpful Group Support Types (Select up to 3)

**Note**: Multi-select, total > 14

```
Celebrating milestones together:      7   (50%)
Seeing my own progress:               7   (50%)
Giving/receiving encouragement:       6   (43%)
Weekly check-ins/standups:            5   (36%)
Accountability reminders from peers:  4   (29%)
Sharing struggles/challenges:         4   (29%)
One-on-one buddy system:              3   (21%)
Anonymous peer feedback:              2   (14%)
I prefer not to engage:               1   (7%)
```

**Top 5 Desired Support Types**:
1. **Celebrating milestones together**: 50% (7/14)
2. **Seeing own progress** (note: this was in motivations list): 50%
3. **Giving/receiving encouragement reactions**: 43% (6/14)
4. **Weekly check-ins/standups**: 36% (5/14)
5. **Accountability reminders from peers**: 29% (4/14)

**Key Insight**: **Celebration + Encouragement are top requests** → validates emoji reaction system + milestone animations in Cohort Space.

**Design Implication**:
- ✅ Milestone celebrations → P1 feature (50% want this)
- ✅ Encouragement reactions → P1 feature (43% + high rating in Q10)
- ⚠️ Weekly standups → Consider async check-in format (36%)

---

### Q15: App Usage Motivation (Select top 3)

**Note**: Multi-select (top 3), total ~42 selections

```
Seeing my own progress over time:        11  (79%)
Achieving my long-term goals:            9   (64%)
Quick and easy to use:                   8   (57%)
Understanding patterns in emotions:      7   (50%)
Feeling part of supportive community:    5   (36%)
Encouragement from peers:                4   (29%)
Beautiful, enjoyable interface:          3   (21%)
Reminders and notifications:             1   (7%)
```

**Top 3 Motivators**:
1. **Seeing my own progress**: 79% (11/14) ← #1 MOTIVATOR
2. **Achieving long-term goals**: 64% (9/14)
3. **Quick and easy to use**: 57% (8/14)

**Key Insight**: **"Seeing progress" is #1 driver** (79%) → **Visual feedback loops are critical for retention**. "Quick and easy" (57%) reinforces <2 min design. Interestingly, "Beautiful interface" is low priority (21%) → function over form.

**Design Implication**:
- ✅ Progress Dashboard must show **visible change over time** (charts, streaks, trends)
- ✅ "Quick and easy" (57%) → Reinforces low-friction UX
- ⚠️ "Beautiful interface" low (21%) → Focus on clarity over aesthetics
- ✅ Goal achievement (64%) → Three-layer goal framework validated

---

## 📋 Section 5: Open-Ended Feedback (Qualitative Gold)

### Q16: Magic Wand Feature (Must Have)

**Responses received**: 3 substantive answers (21% response rate)

**Themes Identified**:

**Theme 1: Goal Clarity & Progress Visualization** - 2 mentions
- _"Define your specific goals, clarify the path to achieving them, and visualize success progression in your application."_ - Respondent #5
- _"long term goal"_ - Respondent #3

**Theme 2: Emotional Connection** - 1 mention
- _"Caring about people, emotional connection"_ - Respondent #5

**Theme 3: Simple, Self-Explanatory UX** - 1 mention
- _"Easy and self-explanatory user interface"_ - Respondent #15

**Key Insight**: Users want **goal visualization** + **path clarity** + **emotional connection** → validates three-layer goal framework + emotional wellness integration.

---

### Q17: Additional Thoughts on Cohort Tracking

**Responses received**: 1 substantive answer (7% response rate)

**Theme: Privacy Concerns**
- _"How is privacy being handled"_ - Respondent #15

**Key Insight**: Even with one response, privacy is explicitly called out → reinforces privacy-first cohort design is critical.

---

## 🎯 Executive Summary - Top 5 Key Findings

### **Key Finding #1: Quick Check-In Design Validated** ✅
**Data**: 79% (11/14) prefer under 2 minutes for daily check-in
**Design Impact**: Validates core assumption - quick interaction is essential
**Action**: Daily Check-In remains **P0 Must Have** feature

---

### **Key Finding #2: Visual Dashboard is Non-Negotiable** ✅
**Data**: 71% (10/14) prefer visual tracking (graphs/charts/mix)
**Design Impact**: Visualization is core value proposition
**Action**: Progress Dashboard remains **P0 Must Have** - Dong's Section 2 work (Wheel of Life, SEL timeline, Affect-Agency grid) is validated

---

### **Key Finding #3: Long-Term Goal Tracking Should Be P0** ⬆️
**Data**: 79% (11/14) rated 4-5 interest (highest of all features, avg 4.1)
**Design Impact**: Users want to connect daily actions to future aspirations
**Action**: **Upgrade Long-Term Goal Tracking from P1 to P0**

---

### **Key Finding #4: Privacy-First Cohort Design Confirmed** ✅
**Data**: 71% (10/14) need to control what they share; 64% (9/14) find peer accountability important
**Design Impact**: Users want social support WITHOUT exposed data
**Action**: Cohort Space aggregated design validated - show group progress, not individual details (P0/P1)

---

### **Key Finding #5: Reminders Are Critical Missing Feature** ⚠️
**Data**: 64% (9/14) forget to reflect (top barrier)
**Design Impact**: Habit formation requires reminder system
**Action**: **Add "Push Notifications/Reminders" to P1 priority** (not currently in proposal)

---

## 📊 Feature Priority Updates

**Based on survey data, recommend updates to Feature Prioritization Matrix**:

### Features to Boost Priority:

| Feature | Old Priority | New Priority | Reason |
|---------|-------------|--------------|--------|
| **Long-Term Goal Tracking** | P1 | **P0** | 79% high interest (4-5 rating), highest avg score 4.1 |
| **Encouragement Reactions** | P2 (if exists) | **P1** | 64% high interest + 43% want in cohort support |
| **Push Notifications/Reminders** | Not listed | **P1** | 64% forget to reflect - critical for habit formation |

### Features Validated (No Change):

| Feature | Priority | Validation |
|---------|----------|------------|
| **Daily Check-In (<2 min)** | P0 | ✅ 79% want <2min, strongest validation |
| **Progress Dashboard** | P0 | ✅ 71% prefer visual tracking, 64% high interest rating |
| **Cohort Space (aggregated)** | P0/P1 | ✅ 64% find peer accountability important, 71% need sharing control |
| **Structured Reflection Prompts** | P1 | ✅ 79% want structured guidance, 29% don't know what to reflect on |

### Features to Consider Lowering (if applicable):

| Feature | Old Priority | New Priority | Reason |
|---------|-------------|--------------|--------|
| Any "blank canvas" freeform journaling | P1/P2 | P3 or Remove | Only 7% want complete freedom |
| Beautiful/decorative UI elements | P2 | P3 | Only 21% motivated by "beautiful interface" - function > form |

---

## 👥 User Segmentation Analysis

### **Segment 1: Aspirational Reflectors** (Primary Persona)
**Definition**: Reflect weekly or 2-3x/week, want to build daily habit
**Size**: 79% (11/14) of respondents

**Characteristics**:
- Reflection frequency: Weekly (43%) or 2-3x/week (36%)
- Time willingness: <2 min (79%)
- Top challenge: **Forget to do it** (64%)
- Preferred features: Visual dashboard (71%), Quick check-in (79%), Goal tracking (79%)

**Design Implications**:
- **Primary target** - design for habit formation
- Need: Reminders, low friction (<2 min), visible progress feedback
- Pain: Forgetting, lack of time → solution: push notifications + streamlined UX

---

### **Segment 2: Social Learners** (64% of users)
**Definition**: Find peer accountability important (Very or Somewhat)
**Size**: 64% (9/14)

**Characteristics**:
- Peer accountability: Very (36%) or Somewhat (29%) important
- Want: Celebrating milestones (50%), Encouragement reactions (43%)
- Privacy needs: Control sharing (71%), No rankings (43%)

**Design Implications**:
- Cohort Space is essential for this segment
- Need: Aggregated progress visibility + encouragement interactions
- Must have: Granular privacy controls

---

### **Segment 3: Independent Trackers** (36% of users)
**Definition**: Prefer working independently
**Size**: 36% (5/14)

**Characteristics**:
- Peer accountability: Not very important
- Still use visual tracking and goals

**Design Implications**:
- App must work fully in solo mode
- Cohort features should be **opt-in**, not required
- Ensure individual dashboard is complete experience

---

### **Segment 4: Mature Students** (65% are 27+)
**Definition**: Age 27-31+
**Size**: 65% (9/14)

**Characteristics**:
- Higher age, likely more experienced with personal development
- 50% already in informal/structured programs
- High interest in long-term goals (79%)

**Design Implications**:
- Don't patronize with gamification
- Focus on meaningful progress toward life goals
- Structured, intentional design (not playful/casual)

---

## 💬 Notable User Quotes (For Presentations)

### On Goal Clarity:
> _"Define your specific goals, clarify the path to achieving them, and visualize success progression in your application."_ - Respondent #5 (Graduate student, 31+)

### On Emotional Connection:
> _"Caring about people, emotional connection"_ - Respondent #5

### On Privacy:
> _"How is privacy being handled"_ - Respondent #15 (Undergraduate, 24-26)

### On Usability:
> _"Easy and self-explanatory user interface"_ - Respondent #15

### On Time Barriers:
Multiple respondents selected: _"I don't have time; I forget to do it"_ as top barriers

---

## ✅ Recommendations

### **Design Decisions Validated by Data**:
1. ✅ **<2 minute daily check-in** (79% support)
2. ✅ **Visual progress dashboard** (71% prefer visual, 64% high interest)
3. ✅ **Structured prompts over blank pages** (79% want structure)
4. ✅ **Aggregated cohort data (not individual)** (71% need sharing control)
5. ✅ **Anti-gamification approach** (43% reject public rankings)

### **Feature Priority Changes to Discuss**:
1. ⬆️ **Upgrade Long-Term Goal Tracking to P0** (79% high interest, highest score)
2. ⬆️ **Add Push Notifications/Reminders to P1** (64% forget to reflect)
3. ⬆️ **Consider Encouragement Reactions for P1** (64% interest, 43% want it)

### **Key Design Principles Confirmed**:
- **Function over form**: 57% value "quick and easy", only 21% care about "beautiful interface"
- **Progress visibility is #1 motivator**: 79% motivated by seeing their own progress
- **Privacy is non-negotiable**: Explicitly mentioned in open feedback
- **Solo mode must work**: 36% prefer independence

---

## 📈 Next Steps After This Analysis

### **Immediate Actions** (Oct 23 - today):
- ✅ Complete this analysis report
- ✅ Present 5 key findings to team in morning meeting
- ✅ Discuss feature priority changes

### **For Oct 25-28** (Figma Design Phase):
- [ ] Update Feature Prioritization Matrix with new scores
- [ ] Use visual tracking insight (71%) to prioritize Section 2 dashboard work
- [ ] Design reminder/notification interaction patterns
- [ ] Ensure privacy controls are prominent in Cohort Space wireframes

### **For Nov 4+ Design Sprint**:
- [ ] Reference quotes in design justifications
- [ ] Keep "79% want <2 min" visible when designing all flows
- [ ] Test wireframes against user pain points (forget, no time, need structure)

---

## 📎 Appendix: Raw Data Summary

### Response Timeline:
- First response: Oct 16, 9:03 AM MDT
- Last response: Oct 23, 8:51 PM MDT
- Collection period: **7 days**

### Demographics Breakdown:
- **Students**: 13 (93%)
- **Graduate students**: 7 (50%)
- **Undergraduates**: 6 (43%)
- **Age 27+**: 9 (64%)
- **Personal dev experience**: 7 (50% informal/structured)

### Response Quality:
- Complete responses: 14 (100%)
- Open-ended response rate: 21% (3/14 answered magic wand question)
- Average completion time: Not tracked

---

**Report Completed**: October 23, 2025
**Total Analysis Time**: ~3 hours
**Analyst**: Dong Zhang (Student ID: 300403848)
**Course**: CSIS 3375 - Section 1, Douglas College
**Project**: QuestLabs Companion - User Research Phase

**Next Deliverable**: Updated Feature Prioritization Matrix (Oct 25)
