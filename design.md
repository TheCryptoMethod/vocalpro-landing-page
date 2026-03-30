```markdown
# VocalPro Landing Page Design System

This document outlines the core design principles and specifications for the VocalPro premium landing page. It aims to provide a consistent and modern aesthetic, targeting craftsmen and healthcare professionals with a professional and engaging user experience.

---

## 1. Color Palette

A dark color scheme with professional blues and a vibrant accent for calls to action.

*   **Background (Deep Indigo):** `#1A1A2E`
*   **Primary (Modern Blue):** `#4A90E2`
*   **Secondary (Cool Gray):** `#8D99AE`
*   **Accent (Vibrant Gold):** `#FFD700`
*   **Text - Light (Off-white):** `#E0E0E0`
*   **Text - Muted (Medium Gray):** `#A0A0A0`
*   **Success/Positive:** `#28A745`
*   **Error/Warning:** `#DC3545`

---

## 2. Typography

Clean, modern sans-serif fonts for optimal readability and a professional feel.

*   **Headings Font:** `Inter` (Google Font)
    *   **Weights:** 700 (Bold), 600 (Semi-Bold)
*   **Body Font:** `Roboto` (Google Font)
    *   **Weights:** 400 (Regular), 500 (Medium)

### Font Sizes (Responsive)

| Element       | Desktop (>=1024px) | Tablet (768px - 1023px) | Mobile (<=767px) | Line Height |
| :------------ | :----------------- | :---------------------- | :--------------- | :---------- |
| **H1**        | 64px (Bold)        | 48px (Bold)             | 36px (Bold)      | 1.2         |
| **H2**        | 48px (Bold)        | 36px (Bold)             | 28px (Bold)      | 1.25        |
| **H3**        | 36px (Semi-Bold)   | 28px (Semi-Bold)        | 24px (Semi-Bold) | 1.3         |
| **H4**        | 28px (Semi-Bold)   | 24px (Semi-Bold)        | 20px (Semi-Bold) | 1.35        |
| **Body Large**| 20px (Regular)     | 18px (Regular)          | 16px (Regular)   | 1.6         |
| **Body Regular**| 18px (Regular)   | 16px (Regular)          | 15px (Regular)   | 1.6         |
| **Body Small**| 16px (Regular)     | 15px (Regular)          | 14px (Regular)   | 1.6         |
| **Caption**   | 14px (Regular)     | 13px (Regular)          | 12px (Regular)   | 1.5         |
| **Button Text**| 18px (Semi-Bold)  | 16px (Semi-Bold)        | 15px (Semi-Bold) | 1           |

---

## 3. Spacing Scale

A consistent 4px base grid for all spacing, ensuring harmony and alignment.

*   **xs:** 4px
*   **sm:** 8px
*   **md:** 16px
*   **lg:** 32px
*   **xl:** 64px
*   **xxl:** 96px
*   **xxxl:** 128px

---

## 4. Border Radius

Subtle rounding for a modern, friendly touch without sacrificing professionalism.

*   **Small:** 4px (e.g., input fields, small buttons)
*   **Medium:** 8px (e.g., cards, larger buttons)
*   **Large:** 12px (e.g., prominent containers, modals)
*   **Full:** 50% (e.g., avatars, circular elements)

---

## 5. Shadow Styles

Elevated elements with subtle, dark shadows to create depth on the dark background.

*   **Subtle Shadow:** `0px 4px 10px rgba(0, 0, 0, 0.2)`
    *   *Use for:* Buttons, small cards, interactive elements.
*   **Medium Shadow:** `0px 8px 20px rgba(0, 0, 0, 0.3)`
    *   *Use for:* Feature cards, pricing plans, testimonials.
*   **Strong Shadow:** `0px 12px 30px rgba(0, 0, 0, 0.4)`
    *   *Use for:* Modals, sticky headers, highly prominent elements.
*   **Inner Shadow:** `inset 0px 2px 4px rgba(0, 0, 0, 0.1)`
    *   *Use for:* Input fields (on focus/active states).

---

## 6. Component Specifications by Section

### 6.1. Hero Section

*   **Layout:** Full-width, vertically and horizontally centered content.
*   **Background:** Dynamic visual (e.g., subtle AI-themed animation, abstract waveform graphic) or high-quality image with a dark overlay (`rgba(26, 26, 46, 0.7)`).
*   **Elements:**
    *   **Headline (H1):** Catchy, benefit-driven. Text color: `Text - Light`.
    *   **Sub-headline (H3):** Elaborates on the headline, reinforces value. Text color: `Text - Muted`.
    *   **Primary CTA Button:** Prominent, uses `Accent` color for background, `Background` color for text. `Border Radius: Medium`. `Shadow: Subtle Shadow`.
        *   *Hover:* Slight scale up (1.05), background darken, `Shadow: Medium Shadow`.
    *   **Secondary CTA Button (Optional):** Outline style, `Primary` color for border and text. Transparent background. `Border Radius: Medium`.
        *   *Hover:* Background `Primary` color (10% opacity), text `Text - Light`.
*   **Spacing:** `padding-top/bottom: xxl` on desktop, `xl` on tablet, `lg` on mobile.

### 6.2. Features Section

*   **Layout:** Grid-based. 3 columns on desktop, 2 columns on tablet, 1 column on mobile.
*   **Elements:**
    *   **Section Title (H2):** Centered. Text color: `Text - Light`.
    *   **Feature Card:**
        *   **Background:** `Background` color, slightly lighter variant or `rgba(26, 26, 46, 0.8)` for contrast.
        *   **Border Radius:** `Medium`.
        *   **Shadow:** `Medium Shadow`.
        *   **Icon/Illustration:** Prominent, uses `Primary` or `Accent` color.
        *   **Feature Title (H3):** Text color: `Text - Light`.
        *   **Description (Body Regular):** Text color: `Text - Muted`.
*   **Spacing:** `gap: lg` between cards. `padding-top/bottom: xxl` on desktop, `xl` on tablet, `lg` on mobile.

### 6.3. Pricing Section

*   **Layout:** Grid-based. 3 columns on desktop, 1 column on tablet/mobile.
*   **Elements:**
    *   **Section Title (H2):** Centered. Text color: `Text - Light`.
    *   **Pricing Card:**
        *   **Background:** `Background` color. Highlighted plan (e.g., "Pro") uses `rgba(74, 144, 226, 0.1)` for background with a `Primary` color border.
        *   **Border Radius:** `Large`.
        *   **Shadow:** `Medium Shadow`.
        *   **Plan Name (H3):** Text color: `Text - Light`.
        *   **Price (H1/H2):** Large, bold. Text color: `Accent` for the main number, `Text - Muted` for currency/period.
        *   **Feature List (Body Regular):** Bullet points or checkmarks. Text color: `Text - Light`. Checkmark icon uses `Success/Positive`.
        *   **CTA Button:** `Primary` color background, `Text - Light` text. Highlighted plan uses `Accent` color background. `Border Radius: Medium`.
            *   *Hover:* Same as Hero CTA.
*   **Spacing:** `gap: lg` between cards. `padding-top/bottom: xxl` on desktop, `xl` on tablet, `lg` on mobile.

### 6.4. Testimonials Section

*   **Layout:** Carousel or 2-column grid on desktop, 1 column on tablet/mobile.
*   **Elements:**
    *   **Section Title (H2):** Centered. Text color: `Text - Light`.
    *   **Testimonial Card:**
        *   **Background:** `Background` color, slightly lighter variant or `rgba(26, 26, 46, 0.8)`.
        *   **Border Radius:** `Medium`.
        *   **Shadow:** `Subtle Shadow`.
        *   **Quote (Body Large):** Italicized. Text color: `Text - Light`.
        *   **Author Name (H4):** Text color: `Primary`.
        *   **Title/Company (Body Small):** Text color: `Text - Muted`.
        *   **Avatar/Image (Optional):** Circular, `Border Radius: Full`.
*   **Spacing:** `gap: lg` between cards. `padding-top/bottom: xxl` on desktop, `xl` on tablet, `lg` on mobile.

### 6.5. FAQ Section

*   **Layout:** Accordion style.
*   **Elements:**
    *   **Section Title (H2):** Centered. Text color: `Text - Light`.
    *   **FAQ Item (Accordion):**
        *   **Question (H3):** Text color: `Text - Light`. Background `Background` color.
            *   *Hover:* Slight background change (`rgba(26, 26, 46, 0.8)`).
        *   **Answer (Body Regular):** Text color: `Text - Muted`. Background `Background` color, slightly lighter.
        *   **Toggle Icon:** Plus/Minus icon, uses `Primary` color.
*   **Spacing:** `margin-bottom: md` between FAQ items. `padding-top/bottom: xxl` on desktop, `xl` on tablet, `lg` on mobile.

### 6.6. Contact Section

*   **Layout:** Form on one side, optional contact info/illustration on the other (desktop). Stacked on tablet/mobile.
*   **Elements:**
    *   **Section Title (H2):** Centered or left-aligned. Text color: `Text - Light`.
    *   **Form:**
        *   **Background:** `Background` color, slightly lighter. `Border Radius: Large`. `Shadow: Medium Shadow`.
        *   **Input Fields (Text, Email, Textarea):**
            *   **Background:** `rgba(0, 0, 0, 0.2)` or `Background` color (darker shade).
            *   **Border:** 1px solid `Secondary` color.
            *   **Border Radius:** `Small`.
            *   **Text Color:** `Text - Light`. Placeholder color: `Text - Muted`.
            *   **Focus State:** `Border` color changes to `Primary`, `Inner Shadow`.
        *   **Submit Button:** `Accent` color background, `Background` color text. `Border Radius: Medium`.
            *   *Hover:* Same as Hero CTA.
    *   **Contact Info (Optional):** Icons (e.g., email, phone) using `Primary` color, text using `Text - Light`.
*   **Spacing:** `padding-top/bottom: xxl` on desktop, `xl` on tablet, `lg` on mobile.

### 6.7. Footer Section

*   **Layout:** Multi-column (e.g., logo, navigation links, social media, copyright).
*   **Background:** `Background` color (or slightly darker, e.g., `#101020`).
*   **Elements:**
    *   **Logo:** White or `Text - Light` version.
    *   **Navigation Links (Body Regular):** Text color: `Text - Muted`.
        *   *Hover:* Text color: `Primary`.
    *   **Social Media Icons:** `Text - Muted` color.
        *   *Hover:* Color: `Primary`.
    *   **Copyright Text (Caption):** Text color: `Text - Muted`.
*   **Spacing:** `padding-top/bottom: xl` on desktop, `lg` on tablet, `md` on mobile.

---

## 7. Responsive Breakpoints

Standard breakpoints for a mobile-first approach.

*   **Mobile:** `max-width: 767px`
*   **Tablet:** `min-width: 768px` and `max-width: 1023px`
*   **Desktop:** `min-width: 1024px`

---

## 8. Animation Guidelines

Animations should be subtle, professional, and enhance the user experience without being distracting.

*   **Overall Principle:** Smooth, purposeful, and performant.
*   **Duration:**
    *   Fast interactions (e.g., button hovers): `0.2s`
    *   Standard transitions (e.g., card lifts, accordion toggles): `0.3s`
    *   Slower, more deliberate animations (e.g., section fade-ins): `0.4s - 0.6s`
*   **Easing:**
    *   Most common: `ease-in-out` or `cubic-bezier(0.4, 0, 0.2, 1)` for smooth acceleration and deceleration.
    *   For quick snaps: `ease-out` or `cubic-bezier(0, 0, 0.2, 1)`.
*   **Specific Examples:**
    *   **Hover Effects:** Buttons, links, cards should have subtle `transform: translateY(-2px)` (lift) or `box-shadow` changes, accompanied by `color` or `background-color` transitions.
    *   **Scroll Reveal:** Sections or key elements can `fade-in` or `slide-up` slightly as they enter the viewport.
    *   **Accordion:** Smooth `height` transition for expanding/collapsing content.
    *   **Form Focus:** Input fields should smoothly transition their `border-color` and potentially apply an `inner shadow` on focus.
    *   **CTA Buttons:** Slight `scale(1.02)` on hover, combined with background color change.
*   **Avoid:** Bouncy, overly complex, or jarring animations. Ensure animations are disabled or simplified for users with reduced motion preferences.
```