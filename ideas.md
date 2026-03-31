# Design Philosophy: Harry's Marylebone

## Selected Approach: **1950s Dolce Vita Noir**

### Design Movement
**Neo-Noir Maximalism** meets **Italian Dolce Vita** — a high-contrast, cinematic aesthetic that channels the glamour of 1950s Italian cinema through a contemporary dark-mode lens. Think Fellini's "La Dolce Vita" reimagined as a digital experience with surgical precision and dramatic lighting.

### Core Principles

1. **Dramatic Contrast as Storytelling**: Deep caviar blacks (#0A0A0A) serve as a canvas for vibrant, saturated product photography. The darkness isn't minimalist—it's theatrical, creating a gallery-like environment where food becomes art.

2. **Architectural Typography**: Linear Spractatus for headers creates sharp, geometric precision that contrasts beautifully with the organic, sensual product imagery. This tension between structure and indulgence defines the brand.

3. **Cinematic Motion**: Every animation tells a story. The "Dynamite Menu" intro isn't just decorative—it's a choreographed reveal that makes dining feel like entering an exclusive performance.

4. **Sensory Immersion**: The spotlight cursor, parallax scrolling, and floating cards create a tactile, almost 3D browsing experience. Users don't just view the menu—they *explore* it.

### Color Philosophy

- **Primary Palette**: Caviar (#0A0A0A) background with champagne gold accents (#D4AF37) for luxury signaling
- **Product Colors**: Hyper-saturated, high-gloss imagery
  - Vivid greens for pasta verde (emerald, not sage)
  - Deep crimsons for margherita (wine-red, not tomato-red)
  - Rich espresso browns for coffee (dark chocolate, not tan)
- **Accent Hierarchy**: Gold for primary CTAs, subtle silver/gray for secondary interactions
- **Emotional Intent**: Opulence meets sophistication. The dark background whispers exclusivity; the gold and vibrant product colors shout celebration.

### Layout Paradigm

**Asymmetric Cinematic Flow** — Reject centered grids. Instead:
- Hero section: Full-width cinematic video with overlaid animated menu (staggered, organic placement)
- Menu sections: Diagonal cuts and angled dividers between "Caffè," "Pranzo," "Dolci," and "Bar"
- Product showcase: Floating cards with glassmorphism, positioned at varying depths and angles
- Parallax zones: Text and images move at different speeds, creating layered depth
- Footer: Minimalist, anchored to bottom with address and org info in refined typography

### Signature Elements

1. **The Spotlight Cursor**: A glowing, interactive element that reveals texture details and food close-ups as users hover. Creates an intimate, exploratory feeling.

2. **Floating Cards with Glassmorphism**: Semi-transparent, frosted-glass effect cards that layer over the dark background. Each card has subtle shadows and blur, creating depth without clutter.

3. **3D Staggered Menu Intro ("Dynamite")**: Menu items (Coffee, Dessert, Pasta, Bar) fly in from different angles (top-left, bottom-right, center) with a slight 3D tilt, settling into a structured grid with a satisfying "snap" effect.

4. **Diagonal Dividers**: SVG-based angled cuts between sections, reinforcing the architectural, geometric aesthetic while maintaining visual flow.

### Interaction Philosophy

- **Purposeful Animation**: Every motion has intent. Hover states reveal details, scroll triggers parallax depth, and menu items "perform" on entry.
- **Tactile Feedback**: Glassmorphism cards respond to cursor proximity with subtle blur/scale changes. The spotlight cursor feels like a physical light source.
- **Exclusive Reveal**: Booking button is sticky, always accessible, but the overlay it triggers is a premium, dark-themed modal with refined typography and spacing.

### Animation Guidelines

1. **Menu Intro ("Dynamite")**: 
   - Duration: 1.2s total, staggered (100ms between items)
   - Easing: `cubic-bezier(0.34, 1.56, 0.64, 1)` (overshoot bounce)
   - Movement: 3D perspective, items rotate slightly (5-10deg) as they fly in
   - Settle: Snap into place with a subtle scale pulse (1.0 → 1.05 → 1.0)

2. **Parallax Scrolling**:
   - Product images move at 0.5x scroll speed
   - Text moves at 0.8x scroll speed
   - Creates layered depth without disorientation

3. **Spotlight Cursor**:
   - Smooth follow (50ms delay from actual cursor)
   - Reveals high-res texture overlays on hover
   - Glow effect (box-shadow with gold/white blend)

4. **Floating Cards**:
   - Entrance: Fade + scale (0.8 → 1.0) over 600ms
   - Hover: Scale (1.0 → 1.02) + blur increase (0.5px → 2px)
   - Exit: Fade + scale (1.0 → 0.9) over 400ms

5. **Scroll Triggers**:
   - Sections fade in as they enter viewport (0.3s ease-out)
   - Staggered child animations for list items

### Typography System

**Font Pairings**:
- **Headers (H1, H2)**: Linear Spractatus (geometric, sharp, architectural)
  - H1: 48px, weight 700, letter-spacing: 2px, all-caps for menu titles
  - H2: 32px, weight 600, letter-spacing: 1px
- **Body Text**: Inter or similar (clean, readable)
  - Body: 16px, weight 400, line-height: 1.6
  - Small: 14px, weight 400, line-height: 1.5
- **Accents**: Playfair Display or similar (elegant serif for descriptions)
  - Menu descriptions: 18px, weight 400, italic

**Hierarchy**:
- Primary: Linear Spractatus in gold or white
- Secondary: Inter in light gray
- Tertiary: Playfair Display in muted gold

---

## Rationale for Selection

This approach balances **luxury and accessibility**, **drama and sophistication**, and **motion and clarity**. It avoids generic dark-mode flatness by leveraging cinematic principles, architectural typography, and sensory interaction design. The result feels like a premium dining experience translated into digital form—exclusive, immersive, and unforgettable.
