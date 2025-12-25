# Emma Partner Proposal Web Experience

An interactive web page that transforms from a star-lit question to a symbolic representation of partnership through constellation animations.

## Overview

This is a romantic partner proposal web experience featuring:
- Star-lit Pacific Northwest night sky
- Interactive constellation animations
- Progressive reveal of a heartfelt question
- Symbolic representation of partnership

## Technical Stack

- **HTML5** - Structure and Canvas/SVG
- **CSS3** - Styling and animations
- **Vanilla JavaScript** - Interactivity and animation logic
- No external dependencies for simplicity

## Project Phases

### Phase 1: Base Scene ✅ COMPLETE
- [x] Full-screen responsive layout
- [x] Deep blue-black gradient background (night sky)
- [x] SVG silhouettes of Pacific Northwest trees (Douglas fir, Western red cedar)
- [x] Trees frame an open center area for main content

### Phase 2: Star Field ✅ COMPLETE
- [x] 85 stars scattered across the center sky area (avoiding tree canopy)
- [x] Subtle twinkle animation using sine wave opacity pulse
- [x] Varying star sizes (0.8px - 2.5px) and colors (white/blue tones)
- [x] Smooth Canvas-based animation with requestAnimationFrame
- [x] Stars evenly distributed with gentle, non-jarring twinkle effect

### Phase 3: Text Formation ✅ COMPLETE
- [x] Calculated star positions to spell "Will you be my partner?"
- [x] Smooth animation from random positions to text formation
- [x] Ease-in-out cubic easing for natural movement
- [x] 2.5 second animation duration
- [x] Stars hold text formation when complete
- [x] Dot-matrix letter system (5x7 grid) for clear legibility
- [x] Responsive text sizing based on viewport
- [x] Two-line layout: "Will you" / "be my partner?"

### Phase 4: Interactive Buttons ✅ COMPLETE
- [x] Two ethereal buttons ("Yes" and "No") below the star-text
- [x] Constellation-themed aesthetic with glassmorphism effect
- [x] Smooth fade-in animation 1 second after text formation completes
- [x] Hover states with subtle glow effects
  - Yes button: soft blue glow on hover
  - No button: soft pink glow on hover
- [x] Active states with lift effect (translateY)
- [x] Both buttons trigger same transformation sequence
- [x] Backdrop blur and semi-transparent styling
- [x] Responsive sizing for mobile devices

### Phase 5: Constellation Transformation ✅ COMPLETE
- [x] Text dissolves when either button is clicked
- [x] Stars rearrange into two side-by-side constellation figures:
  - Orca whale (left) - 39 stars forming distinctive features
  - Stag with antlers (right) - 50 stars forming recognizable silhouette
- [x] Smooth 2-second transformation with ease-in-out cubic easing
- [x] Constellation patterns use normalized coordinates (0-1)
- [x] Responsive sizing (25% of viewport)
- [x] Figures clearly distinguishable and proportionally balanced
- [x] Stars hold final constellation positions
- [x] Symbolic meaning: Orca (ocean/strength) + Stag (forest/grace)

## How to View

Simply open `index.html` in a modern web browser:

```bash
# Using Python's built-in server
python3 -m http.server 8000

# Or simply open the file directly
open index.html
```

Then navigate to `http://localhost:8000` in your browser.

## File Structure

```
Emma/
├── index.html          # Main web experience (self-contained)
└── README.md          # Project documentation
```

## Development Notes

- All code is contained in a single HTML file for simplicity
- Uses vanilla JavaScript (no frameworks) for easy debugging
- SVG trees are hand-crafted to represent Pacific Northwest species
- Canvas for star rendering provides smooth 60fps animations
- Custom dot-matrix font system for text formation
- Constellation patterns defined with normalized coordinates for scalability
- Ease-in-out cubic easing for smooth, natural motion
- Glassmorphism effect for ethereal button styling
- Fully responsive design works on desktop, tablet, and mobile
- Star positions and text size adjust dynamically on window resize
- Animation triggers automatically 1 second after page load
- Interactive buttons appear 1 second after text formation
- Constellation transformation creates symbolic partnership representation

## Design Specifications

### Color Palette
- Night sky gradient: `#0a0e27` → `#1a1f3a` → `#2a2f4a` → `#1a1f35`
- Tree silhouettes: `#0a0d1a` (Douglas Fir), `#0d1020` (Cedar)
- Stars: 70% warm white (`rgb(255, 255, 240-255)`), 30% subtle blue (`rgb(220-255, 230-255, 255)`)
- Star opacity: Sine wave pulse between 0.5 and 1.0 for gentle twinkle

### Tree Species
- **Douglas Fir**: Triangular, layered branches creating classic conical shape
- **Western Red Cedar**: Irregular, drooping branch pattern characteristic of the species

### Animation Specifications
- **Text Formation Duration**: 2.5 seconds
- **Easing Function**: Ease-in-out cubic (smooth acceleration and deceleration)
- **Animation Trigger**: 1 second after page load
- **Text Content**: "Will you" (line 1), "be my partner?" (line 2)
- **Letter System**: Custom 5×7 dot-matrix font with 13 unique characters
- **Button Fade-In**: 1.5 second transition, 1 second after text completion

### Button Specifications
- **Style**: Glassmorphism with backdrop blur
- **Base Color**: `rgba(255, 255, 255, 0.08)` background
- **Border**: `1px solid rgba(255, 255, 255, 0.3)`
- **Hover Effects**:
  - Yes button: Light blue glow `rgba(173, 216, 230, 0.7)`
  - No button: Light pink glow `rgba(255, 192, 203, 0.5)`
  - Expanding radial gradient from center on hover
  - Subtle lift effect (translateY: -2px)
- **Typography**: Georgia serif, 18px (responsive)

### Constellation Specifications
- **Orca Whale (Left)**:
  - 39 stars total
  - Distinctive features: Dorsal fin, eye patch, tail flukes, pectoral fin
  - Positioned at 30% from left edge
  - Symbolizes: Strength, intelligence, connection to the ocean
- **Stag (Right)**:
  - 50 stars total
  - Distinctive features: Antlers, head/ears, body outline, four legs
  - Positioned at 70% from left edge
  - Symbolizes: Grace, nobility, connection to the forest
- **Transformation Duration**: 2.0 seconds
- **Size**: 25% of viewport (min dimension)
- **Coordinate System**: Normalized 0-1 for perfect scalability

## Future Enhancements

- Connecting lines between constellation stars (traditional constellation style)
- Unique celebration animations for different responses
- Additional constellation patterns (e.g., heart, infinity symbol)
- Particle effects or shooting stars
- Include sound design (optional)
- Add sharing capability (optional)
- Advanced mobile touch gestures
- Animation replay or reset functionality

## License

Personal project - All rights reserved
