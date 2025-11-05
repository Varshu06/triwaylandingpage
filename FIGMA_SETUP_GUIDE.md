# Figma Setup Guide for Triway Technologies Landing Page

This guide will help you recreate the Triway Technologies landing page design in Figma.

## 📋 Prerequisites

1. Figma account (free or paid)
2. Access to Figma desktop app or web version
3. Fonts: Poppins and Space Grotesk (available on Google Fonts)

## 🎨 Step-by-Step Setup

### 1. Create a New Figma File

1. Open Figma
2. Click "New Design File"
3. Name it "Triway Technologies Landing Page"

### 2. Set Up Color Styles

Go to **Design → Styles → Colors** and create these color styles:

#### Primary Colors
- **Triway Blue**: `#4A90E2`
- **Triway Orange**: `#FF6B35`
- **Triway Green**: `#61A60E`

#### Background Colors
- **Dark BG**: `#0A0E27`
- **Dark Surface**: `#151B3D`

#### Text Colors
- **Text Primary**: `#FFFFFF`
- **Text Secondary**: `#B8C5D1`
- **Text Muted**: `#7A8FA3`

#### Gradients
- **Primary Gradient**: Linear 135° from `#4A90E2` to `#FF6B35`
- **Text Gradient**: Linear 135° from `#4A90E2` → `#FF6B35` → `#61A60E`
- **Stats Gradient**: Linear 135° from `#4A90E2` to `#61A60E`

### 3. Set Up Typography Styles

Go to **Design → Styles → Text** and create:

#### Headings
- **H1**: Poppins, 800, 48px (clamp: 40-72px), Line height 1.1
- **H2**: Poppins, 800, 36px (clamp: 32-56px), Line height 1.2
- **H3**: Poppins, 700, 24px, Line height 1.3

#### Body Text
- **Body Large**: Poppins, 400, 20px, Line height 1.8
- **Body**: Poppins, 400, 16px, Line height 1.6
- **Small**: Poppins, 500, 14px, Line height 1.5

#### Logo Text
- **Logo**: Space Grotesk, 700, 18px, Letter spacing 2px, Uppercase

### 4. Create Components

#### A. Triway Logo Component

1. Create a Frame (40px × 40px)
2. Add three triangles:
   - **Triangle 1 (Blue)**: 
     - Position: Center
     - Size: 24px width × 40px height
     - Color: `#4A90E2`
     - Rotation: 0°
   - **Triangle 2 (Orange)**:
     - Same size, Color: `#FF6B35`
     - Rotation: 120°
   - **Triangle 3 (Green)**:
     - Same size, Color: `#61A60E`
     - Rotation: 240°
3. Make it a Component: Right-click → "Create Component"
4. Name it "Logo - Triway Triangles"

#### B. Button Components

**Primary Button**:
- Frame: Auto width, Height: 56px
- Background: Primary Gradient
- Border radius: 50px
- Padding: 16px 40px
- Text: Body style, 600 weight, White color
- Shadow: 0px 4px 20px rgba(74, 144, 226, 0.3)

**Secondary Button**:
- Frame: Auto width, Height: 56px
- Background: Transparent
- Border: 2px solid rgba(255, 255, 255, 0.2)
- Border radius: 50px
- Padding: 16px 40px
- Text: Body style, 600 weight, White color

#### C. Card Components

**Value Card**:
- Frame: 280px × Auto (min-height: 300px)
- Background: `rgba(21, 27, 61, 0.6)`
- Border: 1px solid `rgba(255, 255, 255, 0.1)`
- Border radius: 24px
- Padding: 40px
- Top border: 4px solid (color variant)

**Solution Card**:
- Frame: 280px × Auto (min-height: 400px)
- Same as Value Card
- Large number in corner (opacity: 5%)

### 5. Create Page Sections

#### Section 1: Navigation Bar
- Frame: 1440px × 80px
- Background: `rgba(10, 14, 39, 0.95)` with backdrop blur
- Layout: Horizontal, Space between
- Left: Logo + Text
- Right: Navigation links + CTA button
- Position: Fixed at top

#### Section 2: Hero Section
- Frame: 1440px × 100vh (min 900px)
- Background: Dark BG with grid pattern overlay
- Layout: Split 50/50 (Grid)

**Left Side**:
- Badge: Green background, rounded
- Heading: H1 with gradient text
- Description: Body Large
- Two CTA buttons
- Stats: 3 columns

**Right Side**:
- Floating cards (3 cards positioned absolutely)
- Center: Large logo (200px)

#### Section 3: Value Propositions
- Frame: 1440px × Auto
- Background: Dark Surface
- Padding: 100px vertical
- Grid: 4 columns (responsive)

#### Section 4: Solutions
- Frame: 1440px × Auto
- Background: Dark BG
- Padding: 100px vertical
- Grid: 4 columns (responsive)

#### Section 5: Why Choose Us
- Frame: 1440px × Auto
- Background: Dark Surface
- Padding: 100px vertical
- Layout: Split 50/50

#### Section 6: CTA Section
- Frame: 1440px × Auto
- Background: Dark BG
- Padding: 100px vertical
- Layout: Split 50/50
- Right: Contact form

#### Section 7: Footer
- Frame: 1440px × Auto
- Background: Dark Surface
- Padding: 60px top, 20px bottom
- Grid: 4 columns

### 6. Add Effects and Details

#### Background Patterns
- Grid pattern: 50px × 50px, opacity 3%
- Radial gradients for depth

#### Shadows
- Cards: `0 8px 32px rgba(0, 0, 0, 0.16)`
- Buttons: `0 4px 20px rgba(74, 144, 226, 0.3)`

#### Blur Effects
- Navigation: Backdrop blur 20px
- Floating cards: Backdrop blur 20px

### 7. Responsive Breakpoints

Create variants for:
- **Desktop**: 1440px (default)
- **Tablet**: 968px
- **Mobile**: 768px
- **Small Mobile**: 480px

### 8. Export Assets

When ready to export:
1. Select frames/components
2. Right-click → "Export"
3. Formats: PNG, SVG (for logos)
4. Sizes: 1x, 2x, 3x

## 🔧 Quick Tips

1. **Use Auto Layout**: For buttons, cards, and navigation items
2. **Create Variants**: For button states (default, hover, active)
3. **Use Constraints**: For responsive behavior
4. **Component Library**: Make reusable components
5. **Styles**: Use color and text styles for consistency

## 📐 Key Measurements

- **Container Max Width**: 1400px
- **Section Padding**: 100px vertical
- **Card Gap**: 32px (2rem)
- **Border Radius**: 24px (cards), 50px (buttons)
- **Icon Size**: 70px (cards), 40px (features)

## 🎯 Design Tokens Reference

See `design-specification.json` for complete design system details.

## 📝 Next Steps

1. Create the frame structure
2. Add color and text styles
3. Build components
4. Assemble sections
5. Test responsive breakpoints
6. Add interactions (if using Figma Prototyping)

---

**Note**: For animations and interactions, use Figma's Prototyping features or note them in the design spec for developers.

