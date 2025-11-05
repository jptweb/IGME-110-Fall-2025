# P3 Deliverable #2 Example: MealMate Recipe App

**NOTE TO STUDENTS:** This is a example showing what your team needs to submit by the start of next class. Use this as a template to create your own deliverable for YOUR app! Be sure to read all the instructions though; this is more meant as an overview to help answer questions.

---

## Example App: MealMate

**High Concept:** A recipe discovery and meal planning app for college students

**Core Features:** Recipe search, grocery lists, meal planner, recipe saving, timers, ingredient substitutions, budget tracking

**Three Personas:** (you already did these in forst deliverable but adding this to give context).
- **Primary User - "Busy Brian":** 19yo freshman, limited cooking experience, wants simple 5-ingredient recipes
- **Power User - "Meal Prep Morgan":** 21yo junior, meal preps weekly, tracks spending
- **Casual User - "Dietary Dana":** 20yo sophomore, vegetarian, needs dietary filters

---

## PART 1: User Flow Diagrams

*Note: These can be actual diagrams OR clearly formatted text like below. Check your instructor's requirements for the exact number needed per persona.*

### PRIMARY USER (Busy Brian) - Example Flows

**Flow #1: Find a Quick Dinner Recipe**
- **Entry:** App Home Screen
- **Steps:** Tap "Search" → Filter "30 min or less" → Filter "5 ingredients" → Scroll results → Select "Easy Pasta Carbonara"
- **End State:** Viewing recipe details

**Flow #2: Set Cooking Timer**
- **Entry:** Viewing Recipe
- **Steps:** Scroll to cooking step → Tap "Set Timer" → Timer auto-sets to 10 min → Tap "Start"
- **End State:** Timer running

**Flow #3: Share Recipe with Roommate**
- **Entry:** Viewing Recipe
- **Steps:** Tap Share icon → Select "Text Message" → Select contact → Tap "Send"
- **End State:** Recipe link sent

### POWER USER (Meal Prep Morgan) - Example Flows

**Flow #4: Plan Entire Week's Meals**
- **Entry:** App Home Screen
- **Steps:** Tap "Meal Planner" → Tap "+ Add Meal" on Monday → Search "chicken" → Select "Lemon Herb Chicken" → Add to Monday → Repeat for rest of week
- **End State:** Week fully planned

**Flow #5: Generate Grocery List from Meal Plan**
- **Entry:** Meal Planner (with meals planned)
- **Steps:** Tap "Generate Grocery List" → Review compiled ingredients → Uncheck items in pantry → Review total cost → Tap "Send to Phone"
- **End State:** Shopping list ready

### CASUAL USER (Dietary Dana) - Example Flows

**Flow #6: Find Vegetarian Alternatives**
- **Entry:** Viewing "Classic Beef Tacos" recipe
- **Steps:** Notice beef ingredient → Tap "Suggest Substitutions" → Review alternatives → Select "Black beans" → Tap "Save Modified Recipe"
- **End State:** Vegetarian version saved

**Flow #7: Filter by Dietary Restrictions**
- **Entry:** App Home Screen
- **Steps:** Tap profile icon → Tap "Dietary Preferences" → Toggle ON "Vegetarian" → Toggle ON "Nut-free" → Tap "Save" → Return home
- **End State:** All searches now auto-filter

---

## PART 2: Five Lo-Fi Screen Mockups

### ⚠️ IMPORTANT: YOU MUST SUBMIT ACTUAL WIREFRAMES! ⚠️

### **DO NOT SUBMIT TEXT DESCRIPTIONS LIKE BELOW!**
### **SUBMIT ACTUAL DRAWINGS (PAPER OR DIGITAL)!**

**What we're showing below:** Example descriptions of what your wireframes should contain

**What YOU need to submit:** Actual sketches/wireframes - either:
- 📄 **Paper sketches** (take clear photos)
- 💻 **Digital wireframes** (Canva, Figma, PowerPoint, etc.) FigJam is an interesting option too https://www.figma.com/figjam/

**Time check:** Each screen shouldn't take long to create. If it's taking longer than 20 minutes to sketch a screen, consider a different tool or switch to paper!

**Remember:** Lo-fi = boxes, labels, and basic layout. NO colors, fancy fonts, or detailed graphics!

### Screen 1: Home Screen
*Used in Flows: #1, #7*

**What's on this screen:**
- App logo at top
- Search bar: "What do you want to cook?"
- Profile icon (top-right) → leads to settings
- Bottom nav tabs: Home 🏠 | Meal Planner 📅 | My Kitchen 🛒 | Favorites ⭐
- "Quick Dinners" featured category
- "Search by Ingredients" button

### Screen 2: Search Results
*Used in Flow: #1*

**What's on this screen:**
- Back arrow (top-left)
- Active filter chips: "30 min or less" "5 ingredients"
- Recipe cards showing:
  - Photo
  - Recipe name
  - Cook time
  - Ingredient count

### Screen 3: Recipe Detail View
*Used in Flows: #1, #6*

**What's on this screen:**
- Hero image
- Recipe name
- Share icon + Save button
- Tabs: Ingredients | Instructions | Nutrition
- "Suggest Substitutions" button
- Ingredient list with checkboxes
- Steps with timer buttons

### Screen 4: Meal Planner Calendar
*Used in Flow: #4*

**What's on this screen:**
- Week view: Mon-Sun
- Grid: 3 meals/day (Breakfast, Lunch, Dinner)
- Empty slots show "+ Add Meal"
- Filled slots show recipe thumbnail + name
- "Generate Grocery List" button at bottom

### Screen 5: Dietary Preferences
*Used in Flow: #7*

**What's on this screen:**
- Toggle switches for restrictions:
  - ☐ Vegetarian
  - ☐ Vegan
  - ☐ Gluten-free
  - ☐ Nut-free
- "Save Preferences" button
- Note: "All searches will respect these filters"

### Sample Wireframe hand drawn
Note this doesnt correspond with the actual example here (I found it on medium.com) but something of this fidelity would be fine handdrawn or done in a program. Make sure its legible so we can have our test users talk through how they would navigate things next class.

<img width="700" alt="wide4wireframeexample" src="https://github.com/user-attachments/assets/07896b19-8363-4145-ad69-b30935e277f5" />

---

## PART 3: Testing Script with 5 Tasks

**IMPORTANT:** You are creating **5 tasks total** (one per user flow you want to test). The numbered items under "Instructions for the user" are optional guidance steps to help your facilitator conduct the test - they are NOT additional tasks!

**Instructions:** Copy the [P3 Wireframe Feedback Script template](../documents/p3-wireframe-feedback-script.md) and fill in the sections below.

### Section I: Project Info
- **Project name:** MealMate
- **Section number:** [Your section]
- **Team number:** [Your team]
- **Facilitator Name:** [Team member 1]
- **Computer Name:** [Team member 2]
- **Scribe Name:** [Team member 3]

### Section II: User Info
- **First Name:** [To be filled during testing]
- **Age:** [To be filled during testing]

### Section III: Overall Impression (Pre-Task)
1. *Based on the home screen, what do you think this app is for?*
2. *On a scale of 1-5, how clear is the main purpose?*

### Section IV: Task-Specific Feedback

#### Task #1: Find a Quick Dinner Recipe
**Scenario:** "You're a busy college student with only 30 minutes to cook. Find something simple."

**What to do:**
1. Find recipes that take 30 minutes or less
2. Filter to show only 5 ingredients or fewer
3. Select the "Easy Pasta Carbonara" recipe
4. Save this recipe to your favorites
5. Review the ingredient list

**Follow-up questions:**
- *How easy was this task? (1-5)*
- *Did you understand each step? (Yes/No/Sometimes)*
- *Were any labels confusing?*
- *Did you get stuck anywhere?*
- *What did you expect when you tapped the Save button?*

#### Task #2: Plan Your Week's Meals (Power User)
**Scenario:** "You meal prep every Sunday and want to plan all dinners for the week."

**What to do:**
1. Navigate to the meal planning feature
2. Add a recipe to Monday's dinner
3. Add recipes for at least 2 more days
4. Review your weekly plan
5. Generate a shopping list from your planned meals

**Follow-up questions:**
- *How easy was this task? (1-5)*
- *Did you understand each step?*
- *Was it clear how to generate the shopping list?*
- *Did anything work differently than expected?*

### REPEAT FOR THE REST OF THE TASKS (so you have a total of 5)

**Remember:** Your 5 tasks should cover all three personas. For example:
- 2-3 tasks from primary user flows
- 1-2 tasks from power user flows  
- 1 task from casual user flows

---
