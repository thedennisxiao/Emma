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
- Ease-in-out cubic easing for smooth, natural motion
- Fully responsive design works on desktop, tablet, and mobile
- Star positions and text size adjust dynamically on window resize
- Animation triggers automatically 1 second after page load

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

## Future Enhancements

- Add interactive response mechanism (Yes/No buttons)
- Constellation formation animation on acceptance
- Celebration animation or visual effect
- Include sound design (optional)
- Add sharing capability (optional)
- Mobile touch interactions

## License

Personal project - All rights reserved
