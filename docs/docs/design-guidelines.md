## Aircraft Vault – Design Guidelines

### ✈️ Emotional Thesis
Feels like a secure hangar vault—clean, technical, and quietly confident. Every detail respects aviation-level precision, trust, and minimalism.

---

### 🔤 Typography System

| Role       | Font               | Weight | Size | Notes                                    |
|------------|--------------------|--------|------|------------------------------------------|
| H1         | Inter Tight        | 600    | 32px | Condensed, sharp, evokes cockpit labels  |
| H2–H4      | IBM Plex Sans      | 500    | 24/20/18px | Neutral, structured, highly legible |
| Body       | IBM Plex Sans      | 400    | 16px | Minimum 1.5× line-height                 |
| Caption    | IBM Plex Mono      | 400    | 13px | For file info, timestamps, tech labels   |

All type should follow a vertical rhythm (4px or 8px increments) and maintain ≥ AA+ contrast.

---

### 🎨 Color System

```md
#1F2937 → Primary (Charcoal) – Trustworthy, aviation core
#4B91F1 → Accent (Cool Blue) – Confident actions
#F9FAFB → Background – Clean, soft neutral
#10B981 → Success
#FBBF24 → Warning
#EF4444 → Danger

Maintain ≥ 4.5:1 contrast


Avoid saturated reds except for critical alerts


Light/dark mode optional, but defaults to bright cockpit clarity



📐 Spacing & Layout
Grid: 8pt base unit


Folder grid: 3-column desktop → 1-column mobile


Card padding: 16px internal, 24px gutter


Top bar: Persistent with “My Vault” + Upload CTA


Sticky mobile action bar: Upload + New Folder


Use layout rhythm to express reliability and avoid visual clutter.

🎞️ Motion & Interaction
Event
Behavior
Hover (folder)
Thin border highlight or soft glow
Drag over folder
Folder icon pulses subtly
Upload complete
Fade-in + checkmark animation (200ms)
Modal transitions
Slide up softly, ease-in-out (200ms)


Easing: ease-in-out


Duration: 150–250ms (no bouncy motion)


Motion toggle for accessibility



🗣 Voice & Tone
Tone: Technical, competent, quietly friendly


Personality: Helpful co-pilot, never chatty


Microcopy Examples
✅ Onboarding: “Your documents, under control.”


🔗 Share flow: “Generate a share link to grant read-only access.”


📁 Folder: “Folder created. Ready when you are.”


⚠️ Error: “Something went off-course. Try again or upload manually.”



♿ Accessibility
Semantic structure (folders = list; files = list items)


Full keyboard nav for vault browsing


Visible focus states


ARIA roles on all file/folder elements


Motion toggle in settings


High-contrast labels always on by default



🔁 System Consistency
File cards: Same padding, preview size, and action buttons


Folders: Uniform naming, ordering, and icons


Top bar: Persistent on all views


Empty states: Encouraging, not pushy


Style system references:
shadcn/ui → For component structure


Linear → For layout clarity


Apple Human Interface → For system polish



🧭 Design Snapshot Output
🎨 Color Palette
#1F2937 – Charcoal (Primary)
#4B91F1 – Cool Blue (Accent)
#F9FAFB – Background
#10B981 – Success
#FBBF24 – Warning
#EF4444 – Danger

🔤 Typographic Scale
Type
Font
Size
Line Height
Weight
H1
Inter Tight
32px
40px
600
H2
IBM Plex Sans
24px
32px
500
H3
IBM Plex Sans
20px
28px
500
Body
IBM Plex Sans
16px
24px
400
Cap
IBM Plex Mono
13px
18px
400

📏 Spacing Summary
8pt vertical grid


24px card gutters


Sticky bottom bar (mobile)


16px internal padding on components


💬 Emotional Thesis (1-line)
Feels like a secure hangar vault—minimal, structured, and quietly confident.

✅ Design Integrity Review
The visual system embodies the aviation-grade clarity and trust we aimed for. Typography is focused and readable, colors communicate safety and control, and interactions are calm, not flashy. To deepen emotional connection, consider testing a soft dark mode with cockpit-blue accents for low-light environments.
