# Plan: New Standalone Customer Experience Consulting Section

## Objective
Create a dedicated, standalone section between Services and Projects that expands the current brief CX service row into a robust section covering methodology, capabilities, and application of experience. The existing CX service row in the Services grid will be shortened to a concise summary with a link to the new section ("Learn more below").

## Rationale
The current Services grid constrains each item to ~3 sentences. CX is too broad and nuanced to compress that way. A standalone section allows:
- Room to articulate methodology (journey mapping, root-cause analysis, QA frameworks)
- Room to showcase contact centre expertise and government experience
- Room to explain the strategic side: VoC programs, metrics design, CX strategy
- Better visual hierarchy and balance on the page

## Proposed Content Structure

### Section Header
- Rule label: "Customer Experience"
- H2: "How I approach CX."

### 1. Opening Statement (philosophy)
Kept and adapted from current description — the core thesis that CX failures are systemic, not about people. This sets the tone.

### 2. Core Capabilities Grid (2-column layout)
A split layout similar to the Skills section, but with icons or visual indicators. Each column contains grouped capabilities.

**Column 1: Diagnosis & Design**
- Customer journey mapping and service blueprinting
- Root-cause analysis of recurring CX failures
- Quality assurance framework design
- Complaint analysis and systemic improvement

**Column 2: Operations & Strategy**
- Contact centre operations and process redesign
- Voice of Customer (VoC) program design
- CX metrics strategy — NPS, CSAT, CES and beyond
- Training, coaching and knowledge management alignment

### 3. "How I Apply It" paragraph
A narrative paragraph that connects the capabilities to real experience:

> *"I've developed and refined this approach across contact centres, government-contracted programmes, and compliance-heavy environments in New Zealand and Australia. That includes work delivered on behalf of the Australian Commonwealth Department of Health and Aged Care and New South Wales State Government electoral services. I know what works when compliance isn't optional, and I know how to balance operational efficiency with customer experience — because I've had to do both."*

### 4. Closing / CTA
A brief closing line that bridges to engaging Lucan's services:

> *"Whether it's a full CX strategy or a focused improvement in one area, I work directly with your team to make it happen — no lengthy change programmes, no unnecessary complexity."*

## Design Approach

### Layout
- Use the standard `.wrap` max-width for consistency
- Full-width opening statement
- 2-column capabilities grid (responsive → 1 column on mobile)
- Narrative paragraph below the grid
- Closing statement with subtle CTA

### Styling
- Light background (matching Services/Projects) — gives visual contrast with the dark About section that follows
- Use existing typography system (EB Garamond for headings, DM Sans for body)
- Rule label + H2 pattern consistent with other sections
- Capability items use the same treatment as skill-list items (copper dash bullet)

### Position
Insert the new section between the Services section (ends at line 360) and the Projects section (begins at line 363).

## Execution Steps

### Step 1: Write the new CX section content
Draft all copy for the section — opening statement, capability items, narrative paragraph, closing.

### Step 2: Add CSS styles
Add styles for:
- `.cx-grid` — the 2-column capabilities grid
- `.cx-col` — each column within the grid
- `.cx-col-title` — column sub-headings
- `.cx-list` — capability list items (reuse `.skill-list` styling)
- `.cx-narrative` — the "how I apply it" paragraph styling
- `.cx-closing` — closing paragraph / subtle CTA
- Responsive breakpoint for mobile (stack columns)

### Step 3: Add HTML structure
Insert the new `<section>` block between Services and Projects (between lines 360 and 362).

### Step 4: Update existing CX service row
Shorten the CX service row in the Services grid to a concise 2-sentence summary with a link to the new section:

> *"Most CX problems aren't really about the people — they're about how the work is set up. I specialise in journey mapping, quality assurance, VoC programs, and contact centre improvement. [Learn more below &darr;]"*

### Step 5: Update navigation
Add a "Customer Experience" link to both desktop nav and mobile menu, pointing to `#cx` (the new section ID).

### Step 6: Update Skills section
Review the CX & operations skills list — consider adding:
- "Customer journey mapping and service blueprinting"
- "CX metrics and VoC programs"
- "Root-cause analysis and complaint handling"

### Step 7: Review and test
- Verify responsive layout at mobile widths
- Check fade-in animation on new section
- Ensure nav link scrolls smoothly
- Confirm tone aligns with the rest of the site

## Tone Guidelines (same as existing site)
- Direct, plain English — not corporate or buzzword-heavy
- Show expertise through specific language, not self-praise
- Avoid em dashes
- Keep sentences concise
- Don't sound like AI-generated copy
