# Figma Prototyping Teaching Guide

## Overview
- **What's Covered:** Creating interactive Figma prototypes with vertical/horizontal scrolling, page navigation, and modal overlays
- **Estimated Time:** 45-60 minutes for demonstration and practice
- **Prerequisites:** Basic Figma familiarity (creating frames, shapes, and text)
- **Setup Needed:** Figma account, mobile device with Figma app (optional but recommended)

---

## Step-by-Step Guide

### STEP 1: Create a New Prototype File
**Action:** Set up the initial workspace and mobile frame

1. Create new Figma "Design" file
2. Name it "Prototype Practice"
3. Press `F` to create a frame
4. Select mobile phone frame size (iPhone or Android based on your device)

**Key Point:** Choosing the right frame size from the start ensures accurate mobile preview
**Common Issues:** Using desktop frame sizes by mistake - always match your target device

---

### STEP 2: Build Basic Wireframe Header
**Action:** Create the app header with contrast and text

1. Press `R` to create a rectangle at the top
2. Change fill color to dark gray for contrast
3. Press `T` to add text box
4. Type "Header" as placeholder text
5. Adjust font and position

**Code Example (Design Properties):**
```
Rectangle:
- Fill: #333333 (dark gray)
- Height: ~60px

Text:
- Font: Medium/Semibold
- Size: 18-20px
- Color: White
- Alignment: Center
```

**Key Point:** Dark backgrounds with light text create clear visual hierarchy
**Common Issues:** Forgetting to change text color to white on dark backgrounds

---

### STEP 3: Create Bottom Tab Bar
**Action:** Build navigation footer with icon placeholders

1. Copy header rectangle (`Cmd/Ctrl + C`)
2. Paste (`Cmd/Ctrl + V`)
3. Move to bottom of screen
4. Press `R` multiple times to create 3 rectangles as icon placeholders
5. Space them evenly across the tab bar

**Key Point:** Tab bars are fixed navigation - users expect them to stay visible while scrolling
**Common Issues:** Making tab bar too tall (should be ~60-80px)

---

### STEP 4: Add Content Cards
**Action:** Create scrollable content area

1. Press `R` to create a card rectangle
2. Position between header and footer
3. Copy and paste (`Cmd/Ctrl + C/V`) to create 3 cards
4. Space them vertically

**Key Point:** Leave space between cards for visual breathing room
**Common Issues:** Cards touching edges - add ~16-20px margins

---

### STEP 5: Generate Prototype Link
**Action:** Create shareable interactive preview

1. Click **"Prototype"** tab in top right
2. Set device to your mobile phone type
3. Select the entire frame
4. Click **play icon** (▶️) in top right
5. Click **"Share Prototype"** button

**Result:** You now have a shareable URL that others can view and interact with

**Key Point:** Anyone with the link can view your prototype without a Figma account
**Common Issues:** Forgetting to set correct device type - preview won't match actual size

---

## Code Checkpoint - Basic Wireframe Complete

At this point you should have:
- Mobile frame with header (dark gray, centered text)
- Three content cards in the middle
- Bottom tab bar with 3 icon placeholders
- A working prototype link (not yet interactive)

---

### STEP 6: Enable Page-Level Vertical Scroll
**Action:** Make the entire page scrollable while keeping header/footer fixed

1. **Zoom out** and select the frame
2. **Extend frame length** by dragging bottom edge down
3. Select the toolbar and **drag to new bottom**
4. Copy one card and **paste multiple times** to fill screen
5. Adjust frame length so it's completely filled

**Result:** Page now scrolls vertically

**WARNING:** Header and footer currently scroll with content - we'll fix this next

**Key Point:** Frame height must be taller than device viewport for scrolling to work

---

### STEP 7: Fix Header to Top (Sticky Positioning)
**Action:** Make header stay visible during scroll

1. Select **all header elements** (rectangle + text)
2. Hold `Ctrl` to ensure you're selecting everything
3. Right-click → **"Group Selection"** (or `Cmd/Ctrl + G`)
4. In right panel under **Constraint**
5. Keep top constraint active
6. Check **"Fixed position when scrolling"** box

**Code Example (Properties):**
```
Header Group:
- Constraint: Top
- Fixed position: ✓ Checked
```

**Result:** Header now stays at top while content scrolls beneath it

**Common Issues:** Forgetting to group elements first - fixed position won't work on ungrouped items

---

### STEP 8: Fix Footer to Bottom (Sticky Positioning)
**Action:** Make tab bar stay visible during scroll

1. Select **all footer elements** (rectangle + icons)
2. Right-click → **"Group Selection"** (or `Cmd/Ctrl + G`)
3. In right panel under **Constraint**
4. Click **bottom line** to change constraint to bottom
5. Check **"Fixed position when scrolling"** box

**Code Example (Properties):**
```
Footer Group:
- Constraint: Bottom (not top!)
- Fixed position: ✓ Checked
```

**Result:** Footer now stays at bottom while content scrolls

**Key Point:** Must change constraint to "Bottom" for footer - different from header!

---

## Scrolling Checkpoint

**Test your prototype now:**
- Page should scroll vertically
- Header stays fixed at top
- Footer stays fixed at bottom
- Content scrolls between them

---

### STEP 9: Prepare for Horizontal Scroll Component
**Action:** Create horizontally scrollable card section

1. Go back to design file
2. Select **first card** and make it narrower (~60-70% of frame width)
3. Copy and paste to create multiple cards **side by side**
4. Select **all upper cards**
5. Drag them **out of the main frame** temporarily

**Key Point:** We're building a contained horizontal scroll area separate from the vertical page scroll
**Common Issues:** Trying to make cards scroll horizontally while still in the main frame - won't work

---

### STEP 10: Frame the Horizontal Scroll Section
**Action:** Create a container that enables horizontal scrolling

1. With cards selected, right-click → **"Frame Selection"**
2. This creates a new frame around just these cards
3. **Drag this new frame back** into the mobile frame
4. Position it where you want the horizontal scroll area

**Result:** Cards are now in their own frame that we can control

**Key Point:** Frames within frames enable different scroll behaviors
**Common Issues:** Not creating the frame before trying to add scroll - horizontal scroll needs a frame

---

### STEP 11: Configure Horizontal Scrolling
**Action:** Set frame properties for horizontal scroll

1. Select the **cards frame** (not individual cards)
2. Adjust **frame width** to match phone width (so cards overflow)
3. In right panel, check **"Clip content"** box
4. In **Prototype tab**, enable **"Horizontal scrolling"**

**Code Example (Properties):**
```
Cards Frame:
- Width: ~90% of phone width
- Clip content: ✓ Checked
- Prototype: Horizontal scrolling ✓ Enabled
- Vertical scrolling: Disabled
```

**Result:** Users can now swipe horizontally through cards

**Key Point:** Frame width MUST be smaller than total cards width for scroll to activate
**Common Issues:** Frame too wide - no overflow means no scroll needed

---

## Component Scrolling Checkpoint

**Test your prototype now:**
- Page scrolls vertically (header/footer fixed)
- Upper card section scrolls horizontally
- You can adjust frame size without squishing cards

---

### STEP 12: Create a Second Page
**Action:** Build a new screen for navigation testing

1. Double-click page frame name → rename to **"Page 1"**
2. Copy **entire Page 1** frame (`Cmd/Ctrl + C`)
3. Paste beside it (`Cmd/Ctrl + V`)
4. Rename new frame to **"Page 2"**
5. Keep header and footer
6. Adjust/create new rectangles to make it visually different

**Key Point:** Navigation requires at least 2 distinct pages
**Common Issues:** Not making pages visually different enough - users won't notice navigation working

---

### STEP 13: Create Navigation Interaction (Method 1)
**Action:** Link tab bar icon to different page

1. Make sure **Prototype tab** is selected (top right)
2. Select **one icon** on Page 1's tab bar
3. **Drag the blue circle** (connection point) to Page 2
4. Release to create the connection

**Result:** Clicking that icon now navigates to Page 2

**Code Example (Interaction Details):**
```
Icon → Page 2:
- On: Click/Tap
- Action: Navigate to Page 2
- Animation: Instant (default)
```

**Key Point:** The blue circle appears when you hover over interactive elements
**Common Issues:** Accidentally dragging the element instead of the connection point

---

### STEP 14: Create Return Navigation
**Action:** Link back from Page 2 to Page 1

1. On **Page 2**, select **different icon** on tab bar
2. Drag blue circle to **Page 1**

**Result:** Users can now click between pages using tab icons

**Key Point:** Complete navigation requires links in both directions
**Common Issues:** Linking same icon on both pages - users expect consistent icon meanings

---

### STEP 15: Create Navigation Interaction (Method 2)
**Action:** Alternative way to create navigation

1. Select icon on Page 2
2. In **Prototype panel**, click **"+ Add Interaction"**
3. Click the new interaction
4. Change **"None"** dropdown to **"Navigate to"**
5. Select **"Page 1"** from destination dropdown

**Code Example (Properties):**
```
Interaction:
- Trigger: On Click
- Action: Navigate to → Page 1
- Animation: Instant
```

**Result:** Exact same navigation as Method 1, just created differently

**Key Point:** Method 2 is better for complex interactions with multiple triggers
**Common Issues:** Forgetting to change "None" to "Navigate to"

---

## Navigation Checkpoint

**Test your prototype now:**
- Click tab icons to move between Page 1 and Page 2
- Navigation should feel instant and responsive
- Icons should clearly indicate which page you're on (if designed well)

---

### STEP 16: Create Modal/Overlay Frame
**Action:** Build a popup dialog

1. Press `F` to create new frame
2. Make it **smaller than mobile screen** (~70-80% width)
3. Position it **near your pages** (doesn't need to be on them)
4. Use rectangles to create a modal design:
   - Background rectangle
   - Close icon in top right
   - Content area

**Key Point:** Modals should be smaller than full screen to show they're overlays
**Common Issues:** Making modal full-screen - loses the overlay effect

---

### STEP 17: Create Overlay Interaction
**Action:** Make icon trigger the modal popup

1. Go to **Page 2**
2. Select **one of the icons** (we'll use as modal trigger)
3. In **Prototype tab**, drag blue circle to **modal frame**
4. In interaction details, change **"Navigate to"** to **"Open overlay"**

**Code Example (Properties):**
```
Interaction:
- Trigger: On Click
- Action: Open overlay → Modal Frame
- Animation: Instant
```

**Result:** Clicking the icon opens modal as an overlay

**WARNING:** Without next steps, modal will be hard to see and can't be closed

---

### STEP 18: Improve Overlay Visibility
**Action:** Add background dimming and click-outside-to-close

1. With the interaction still selected
2. Under **interaction details**, check:
   - ✓ **"Add background behind overlay"**
   - ✓ **"Close when clicking outside"**

**Code Example (Properties):**
```
Overlay Settings:
- Background behind overlay: ✓ Checked
- Close when clicking outside: ✓ Checked
```

**Result:** Modal now has dimmed background and can be dismissed by clicking outside

**Key Point:** These two settings make modals feel polished and user-friendly
**Common Issues:** Forgetting background - modal blends into page content

---

### STEP 19: Add Close Button to Modal
**Action:** Create explicit way to dismiss modal

1. Select the **close icon** in top right of modal
2. In **Prototype tab**, click **"+ Add interaction"**
3. Set interaction to **"Close overlay"**

**Code Example (Properties):**
```
Close Icon Interaction:
- Trigger: On Click
- Action: Close overlay
- Icon: X or cross symbol
```

**Result:** Users can now close modal by clicking X or clicking outside

**Key Point:** Always provide two ways to close modals (explicit close button + outside click)
**Common Issues:** Close icon not actually clickable - verify interaction is added

---

## Modal Checkpoint

**Test your prototype now:**
- Click designated icon to open modal
- Modal appears with dimmed background
- Click outside modal to close
- Click X icon to close
- Modal properly overlays page content

---

## Bonus Tips

### TIP 1: Test on Real Device
**Action:** Use Figma mobile app for realistic testing

1. Download **Figma app** on your mobile phone
2. Open the app and log in
3. Click **"Mirror"** icon in bottom right
4. Select any frame on your laptop

**Result:** Prototype appears on your phone in real-time

**Key Point:** This is THE best way to test mobile interactions - more realistic than desktop preview
**Common Issues:** Laptop and phone need to be on same WiFi network

---

### TIP 2: Use Components for Shared Elements
**Action:** Make tab bar edits update across all pages automatically

1. **Drag tab bar** outside of any page frames
2. Right-click → **"Create Component"**
3. Add **all interactions** to this main component (all icon links)
4. **Copy this main component**
5. **Paste into each page** (automatically becomes instance)

**Code Example (Component Structure):**
```
Main Component (outside frames):
- All interactions defined once
- Icon 1 → Page 1
- Icon 2 → Page 2
- Icon 3 → Page 3

Instances (on each page):
- Automatically inherit all interactions
- Updates when main component changes
```

**Result:** Edit tab bar once, all pages update automatically

**Key Point:** HUGE time saver when you have many pages or need to make changes
**Common Issues:** Editing instance instead of main component - changes don't propagate

---

### TIP 3: Shadow User Testing
**Action:** Watch real-time as someone uses your prototype

1. Open **prototype link** (the share URL)
2. Send this link to a test user
3. Once they start using it, click **their profile photo** in top right
4. Select **"Shadow"** option

**Result:** You see exactly what they're doing in real-time

**Key Point:** Perfect for remote user testing and observing interaction patterns
**Common Issues:** Tester must use the share link, not view the design file

---

## Summary

### Core Skills Mastered:
1. **Page-Level Vertical Scroll** with fixed header/footer
2. **Component-Level Horizontal Scroll** within a frame
3. **Cross-Page Navigation** using interactive elements
4. **Modal Overlays** with proper visibility and dismissal

### Key Figma Concepts:
- Fixed positioning for sticky elements
- Frames within frames enable different scroll behaviors
- Components save massive time on repeated elements
- Prototype mode vs Design mode serve different purposes

### Common Troubleshooting:
| Problem | Solution |
|---------|----------|
| Page won't scroll | Frame height must exceed viewport height |
| Header/footer scrolls with content | Group elements, enable "Fixed position" |
| Horizontal scroll not working | Check: Clip content ✓, Frame width < cards width |
| Navigation doesn't work | Verify blue connection line exists in Prototype tab |
| Modal hard to see | Add background behind overlay |
| Can't close modal | Add "Close overlay" interaction to X icon |

### What You Can Do Now:
- Create multi-page interactive prototypes
- Implement realistic scrolling behaviors
- Add navigation between screens
- Build modal dialogs and overlays
- Test designs on real devices
- Use components to work efficiently

---


**Bonus:** Share your prototype link and get feedback from classmates!

---

*This guide based on comprehensive Figma prototyping tutorial covering essential interactive features for mobile app design.*
