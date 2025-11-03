# P3 Deliverable #2 Example: MealMate Recipe App

**NOTE TO STUDENTS:** This is a complete example showing what your team needs to submit by the start of next class. Use this as a template to create your own deliverable for YOUR app!

---

## What You're Submitting

Your team needs to submit THREE things:

1. **9 User Flow Diagrams** (5 for primary user, 2 for power user, 2 for casual user)
2. **5+ Lo-Fi Screen Mockups** (paper sketches or digital wireframes)
3. **Testing Script with 5 Tasks** (using the provided template)

---

## Example App: MealMate

**High Concept:** A recipe discovery and meal planning app for college students

**Core Features:** Recipe search, grocery lists, meal planner, recipe saving, timers, ingredient substitutions, budget tracking

**Three Personas:**
- **Primary User - "Busy Brian":** 19yo freshman, limited cooking experience, wants simple 5-ingredient recipes
- **Power User - "Meal Prep Morgan":** 21yo junior, meal preps weekly, tracks spending
- **Casual User - "Dietary Dana":** 20yo sophomore, vegetarian, needs dietary filters

---

## PART 1: Nine User Flow Diagrams

*Note: These can be actual diagrams OR clearly formatted text like below*

### PRIMARY USER (Busy Brian) - 5 Flows

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

**Flow #4: Check What's In My Pantry**
- **Entry:** App Home Screen
- **Steps:** Tap "My Kitchen" → Tap "Pantry" → View list → Tap "+ Add Item" → Type "spaghetti" → Save
- **End State:** Item added to pantry

**Flow #5: Find Recipes Using My Ingredients**
- **Entry:** App Home Screen
- **Steps:** Tap "Search by Ingredients" → Select "spaghetti" from pantry → Select "garlic" → Tap "Find Recipes"
- **End State:** Viewing filtered results

### POWER USER (Meal Prep Morgan) - 2 Flows

**Flow #6: Plan Entire Week's Meals**
- **Entry:** App Home Screen
- **Steps:** Tap "Meal Planner" → Tap "+ Add Meal" on Monday → Search "chicken" → Select "Lemon Herb Chicken" → Add to Monday → Repeat for rest of week
- **End State:** Week fully planned

**Flow #7: Generate Grocery List from Meal Plan**
- **Entry:** Meal Planner (with meals planned)
- **Steps:** Tap "Generate Grocery List" → Review compiled ingredients → Uncheck items in pantry → Review total cost → Tap "Send to Phone"
- **End State:** Shopping list ready

### CASUAL USER (Dietary Dana) - 2 Flows

**Flow #8: Find Vegetarian Alternatives**
- **Entry:** Viewing "Classic Beef Tacos" recipe
- **Steps:** Notice beef ingredient → Tap "Suggest Substitutions" → Review alternatives → Select "Black beans" → Tap "Save Modified Recipe"
- **End State:** Vegetarian version saved

**Flow #9: Filter by Dietary Restrictions**
- **Entry:** App Home Screen
- **Steps:** Tap profile icon → Tap "Dietary Preferences" → Toggle ON "Vegetarian" → Toggle ON "Nut-free" → Tap "Save" → Return home
- **End State:** All searches now auto-filter

---

## PART 2: Five Lo-Fi Screen Mockups

**IMPORTANT:** These descriptions show what should be IN your wireframes. You'll actually create paper sketches or digital wireframes (Canva/Figma). I'm describing them here for demonstration purposes only.

### Screen 1: Home Screen
*Used in Flows: #1, #4, #5, #9*

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
*Used in Flows: #1, #8*

**What's on this screen:**
- Hero image
- Recipe name
- Share icon + Save button
- Tabs: Ingredients | Instructions | Nutrition
- "Suggest Substitutions" button
- Ingredient list with checkboxes
- Steps with timer buttons

### Screen 4: My Kitchen / Pantry
*Used in Flow: #4*

**What's on this screen:**
- Tabs: Pantry | Fridge | Shopping List
- "+ Add Item" button (top-right)
- Grouped ingredient list:
  - Grains (spaghetti, rice)
  - Canned Goods
  - Spices
- "Find Recipes with These" button at bottom

### Screen 5: Meal Planner Calendar
*Used in Flow: #6*

**What's on this screen:**
- Week view: Mon-Sun
- Grid: 3 meals/day (Breakfast, Lunch, Dinner)
- Empty slots show "+ Add Meal"
- Filled slots show recipe thumbnail + name
- "Generate Grocery List" button at bottom

### Optional Screen 6: Dietary Preferences
*Used in Flow: #9*

**What's on this screen:**
- Toggle switches for restrictions:
  - ☐ Vegetarian
  - ☐ Vegan
  - ☐ Gluten-free
  - ☐ Nut-free
- "Save Preferences" button
- Note: "All searches will respect these filters"

### Optional Screen 7: Substitution Modal
*Used in Flow: #8*

**What's on this screen:**
- "Suggested Substitutions for Beef" header
- List of alternatives:
  - ⭐⭐⭐ Black beans
  - ⭐⭐⭐ Plant-based crumbles
  - ⭐⭐ Mushrooms
- Each has "Use This" button
- "Cancel" button at bottom

---

## PART 3: Testing Script with 5 Tasks

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

#### Task #2: Check Your Pantry Inventory
**Scenario:** "You want to track ingredients you have at home."

**What to do:**
1. Navigate to where you view pantry items
2. Add "spaghetti" to your pantry
3. Add "garlic" to your pantry
4. Review your complete list
5. Find where you'd search recipes using these ingredients

**Follow-up questions:**
- *How easy was this task? (1-5)*
- *Did you understand each step?*
- *Were any buttons hard to find?*
- *Did anything work differently than expected?*

#### Task #3: Plan Your Week's Meals
**Scenario:** "You meal prep on Sundays and want to plan all week's dinners."

**What to do:**
1. Navigate to the meal planning calendar
2. Add a dinner recipe to Monday
3. Add dinner recipes to 3 more days
4. Review your complete week
5. Find where you'd generate a grocery list

**Follow-up questions:**
- *How easy was this task? (1-5)*
- *Was the calendar view clear?*
- *Could you see your whole plan at once?*
- *Was adding meals intuitive?*

#### Task #4: Find Vegetarian Alternatives
**Scenario:** "You found a recipe with meat, but you're vegetarian."

*[Start them on the "Classic Beef Tacos" recipe screen]*

**What to do:**
1. Find the feature that suggests vegetarian substitutions
2. Review the alternatives offered
3. Select "Black beans" as your replacement
4. Verify the recipe updated
5. Save the modified version

**Follow-up questions:**
- *How easy was this task? (1-5)*
- *Was the Substitutions button noticeable?*
- *Were the alternatives helpful?*
- *Did you notice the recipe changed?*

#### Task #5: Set Dietary Filters
**Scenario:** "You're vegetarian and your roommate has a nut allergy. Set up filters for all searches."

**What to do:**
1. Navigate to dietary preferences/settings
2. Turn ON the "Vegetarian" filter
3. Turn ON the "Nut-free" filter
4. Save your preferences
5. Confirm future searches will use these filters

**Follow-up questions:**
- *How easy was this task? (1-5)*
- *Was the settings icon easy to find?*
- *Were the toggle switches clear?*
- *Did you understand this affects all searches?*

### Section V: Final Summary (Post-Task)
1. *What did you like MOST about the app's structure?*
2. *What did you like LEAST?*
3. *Any other suggestions?*
4. *MAGIC WAND: "If you could add one feature to make cooking easier for college students, what would it be?"*

---

## What to Submit to myCourses

**By start of next class:**

1. ✅ **Document with 9 user flows** (formatted like Part 1 above, or as diagrams)
2. ✅ **5+ screen mockups** (photos of paper sketches OR digital wireframes from Canva/Figma)
3. ✅ **Completed testing script** (using the template, filled out like Part 3 above)

**Submission notes:**
- Only ONE team member submits (team dropbox)
- If mockups are paper, take clear photos
- If mockups are digital, include link or export as images
- Testing script can be Word doc, Google Doc, or PDF

---

## Tips for Success

**Choose flows strategically** - Pick ones showing your best features across all 3 personas

**Reuse screens** - One screen (like Home) can support multiple flows

**Write clear tasks** - Use scenario language ("You want to...") for context

**Keep wireframes simple** - Boxes and labels, not fancy designs (save that for hi-fi!)

**Test yourselves first** - Have a teammate try your tasks before class

---

## Common Mistakes to Avoid

Creating 9 separate mockups for 9 flows (you only need 5-7 screens total!)

Making mockups too detailed (this is LO-fi, not hi-fi)

Writing vague tasks ("Use the app" vs. "Find a recipe under 30 minutes")

Forgetting to test all 3 personas (make sure at least one task covers each)

Not bringing materials to class for iteration (bring paper/markers to update screens!)

---

**Next Class (11B):** You'll test your prototypes with classmates using these scripts. Be ready to take notes on what works and what needs fixing before you build the hi-fi version!
