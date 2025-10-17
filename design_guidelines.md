# Design Guidelines: Romantic Birthday Website for Diyasha

## Design Approach
**Reference-Based Approach**: Drawing inspiration from romantic, celestial-themed experiences with luxury e-commerce aesthetics. The design should evoke the emotional depth of premium storytelling platforms while maintaining the intimate, personal nature of a love letter.

## Core Design Principles
1. **Cosmic Romance**: Every element should feel like it's floating in a dreamy, starlit universe
2. **Royal Elegance**: Luxurious yet intimate, like a handwritten letter sealed with gold
3. **Emotional Depth**: Design should amplify the heartfelt nature of the content
4. **Celestial Motion**: Gentle, continuous animations that never feel overwhelming

## Color Palette

### Primary Colors
- **Rose Pink**: 340 85% 75% - Primary romantic accent, used for key headings and hearts
- **Royal Gold**: 45 90% 65% - Accent for special elements, borders, and shimmer effects
- **Midnight Blue**: 240 45% 15% - Deep background base
- **Lavender**: 270 60% 80% - Soft highlights and glow effects

### Gradients
- Background: Radial gradient from midnight blue to deep purple (260 50% 20%)
- Text glows: Soft lavender to rose pink transitions
- Overlays: Semi-transparent rose pink (340 85% 75% / 0.1) for depth layers

## Typography

### Font Families
- **Primary Headings**: 'Great Vibes' or 'Dancing Script' (elegant handwritten cursive) via Google Fonts
- **Body Text**: 'Cormorant Garamond' or 'Playfair Display' (refined serif for readability)
- **Countdown/Timer**: 'Cinzel' (regal, display font)

### Type Scale
- Hero Title: text-6xl md:text-7xl lg:text-8xl (80-96px)
- Page Titles: text-4xl md:text-5xl (48-60px)
- Section Headers: text-3xl md:text-4xl (36-48px)
- Body Text: text-lg md:text-xl (18-20px) with increased line-height (1.8)
- Timer Numbers: text-5xl md:text-6xl (60-72px)

## Layout System

### Spacing Units
Use Tailwind spacing: **4, 8, 12, 16, 20, 24, 32** for consistent rhythm
- Section padding: py-20 md:py-32
- Content spacing: space-y-8 md:space-y-12
- Element margins: mb-8, mt-12, gap-6

### Container Strategy
- Full viewport sections for immersive experience
- Max-width prose (65ch) for letter content readability
- Centered layouts: mx-auto, text-center
- Mobile: px-6, Tablet/Desktop: px-8 md:px-12

## Page-Specific Layouts

### 1. Home Page
- Full viewport hero (min-h-screen) with centered content
- Countdown timer prominently placed center-screen
- Floating navigation at top with glass-morphism effect (backdrop-blur-md)
- Background: Animated cosmic gradient with twinkling star particles

### 2. Letter from Saru
- Parchment-style content area with soft glow border
- Single column layout (max-w-3xl) for intimate reading experience
- Generous vertical spacing between paragraphs (space-y-6)
- Floating heart animations rising from bottom corners

### 3. Sorry Page (Apology Room)
- Softer, calmer variation of cosmic theme
- Text blocks with gentle fade-in animations on scroll
- Centered poetic verses with ample breathing room
- Subtle star pulse effects in background

### 4. Birthday Surprise Page
- Explosive reveal with confetti animation
- Large celebratory message center-screen
- Multiple layers of floating elements (hearts, stars, sparkles)
- Gradient text effects on main message

## Component Library

### Navigation
- Fixed top bar with glass-morphism (bg-midnight-blue/30, backdrop-blur-lg)
- Links: Home | Letter | Sorry | Surprise
- Active state: Rose pink glow effect
- Mobile: Hamburger menu with slide-in panel

### Countdown Timer
- Grid layout: 4 columns (Days | Hours | Minutes | Seconds)
- Each unit in bordered card with glow effect
- Large numbers in Cinzel font with royal gold color
- Labels below in smaller cursive font
- Target: October 18, 2025 00:00:00 IST

### Text Content Cards
- Semi-transparent backgrounds (bg-white/5)
- Soft borders with rose pink glow (border border-rose-pink/30)
- Generous padding (p-8 md:p-12)
- Rounded corners (rounded-2xl)

### Interactive Elements
- Buttons (if needed): Outlined style with glass effect, rose pink border, hover glow
- Links: Underline on hover with smooth transition

## Animations & Effects

### Background Animations
- Twinkling stars: Random opacity pulses (1s-3s duration)
- Floating particles: Gentle vertical drift with slight horizontal sway
- Gradient shift: Slow color rotation (30s loop)

### Content Animations
- Page transitions: Fade with 0.5s duration
- Text reveals: Fade-in from bottom with stagger effect
- Hearts floating: Rise from bottom with rotation, fade out at top
- Sparkles: Random position appearance/disappearance

### Glow Effects
- Text shadows: Multiple layered shadows in rose pink and lavender
- Box glows: Soft outer glow on cards and containers
- Pulse animations: Subtle scale and opacity changes on special elements

## Accessibility & Responsiveness

### Dark Mode
- Primary dark theme only (no light mode needed for this romantic atmosphere)
- Ensure text contrast ratios meet WCAG standards against dark backgrounds
- Glowing text remains readable

### Responsive Breakpoints
- Mobile (base): Single column, reduced animations for performance
- Tablet (md: 768px): Introduce more spacing, full animations
- Desktop (lg: 1024px): Maximum visual impact, all effects active

### Performance
- Limit particle count on mobile (50 vs 200 on desktop)
- Use CSS transforms for animations (GPU accelerated)
- Lazy load heavy effects below fold

## Special Features

### Countdown Logic
- Calculate time difference to October 18, 2025 00:00:00 IST
- Update every second with smooth number transitions
- Auto-redirect or unlock Surprise page when countdown reaches zero

### Page Transitions
- Fade out current page (300ms)
- Fade in new page (300ms)
- Total transition: 600ms smooth easing

### Surprise Reveal
- Triggered automatically when countdown ends
- Confetti burst from center outward
- Message reveals with scale-up animation
- Continuous celebration animations (hearts, stars raining)

## Images
**No images required** - This is a purely text and animation-based design to maintain the ethereal, cosmic atmosphere without distractions. All visual interest comes from gradients, particle effects, and typography.

---

**Final Note**: Every element should feel weightless, as if floating in a cosmic love story. The design must be deployment-ready for Replit/Vercel/Netlify with a shareable direct link. Prioritize emotional impact and romantic atmosphere over complexity.