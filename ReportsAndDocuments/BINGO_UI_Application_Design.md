# BINGO Mechanism - UI Application Design

**Based on**: QuestLabs 5×5 Card System (from Instructions2.jpg)
**Designer**: Dong Zhang (Section 2 - Dashboard & Visualizations)
**Date**: 2025-10-16
**Status**: Design Specification for Wireframing

---

## 📋 Table of Contents

1. [Original BINGO System Analysis](#1-original-bingo-system-analysis)
2. [Digital Adaptation for QuestLabs Companion](#2-digital-adaptation)
3. [UI Components Specification](#3-ui-components)
4. [Interaction Design](#4-interaction-design)
5. [Integration with Cohort Features](#5-cohort-integration)
6. [Wireframe Requirements](#6-wireframe-requirements)

---

## 1. Original BINGO System Analysis

### 1.1 Physical Card Structure (from Instructions2.jpg)

**Layout**:

```
┌─────────────────────────────────────────────┐
│  QUEST LABS │ SCHOOL WORK │ HOME │ JOB     │
├─────────────┼─────────────┼──────┼─────────┤
│ onboarding  │  research   │ free │  free   │
│ offboarding │   consent   │      │         │
├─────────────┼─────────────┼──────┼─────────┤
│   abcdefg   │   Sandbox   │ free │  free   │
│  Futures    │  Sessions   │      │         │
│ Literacies  │             │      │         │
├─────────────┼─────────────┼──────┼─────────┤
│    Quest    │   Sandbox   │ free │  free   │
│    Board    │  Sessions   │      │         │
├─────────────┼─────────────┼──────┼─────────┤
│   digital   │   Sandbox   │ free │  free   │
│    garden   │  Sessions   │      │         │
├─────────────┼─────────────┼──────┼─────────┤
│    2032     │  Personal   │ free │  free   │
│   Dream CV  │Professional │      │         │
│             │  Evolution  │      │         │
└─────────────┴─────────────┴──────┴─────────┘
```

**Visual Design Elements**:

- **Background**: Pink (#E8A5D5)
- **Completed tasks**: Deep green filled squares (#2D7A5F)
- **Incomplete tasks**: White squares with "free" text
- **Category headers**: Bold, caps lock
- **Mascot**: Orange welcome character on right side

### 1.2 Key Design Insights

✅ **What Works**:

1. **5×5 grid provides clear structure** - Easy to see progress at a glance
2. **Color coding is instant** - Green = done, White = pending
3. **"Free" spaces provide flexibility** - Users can customize goals
4. **Category columns organize by life domain** - Work, school, home, personal
5. **Non-competitive visual** - No scores, ranks, or comparisons

✅ **Psychological Benefits**:

- **Visual satisfaction**: Filling squares triggers completion dopamine
- **Flexible framework**: Not rigid—allows personalization
- **Progress tracking**: See weekly/monthly patterns
- **No pressure**: "Free" spaces mean it's okay to adapt goals

---

## 2. Digital Adaptation for QuestLabs Companion

### 2.1 Core Modifications

**Changes from Physical to Digital**:

| Aspect         | Physical Card    | Digital App                      |
| -------------- | ---------------- | -------------------------------- |
| **Size**       | 5×5 (25 squares) | Flexible: 3×5 or 4×4 weekly view |
| **Categories** | Fixed columns    | Customizable by user's 5 Quests  |
| **Completion** | Emoji stickers   | Tap to fill + animation          |
| **Sharing**    | Photo upload     | Optional cohort visibility       |
| **Reset**      | New card weekly  | Auto-reset with archive          |

### 2.2 Proposed Digital Structure

```
Quest Board (Weekly View)

My 5 Quests This Week:
┌────────────┬────────────┬────────────┬────────────┬────────────┐
│ Academic   │  Wellness  │  Relation  │   Digital  │   Growth   │
│            │            │   ships    │    Diet    │            │
├────────────┼────────────┼────────────┼────────────┼────────────┤
│     ✅     │     ✅     │     ⬜     │     ✅     │     ⬜     │  Mon
├────────────┼────────────┼────────────┼────────────┼────────────┤
│     ✅     │     ⬜     │     ✅     │     ✅     │     ✅     │  Tue
├────────────┼────────────┼────────────┼────────────┼────────────┤
│     ⬜     │     ✅     │     ✅     │     ⬜     │     ⬜     │  Wed
├────────────┼────────────┼────────────┼────────────┼────────────┤
│     ✅     │     ✅     │     ⬜     │     ✅     │     ✅     │  Thu
├────────────┼────────────┼────────────┼────────────┼────────────┤
│     ⬜     │     ⬜     │     ✅     │     ⬜     │     ⬜     │  Fri
└────────────┴────────────┴────────────┴────────────┴────────────┘

Progress: 15/25 (60%) 🎉
"You're 10 squares away from a full BINGO week!"
```

### 2.3 Alternative: Monthly BINGO Card

For longer-term tracking:

- **4 weeks × 5 quests = 20 squares**
- **Milestone**: Complete 15/20 squares = monthly achievement
- **Flexibility**: Built-in buffer (5 "free" days)

---

## 3. UI Components Specification

### 3.1 Quest Board Main Screen

#### **Header Section**

```
┌──────────────────────────────────────────────┐
│  📊 Quest Board                    [⚙️ Edit] │
│  Week of Oct 14-20, 2025                     │
│                                              │
│  Progress: ████████████░░░░░░ 15/25 (60%)   │
│  "Great momentum! 10 more for full BINGO"   │
└──────────────────────────────────────────────┘
```

**Components**:

- Title with edit button (to change quest categories)
- Date range indicator
- Progress bar (visual + numerical)
- Encouragement message (dynamic based on progress)

---

#### **Grid Section**

**Individual Square Spec**:

```
┌─────────────┐
│  Academic   │  ← Category label (top)
│             │
│      ✅     │  ← Status icon (center)
│             │
│    Mon      │  ← Day label (bottom)
└─────────────┘
```

**Dimensions**:

- Square size: 64×64 dp (mobile)
- Padding: 4dp between squares
- Corner radius: 8dp (rounded corners)
- Border: 2dp solid #E0E0E0 (gray)

**States**:

1. **Empty** (⬜):

   - Background: White (#FFFFFF)
   - Border: Light gray (#E0E0E0)
   - Icon: Empty square outline

2. **Completed** (✅):

   - Background: Deep green (#2D7A5F)
   - Border: None
   - Icon: White checkmark
   - Animation: Scale + fade in (200ms)

3. **Skipped/Free** (Optional):

   - Background: Light gray (#F5F5F5)
   - Border: Dashed gray (#CCCCCC)
   - Icon: "—" (dash)

4. **Today** (Active):
   - Border: Teal (#5FC9C5) 3dp
   - Subtle pulse animation

---

#### **Footer Section**

```
┌──────────────────────────────────────────────┐
│  Quick Stats:                                │
│  🔥 Longest streak: 4 days                   │
│  ⭐ Best quest: Academic (5/5)               │
│  💪 Room for growth: Digital Diet (2/5)      │
│                                              │
│  [Share with Cohort] [View History]         │
└──────────────────────────────────────────────┘
```

**Components**:

- Quick insights (top 3 stats)
- Two action buttons:
  - "Share with Cohort" → Shows aggregated progress to group
  - "View History" → Opens monthly/quarterly archive

---

### 3.2 Quest Selection/Edit Screen

When user taps **[⚙️ Edit]**:

```
┌──────────────────────────────────────────────┐
│  ← Back          Edit Quests                 │
├──────────────────────────────────────────────┤
│  Choose your 5 focus areas for this week:   │
│                                              │
│  1. [Academic Progress    ]  [×]             │
│  2. [Emotional Wellness   ]  [×]             │
│  3. [Relationships        ]  [×]             │
│  4. [Digital Diet         ]  [×]             │
│  5. [Physical Health      ]  [×]             │
│                                              │
│  + Add custom quest                          │
│                                              │
│  Common suggestions:                         │
│  • School/Work                               │
│  • Family                                    │
│  • Fun/Recreation                            │
│  • Growth/Learning                           │
│  • Home/Organization                         │
│                                              │
│  [Cancel]                   [Save Changes]   │
└──────────────────────────────────────────────┘
```

**Functionality**:

- Drag to reorder quests
- Tap [×] to remove
- Tap "+ Add custom" to create new category
- Preset suggestions based on Wheel of Life dimensions

---

### 3.3 Daily Check-In Integration

When user completes Daily Check-In:

```
┌──────────────────────────────────────────────┐
│  ✅ Daily Check-In Complete!                 │
│                                              │
│  Which quests did you work on today?         │
│  (Select all that apply)                     │
│                                              │
│  ☑️ Academic Progress                        │
│  ☐ Emotional Wellness                        │
│  ☑️ Relationships                            │
│  ☐ Digital Diet                              │
│  ☐ Physical Health                           │
│                                              │
│  [Skip] [Continue]                           │
└──────────────────────────────────────────────┘
```

**Flow**:

1. User completes Daily Check-In (rates emotions 1-5)
2. System prompts: "Which quests did you work on today?"
3. User selects 1-5 categories
4. System fills corresponding squares on Quest Board
5. Celebration animation plays if milestone reached

---

## 4. Interaction Design

### 4.1 Tap Interactions

**Single Tap on Square**:

```
Action: Toggle completion status
Effect:
  If empty → Fill with green + checkmark
  If filled → Empty (undo)
Animation: 200ms scale + fade
Haptic: Light tap feedback (iOS/Android)
```

**Long Press on Square**:

```
Action: Show context menu
Options:
  • Mark as skipped (gray out)
  • Add note ("Why I worked on this")
  • View related reflections
  • [Cancel]
```

**Tap on Category Header**:

```
Action: Filter/highlight that quest
Effect: Dim other columns, show weekly trend
Example: "Academic: 4/5 days this week (+1 from last week)"
```

### 4.2 Completion Animations

**Milestone Animations**:

**50% Progress (12-13/25 squares)**:

- Confetti animation (pink + teal colors)
- Sound: Soft chime
- Message: "Halfway there! You're building great momentum 💪"

**75% Progress (18-19/25 squares)**:

- More intense confetti
- Sound: Achievement bell
- Message: "Almost a full BINGO! Just 7 more squares 🎉"

**100% Progress (25/25 squares)**:

- Full-screen celebration animation
- Fireworks + mascot character dancing
- Sound: Triumphant fanfare (short, 2 seconds)
- Message: "FULL BINGO! You crushed this week! 🌟"
- Unlocks: Badge, share option, cohort notification

**Animation Specs**:

- Duration: 1.5-2 seconds (not too long)
- Skippable: Tap anywhere to dismiss
- Frequency: Only on milestone moments, not every square

### 4.3 Gesture Interactions

**Swipe Left on Grid**:

```
Action: Go to previous week
Effect: Smooth horizontal slide transition
Archive View: Past weeks shown in read-only mode
```

**Swipe Right on Grid**:

```
Action: Go to next week (if available)
Effect: Smooth horizontal slide transition
Note: Future weeks show empty template
```

**Pinch to Zoom** (optional):

```
Action: Switch view modes
  Pinch in → Monthly view (4 weeks × 5 quests)
  Pinch out → Weekly view (7 days × 5 quests)
```

---

## 5. Cohort Integration

### 5.1 Sharing with Cohort

**Privacy-Preserving Design**:

When user taps **[Share with Cohort]**:

```
┌──────────────────────────────────────────────┐
│  Share Progress with Cohort?                 │
│                                              │
│  Your cohort will see:                       │
│  ✅ Your completion percentage (60%)         │
│  ✅ "Someone reached 60% this week!"         │
│                                              │
│  Your cohort will NOT see:                   │
│  ❌ Which specific quests you worked on      │
│  ❌ Your daily check-in ratings              │
│  ❌ Your personal notes                      │
│                                              │
│  [Cancel]              [Share]               │
└──────────────────────────────────────────────┘
```

**What Cohort Sees** (in their Progress Board):

```
┌──────────────────────────────────────────────┐
│  📊 Cohort Progress Board                    │
│                                              │
│  This Week's Quest Board Activity:           │
│  ████████████████░░░░░░  4/5 members active  │
│                                              │
│  • Someone completed 80% (amazing!)          │
│  • Someone reached 60% (great momentum!)     │
│  • Someone completed 50% (halfway there!)    │
│  • Someone reached 40% (keep it up!)         │
│                                              │
│  [Give encouragement] 👏                     │
└──────────────────────────────────────────────┘
```

**Key Privacy Features**:

- ✅ Only show completion percentages (not specific quests)
- ✅ Anonymous "someone" language (no names)
- ✅ Sorted by achievement level (not by name)
- ✅ Opt-in sharing (user must choose to share)

### 5.2 Cohort Quest Board Challenges (Optional Feature)

**Group Challenge Mode**:

```
┌──────────────────────────────────────────────┐
│  🎯 Cohort Challenge: Team BINGO             │
│                                              │
│  Goal: Complete 100 total squares as a team │
│  Progress: ████████░░░░  78/100 (78%)       │
│                                              │
│  Still need: 22 squares by Sunday!           │
│                                              │
│  Top contributors this week:                 │
│  🥇 Someone: 18/25                           │
│  🥈 Someone: 15/25                           │
│  🥉 Someone: 14/25                           │
│  4️⃣ Someone: 13/25                           │
│  5️⃣ You: 12/25                               │
│                                              │
│  [Encourage team] 💪                         │
└──────────────────────────────────────────────┘
```

**Design Considerations**:

- ⚠️ **Potential Issue**: Rankings might trigger comparison anxiety
- ✅ **Solution**: Show only top 3 + user's position
- ✅ **Alternative**: Remove rankings, show only total progress
- ✅ **Best Practice**: Make this an opt-in feature, not default

---

## 6. Wireframe Requirements

### 6.1 Screens to Design (Section 2 Responsibility)

**Priority 1 - Must Have**:

1. Quest Board Main Screen (weekly grid view)
2. Daily Check-In Quest Selection
3. Edit Quests Screen
4. Cohort Progress Board (aggregated view)

**Priority 2 - Should Have**: 5. Quest Board Archive/History View 6. Milestone Celebration Modal 7. Individual Quest Trend Graph (line chart showing weekly progress)

**Priority 3 - Nice to Have**: 8. Monthly BINGO Card View 9. Cohort Challenge Screen 10. Quest Notes/Reflection Detail View

### 6.2 Wireframe Annotations

For each screen, include:

**Layout Specs**:

- Grid dimensions (columns × rows)
- Square sizes (dp)
- Spacing (padding, margins)
- Typography (heading/body sizes)

**Color Codes**:

- Completed: #2D7A5F (deep green)
- Empty: #FFFFFF (white)
- Border: #E0E0E0 (light gray)
- Today highlight: #5FC9C5 (teal)
- Background: #FBF8F3 (off-white)

**Interaction Notes**:

- Tap behaviors (on square, on header, on buttons)
- Swipe gestures (left/right for week navigation)
- Long-press actions (context menu)

**Animation Triggers**:

- Square fill animation (200ms)
- Milestone celebration (at 50%, 75%, 100%)
- Cohort update notification

### 6.3 Integration Points with Other Sections

**Connection to Section 1 (Daily Check-In)**:

- After Daily Check-In → Prompt "Which quests did you work on?"
- Quest selection updates Quest Board automatically

**Connection to Section 3 (Cohort Space)**:

- "Share with Cohort" button → Sends aggregated data to Cohort Progress Board
- Cohort Challenge progress bar → Updates in real-time

**Connection to Dashboard**:

- Quest Board is a main tab/module in Dashboard
- Quick stats feed into overall Dashboard metrics

---

## 7. Technical Considerations

### 7.1 Data Structure

```json
{
  "user_id": "user123",
  "week": "2025-10-14",
  "quests": [
    {"id": 1, "name": "Academic Progress", "category": "school"},
    {"id": 2, "name": "Emotional Wellness", "category": "wellness"},
    {"id": 3, "name": "Relationships", "category": "social"},
    {"id": 4, "name": "Digital Diet", "category": "lifestyle"},
    {"id": 5, "name": "Physical Health", "category": "wellness"}
  ],
  "completions": [
    {"day": "2025-10-14", "quest_ids": [1, 2, 4]},
    {"day": "2025-10-15", "quest_ids": [1, 3, 4, 5]},
    {"day": "2025-10-16", "quest_ids": [2, 3]},
    ...
  ],
  "progress": {
    "total_squares": 25,
    "completed": 15,
    "percentage": 60
  },
  "shared_with_cohort": true,
  "cohort_id": "cohort_abc"
}
```

### 7.2 State Management

**Local State** (per device):

- Current week's grid data
- Unsaved changes (optimistic UI)
- Animation states

**Server State** (synced):

- Quest definitions (5 categories)
- Completion history (all weeks)
- Cohort sharing settings

**Sync Strategy**:

- Auto-save on every square tap (debounced)
- Pull latest data on app open
- Conflict resolution: Server wins (for cohort data)

---

## 8. Design Variations to Consider

### 8.1 Alternative Visual Styles

**Option A: Emoji-Based** (playful)

```
┌────────┬────────┬────────┐
│   📚   │   😊   │   🏃   │  Academic / Wellness / Fitness
│   ✅   │   ⬜   │   ✅   │  Mon
└────────┴────────┴────────┘
```

**Option B: Gradient-Based** (modern)

- Completed squares: Green gradient (#2D7A5F → #4CAF50)
- Empty squares: Light to dark gray gradient
- Today: Teal glow effect

**Option C: Minimalist** (clean)

- Remove all borders
- Use only background colors
- Checkmark appears on hover/tap only

**Recommendation**: **Option A (Emoji-Based)** for high-level view, **Standard (Checkmark)** for detailed grid.

### 8.2 Responsive Design

**Mobile (375px width)**:

- 5 columns × 5 rows
- Square size: 60×60 dp
- Scrollable if needed

**Tablet (768px width)**:

- 5 columns × 7 rows (show full week)
- Square size: 80×80 dp
- Side panel for quick stats

**Desktop (1024px+ width)**:

- Side-by-side view: Grid + Analytics
- Larger squares (100×100 dp)
- Hover effects (reveal notes on hover)

---

## 9. User Testing Questions

Before finalizing design, test with users:

1. **Clarity**: "What does this grid represent?"
2. **Motivation**: "Does seeing empty squares motivate you to fill them?"
3. **Flexibility**: "Do you like having 'free' or customizable quests?"
4. **Privacy**: "Would you be comfortable sharing your progress percentage with a small group?"
5. **Frequency**: "Would you prefer a daily grid (7 days) or weekly tasks (5 categories)?"

---

---

**File Created**: 2025-10-16
**Designer**: Dong Zhang
**Section**: Section 2 - Dashboard & Visualizations
