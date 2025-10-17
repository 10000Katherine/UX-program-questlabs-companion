# Survey Data Analysis Template - QuestLabs Companion

**Analysis Date**: Oct 11, 2025 (or when 15+ responses collected)
**Analyst**: Dong Zhang
**Survey Link**: https://docs.google.com/forms/d/e/1FAIpQLSecelozNUqU-wZzHfmVYWwrKLkcN-iYRBxQTutOt5N7o5qchw/viewform
**Goal**: Extract key insights to validate design decisions and update Feature Prioritization Matrix

---

## 📊 Quick Start Guide

### Step 1: Export Data from Google Forms
1. Open your Google Form
2. Click "Responses" tab
3. Click the green Google Sheets icon (top right)
4. This creates a spreadsheet with all responses

### Step 2: Clean Data (in Google Sheets)
1. Remove any test responses
2. Check for incomplete submissions
3. Note: Keep partial responses if they answered key questions

### Step 3: Fill Out This Template
Use this document as your analysis notebook. Copy-paste key findings, percentages, and quotes.

---

## 🎯 Analysis Framework

### Three Types of Insights to Extract:

1. **Quantitative**: Percentages, averages, distributions
   - Used to validate design assumptions
   - Updates Feature Prioritization Matrix scores
   - Example: "70% prefer visual tracking"

2. **Qualitative**: User quotes, pain points, desires
   - Used in presentations and design justifications
   - Adds human context to numbers
   - Example: "I forget to track because it feels like a chore"

3. **Segmentation**: User groups with different needs
   - Used to identify primary vs. secondary personas
   - Informs feature prioritization
   - Example: "Active reflectors" vs. "Aspirational reflectors"

---

## 📋 Section 1: Demographics & Screening

### Total Responses: [FILL IN]
- Valid responses: [FILL IN]
- Removed (test/incomplete): [FILL IN]

### Q1: Student Status
```
Full-time undergraduate:    [XX]  [XX%]
Part-time undergraduate:    [XX]  [XX%]
Graduate student:           [XX]  [XX%]
Recent grad (within 2 yrs): [XX]  [XX%]
```

**Key Insight**: [Write 1-2 sentences about your respondent pool]

Example: "85% are full-time undergrads, our primary target audience. Sample is representative."

---

### Q2: Age Range
```
18-20:  [XX]  [XX%]
21-23:  [XX]  [XX%]
24-26:  [XX]  [XX%]
27-30:  [XX]  [XX%]
```

**Key Insight**: [Age distribution analysis]

Example: "Majority (60%) are 21-23, matching typical college demographic."

---

### Q3: Personal Development Program Participation
```
Yes, structured program:  [XX]  [XX%]
Yes, informal:            [XX]  [XX%]
No, but interested:       [XX]  [XX%]
No, not interested:       [XX]  [XX%]
```

**Key Insight**: [Familiarity with structured programs]

Example: "40% have structured program experience → familiar with cohort concepts."

---

## 📋 Section 2: Current Habits & Pain Points

### Q4: Reflection Frequency
```
Daily:              [XX]  [XX%]
2-3 times/week:     [XX]  [XX%]
Weekly:             [XX]  [XX%]
Monthly or less:    [XX]  [XX%]
Rarely or never:    [XX]  [XX%]
```

**Analysis**:
- **Active reflectors** (Daily + 2-3x/week): [XX%]
- **Aspirational** (Weekly + Monthly): [XX%]
- **Non-reflectors** (Rarely/never): [XX%]

**Key Insight**: [Habit formation challenge]

Example: "Only 25% reflect daily → validates need for habit-building features."

**Design Implication**:
- [ ] ✅ If <30% daily → Daily Check-In is critical (validates P0 priority)
- [ ] ⚠️ If >60% daily → Consider more advanced features for power users

---

### Q5: Biggest Challenges (Select up to 2)
```
Don't have time:              [XX]  [XX%]
Don't know what to reflect:   [XX]  [XX%]
Feels overwhelming/boring:    [XX]  [XX%]
Forget to do it:              [XX]  [XX%]
Don't see value/results:      [XX]  [XX%]
Prefer talking to writing:    [XX]  [XX%]
Other:                        [XX]  [XX%]
```

**Top 3 Challenges**:
1. [Challenge Name]: [XX%]
2. [Challenge Name]: [XX%]
3. [Challenge Name]: [XX%]

**Key Insight**: [What blocks users most]

Example: "Top challenge: 'Forget to do it' (45%) → need reminders + low-friction design."

**Design Implication**:
- If "Don't know what to reflect" is high → Structured prompts are critical
- If "Don't have time" is high → <2 min check-in is validated
- If "Forget to do it" is high → Push notifications needed

---

### Q6: Current Tracking Tools
```
Yes, regularly (which tools?):  [XX]  [XX%]
  ↳ Tools mentioned: [List top 3-5 apps]
Yes, but stopped:               [XX]  [XX%]
No, use pen and paper:          [XX]  [XX%]
No, don't track anything:       [XX]  [XX%]
```

**Popular Apps Mentioned**:
1. [App Name] - mentioned [X] times
2. [App Name] - mentioned [X] times
3. [App Name] - mentioned [X] times

**Key Insight**: [Tool usage patterns]

Example: "50% stopped using apps → high churn validates need for sustained engagement design."

---

### Q7: Why Stopped Using Apps (if applicable)
```
Too time-consuming:                [XX]  [XX%]
Too complicated:                   [XX]  [XX%]
Felt like chore, not helpful:      [XX]  [XX%]
Didn't integrate life areas:       [XX]  [XX%]
Privacy concerns:                  [XX]  [XX%]
Other:                             [XX]  [XX%]
```

**Key Insight**: [Why apps fail]

Example: "33% stopped because 'felt like chore' → must be intrinsically motivating, not obligation."

**Design Implication**:
- If "Too time-consuming" → Reinforces <2 min design
- If "Too complicated" → Simple UI is critical
- If "Didn't integrate life areas" → Validates holistic 3-dimension tracking

---

## 📋 Section 3: Preferences & Design Validation

### Q8: Time Willingness for Daily Check-In
```
Under 1 minute:              [XX]  [XX%]
1-2 minutes:                 [XX]  [XX%]
3-5 minutes:                 [XX]  [XX%]
5-10 minutes:                [XX]  [XX%]
10+ minutes:                 [XX]  [XX%]
```

**Analysis**:
- **Quick check-in preference** (<2 min): [XX%]
- **Moderate time** (3-5 min): [XX%]
- **Long form** (5+ min): [XX%]

**Key Insight**: [Time constraint validation]

Example: "70% want <2 min check-in → VALIDATES core design assumption!"

**Design Implication**:
- [ ] ✅ If 60%+ choose <2 min → Daily Check-In P0 priority confirmed
- [ ] ⚠️ If 40%+ choose 5+ min → Consider optional extended reflection mode

---

### Q9: Preferred Progress Tracking Format
```
Visual graphs and charts:     [XX]  [XX%]
Written journal entries:      [XX]  [XX%]
Calendar/streak view:         [XX]  [XX%]
Mix of visuals and text:      [XX]  [XX%]
Don't care about history:     [XX]  [XX%]
```

**Analysis**:
- **Visual preference** (Graphs + Mix): [XX%]
- **Text preference** (Journal only): [XX%]
- **Indifferent**: [XX%]

**Key Insight**: [Visual dashboard validation]

Example: "75% prefer visual/mix → Progress Dashboard P0 priority VALIDATED!"

**Design Implication**:
- [ ] ✅ If 70%+ visual → Dashboard is Must Have
- [ ] Consider secondary text view for 20-30% who prefer writing

---

### Q10: Feature Interest Matrix (Rate 1-5)

**Instructions for Analysis**:
1. Calculate average score (1-5) for each feature
2. Calculate % rating 4-5 (high interest)
3. Use to update Feature Prioritization Matrix

| Feature | Avg Score | % High Interest (4-5) | Priority Update |
|---------|-----------|----------------------|-----------------|
| Quick daily mood check-in | [X.X] | [XX%] | [Keep P0 / Adjust] |
| Long-term goal tracking | [X.X] | [XX%] | [Keep P1 / Adjust] |
| Structured reflection prompts | [X.X] | [XX%] | [Keep P2 / Adjust] |
| Progress dashboard w/ graphs | [X.X] | [XX%] | [Keep P0 / Adjust] |
| Peer group aggregated progress | [X.X] | [XX%] | [Keep P0 / Adjust] |
| Give/receive encouragement | [X.X] | [XX%] | [Keep P1 / Adjust] |

**Priority Update Rules**:
- If % High Interest >70% → Boost by 1 tier (P1→P0, P2→P1)
- If % High Interest <40% → Drop by 1 tier (P0→P1, P1→P2)
- If % High Interest 40-70% → Keep current tier

**Key Insights**:
- **Most desired**: [Feature with highest %]
- **Least desired**: [Feature with lowest %]
- **Surprises**: [Any unexpected results]

Example: "Daily check-in: 85% high interest → CONFIRMS P0. Reflection prompts: only 35% → consider dropping to P3."

---

### Q11: Ideal Reflection Tool Type
```
Complete freedom (blank canvas):      [XX]  [XX%]
Some structure + flexibility:         [XX]  [XX%]
Clear structure (fill-in-blanks):     [XX]  [XX%]
Quick ratings only (minimal writing): [XX]  [XX%]
```

**Key Insight**: [Structure preference]

Example: "60% want 'some structure + flexibility' → validates fill-in-blank prompts over blank pages."

**Design Implication**:
- If "Clear structure" + "Some structure" >70% → Structured Reflection Journal is valuable
- If "Quick ratings only" >50% → Daily Check-In should minimize text input

---

## 📋 Section 4: Social & Privacy Validation

### Q12: Privacy Comfort in Small Group (Select all that apply)
```
Knowing members personally:           [XX]  [XX%]
Only group summaries (not details):   [XX]  [XX%]
Controlling what I share:             [XX]  [XX%]
No public profiles or rankings:       [XX]  [XX%]
Anonymous usernames:                  [XX]  [XX%]
Wouldn't share at all:                [XX]  [XX%]
```

**Top 3 Privacy Needs**:
1. [Privacy feature]: [XX%]
2. [Privacy feature]: [XX%]
3. [Privacy feature]: [XX%]

**Key Insight**: [Privacy requirements]

Example: "'Only group summaries' (70%) + 'Control what I share' (65%) → validates aggregated data design."

**Design Implication**:
- If "Only group summaries" >60% → Cohort Space aggregated design VALIDATED
- If "Wouldn't share at all" >30% → Need strong opt-in/opt-out controls

---

### Q13: Peer Accountability Importance
```
Very important (need others):       [XX]  [XX%]
Somewhat important (helps):         [XX]  [XX%]
Not very important (independent):   [XX]  [XX%]
Not important at all (pressure):    [XX]  [XX%]
```

**Analysis**:
- **Social users** (Very + Somewhat): [XX%]
- **Independent users** (Not very + Not at all): [XX%]

**Key Insight**: [Social vs. solo preference]

Example: "65% find peer accountability important → VALIDATES Cohort Space as P0 feature."

**Design Implication**:
- [ ] ✅ If >60% social → Cohort Space is Must Have
- [ ] If 30-40% independent → Ensure app works well without social features too

---

### Q14: Helpful Group Support Types (Select up to 3)

```
Weekly check-ins/standups:           [XX]  [XX%]
Celebrating milestones:              [XX]  [XX%]
Accountability reminders:            [XX]  [XX%]
Sharing struggles openly:            [XX]  [XX%]
Encouragement reactions:             [XX]  [XX%]
Collaborative goal-setting:          [XX]  [XX%]
Seeing others' progress:             [XX]  [XX%]
Anonymous peer feedback:             [XX]  [XX%]
One-on-one buddy system:             [XX]  [XX%]
Prefer not to engage:                [XX]  [XX%]
Other:                               [XX]  [XX%]
```

**Top 5 Desired Support Types**:
1. [Support type]: [XX%]
2. [Support type]: [XX%]
3. [Support type]: [XX%]
4. [Support type]: [XX%]
5. [Support type]: [XX%]

**Key Insight**: [Specific cohort features to prioritize]

Example: "Top requests: 'Encouragement reactions' (55%) and 'Celebrating milestones' (50%) → validates emoji system + milestone animations."

**Design Implication**:
- High-demand features → Add to P1 (High Priority)
- Low-demand features (<20%) → Consider dropping or making optional

---

### Q15: App Usage Motivation (Rank top 3)

**Note**: This question asks users to rank. In Google Sheets:
1. Assign points: 1st choice = 3 pts, 2nd = 2 pts, 3rd = 1 pt
2. Sum points for each motivation
3. Rank by total points

| Motivation | Total Points | Rank |
|------------|--------------|------|
| Seeing my own progress | [XX] | [X] |
| Encouragement from peers | [XX] | [X] |
| Achieving long-term goals | [XX] | [X] |
| Understanding patterns | [XX] | [X] |
| Supportive community | [XX] | [X] |
| Quick and easy to use | [XX] | [X] |
| Beautiful interface | [XX] | [X] |
| Reminders/notifications | [XX] | [X] |

**Top 3 Motivators**:
1. [Motivator]: [XX points]
2. [Motivator]: [XX points]
3. [Motivator]: [XX points]

**Key Insight**: [What drives sustained use]

Example: "'Seeing my own progress' ranked #1 → Progress Dashboard visual feedback is critical."

**Design Implication**:
- Top motivator → Ensure this is prominent in UX
- If "Quick and easy" ranks high → Reinforces <2 min design
- If "Beautiful interface" ranks low → Focus on function over form

---

## 📋 Section 5: Open-Ended Feedback (Qualitative Gold)

### Q16: Magic Wand Feature (Must Have)

**Instructions**:
1. Read all responses
2. Group into themes (e.g., "visual progress", "peer support", "reminders")
3. Count frequency of each theme
4. Extract 3-5 powerful quotes

**Themes Identified**:

**Theme 1: [Theme Name]** - mentioned [X] times
- Quote: "_[Exact user quote]_"
- Quote: "_[Another quote]_"

**Theme 2: [Theme Name]** - mentioned [X] times
- Quote: "_[Exact user quote]_"

**Theme 3: [Theme Name]** - mentioned [X] times
- Quote: "_[Exact user quote]_"

**Example**:
```
Theme 1: Visual Progress Tracking - 8 mentions
- "I need to SEE my progress over time, not just remember it"
- "Graphs that show when I'm doing well emotionally vs. not"

Theme 2: Low-Friction Design - 6 mentions
- "Something that takes 30 seconds, not 10 minutes"
- "I want to tap a few buttons and be done"
```

**Key Insight**: [What users truly need]

Example: "Visual progress + low-friction are most requested → validates Dashboard + Quick Check-In."

---

### Q17: Additional Thoughts on Cohort Tracking

**Instructions**: Same as Q16 - identify themes and extract quotes

**Themes Identified**:

**Theme 1: [Theme Name]** - mentioned [X] times
- Quote: "_[Exact user quote]_"

**Theme 2: [Theme Name]** - mentioned [X] times
- Quote: "_[Exact user quote]_"

**Key Insight**: [Concerns or ideas about social features]

Example: "Many express privacy concerns → reinforces aggregated-only data design."

---

## 🎯 Executive Summary

**Copy this section to presentation/report**:

### Key Finding #1: [Most Important Insight]
**Data**: [Percentage or stat]
**Design Impact**: [What this means for design]
**Action**: [Update to Feature Matrix or design decision]

Example:
```
Key Finding #1: Users Want <2 Minute Daily Check-Ins
Data: 72% prefer under 2 minutes for daily check-in
Design Impact: Validates core design assumption - quick interaction is essential
Action: Daily Check-In remains P0 Must Have feature
```

---

### Key Finding #2: [Second Most Important]
**Data**: [Percentage or stat]
**Design Impact**: [What this means for design]
**Action**: [Update to Feature Matrix]

---

### Key Finding #3: [Third Most Important]
**Data**: [Percentage or stat]
**Design Impact**: [What this means for design]
**Action**: [Update to Feature Matrix]

---

### Key Finding #4-5: [Additional Insights]
(Repeat format)

---

## 📊 Feature Priority Updates

**Based on survey data, update Feature_Prioritization_Matrix.md**:

### Features to Boost Priority:

| Feature | Old Priority | New Priority | Reason |
|---------|-------------|--------------|--------|
| [Feature Name] | P2 | P1 | [XX% high interest, above threshold] |
| [Feature Name] | P1 | P0 | [XX% critical need identified] |

### Features to Lower Priority:

| Feature | Old Priority | New Priority | Reason |
|---------|-------------|--------------|--------|
| [Feature Name] | P1 | P2 | [Only XX% interest, below threshold] |

### Features Validated (No Change):

| Feature | Priority | Validation |
|---------|----------|------------|
| Daily Check-In | P0 | ✅ [XX% want <2min, XX% rate high interest] |
| Cohort Space | P0 | ✅ [XX% find peer accountability important] |
| Dashboard | P0 | ✅ [XX% prefer visual tracking] |

---

## 💬 Notable User Quotes (For Presentations)

**Select 5-8 powerful quotes that tell the story**:

### On Time Constraints:
> "_[Quote about not having time]_" - Respondent #[X]

### On Privacy:
> "_[Quote about privacy concerns]_" - Respondent #[X]

### On Motivation:
> "_[Quote about staying motivated]_" - Respondent #[X]

### On Current App Failures:
> "_[Quote about why they stopped using other apps]_" - Respondent #[X]

### On Social Accountability:
> "_[Quote about peer support]_" - Respondent #[X]

**Usage**: Insert these quotes into:
- Oct 9 presentation slides
- Feature prioritization discussions
- Design justification documents

---

## 📈 Segmentation Analysis (Optional but Valuable)

### Segment 1: Active Reflectors
**Definition**: Reflect daily or 2-3x/week
**Size**: [XX%] of respondents

**Characteristics**:
- Time willingness: [X.X min average]
- Top challenges: [List]
- Preferred features: [List]

**Design Implications**: [What this segment needs]

---

### Segment 2: Aspirational Reflectors
**Definition**: Reflect weekly or monthly
**Size**: [XX%] of respondents

**Characteristics**:
- Time willingness: [X.X min average]
- Top challenges: [List]
- Preferred features: [List]

**Design Implications**: [What this segment needs]

---

### Segment 3: Social vs. Independent
**Social Users** (peer accountability very/somewhat important): [XX%]
**Independent Users** (not very/not at all important): [XX%]

**Design Implication**:
- If 60%+ social → Cohort features are critical
- If 40%+ independent → Ensure solo mode works well

---

## ✅ Next Steps After Analysis

**Immediate Actions** (same day):
- [ ] Update `Feature_Prioritization_Matrix.md` with new User Value scores
- [ ] Recalculate priority scores using formula
- [ ] Document any features that changed tiers

**For Oct 14 Meeting**:
- [ ] Present Executive Summary (3-5 key findings)
- [ ] Show updated Feature Priority Matrix
- [ ] Discuss any surprising insights
- [ ] Confirm P0 + P1 features for wireframing

**For Design Phase** (Oct 21+):
- [ ] Use quotes in design justifications
- [ ] Reference data when making design decisions
- [ ] Keep user pain points visible during wireframing

---

## 📎 Appendix: Data Export Format

**From Google Sheets, create these views**:

### View 1: Summary Table
```
Question | Option | Count | Percentage
---------|--------|-------|------------
Q8: Time | <1 min | 5 | 33%
Q8: Time | 1-2 min| 7 | 47%
...
```

### View 2: Crosstab Analysis (Optional)
Compare segments:
```
             | Active Reflectors | Aspirational
-------------|-------------------|-------------
Want <2 min  | 80%              | 60%
Visual pref  | 90%              | 70%
Social need  | 75%              | 50%
```

---

**Template Created**: 2025-10-16
**Last Updated**: [Fill in after analysis]
**Analyst**: Dong Zhang
**Responses Analyzed**: [Fill in final count]
**Analysis Duration**: [Fill in - aim for 2-3 hours]

**Pro Tips**:
- Do analysis in one sitting (maintain focus)
- Use Google Sheets built-in charts for quick visualization
- Don't overthink - look for clear patterns
- Trust your instincts on qualitative themes
- When in doubt, quote the user directly
