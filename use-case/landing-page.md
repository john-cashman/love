---
title: "Landing Page"
description: "Welcome to the official guide to building landing pages in Lovable. "
icon: "file"
---

Learn how to go from idea to a fully functional, animated landing page, using AI \+ a sprinkle of razzle dazzle.

## Two Ways to Build Landing Pages

### 1. One-Shot Generation

Let Lovable do the heavy lifting. Just write a single prompt and let the AI generate your entire landing page.

**Prompt Example:**

```
You are a CRO expert. Build a landing page for a space tourism agency targeting wealthy individuals. The experience includes zero-gravity flights. Follow conversion rate optimization best practices. 
```

Add specific audience, features, or tone to help Lovable make better assumptions.

### 2. Section-by-Section

Prefer more control? Build one piece at a time: hero, pricing, FAQs, and more.

**Example flow:**

### Step 1
Generate a blank hero section

### Step 2
Click into any section with [visual edits](https://docs.lovable.dev/features/visual-edit) to:

    - Change text, colors, size
    - Move or delete elements
    - Tweak layout or animations

### Step 3
Add images, animations, pricing tables (details at the bottom)

### Step 4
Refactor styling \+ add branding \+ request a theme like:

    - Dark mode
    - Neo-brutalism
    - Glassmorphism
    - Futuristic fonts (e.g., _Space Grotesque_)

    
"Make the layout more elegant and smaller" can work wonders.

    **Case Study: Building HorseX Live**

    

    This page is based on our livestream where we built a space-themed landing page called **HorseX**—a space travel agency for horses (yes, seriously).

    - Space theme 🌌
    - Animations
    - Dark mode
    - Horse mascot (obviously)
    - Pricing & FAQs
    - Logo \+ favicon

### Step 5
Launch, Host, and Showcase

    - **Publish** with one click
    - **Connect to custom domain**
    - **Launch on Lovable Launch** (like Product Hunt but for Lovable)

    
Increase visibility by submitting to [Lovable Launch](https://docs.lovable.dev/features/launched)

## Layout Inspiration & Tools

Here are a few tools we used live:

- [**Mobbin**](https://mobbin.com) – Real-world design inspiration
- [**21st.dev**](http://21st.dev) – Copy-paste animation and design components
- [**Replicate Playground**](https://replicate.com/playgroundai) – AI image/logo generation
- [**Remove.bg**](http://Remove.bg) – Remove image backgrounds
- [**Icon Generator**](https://icons.pqoqubbw.dev/) – Free animated icons

## Advanced features

Level up your landing page with Lovable by adding rich interactive experiences, responsive UIs, and real working product previews.

  <details>
<summary>P5.js + Custom Animations</summary>
For visual magic like orbiting horses or flickering stars:

    - Use P5.js sketches in hero sections
    - Animate backgrounds (fix opacity \+ contrast for visibility)
    - Add particle effects or timeline scroll animations

    🛠 If it fails to render, use:

    - Chat mode for debugging
    - “Implement plan” from code block
    - Ask it to reset \+ use working reference code

    
Use Chat Mode to debug P5.js when things break.

</details>
  <details>
<summary>Customize Favicon</summary>
Favicons need to be 64x64 `.ico` or `.png`.

    **Steps:**

    1. Generate an icon on Replicate
    2. Resize via [favicon.io](http://favicon.io) or similar
    3. Paste image into prompt:

    ```
    Change the website favicon to this.
    ```
</details>
  <details>
<summary>Contact Forms that Actually Work</summary>
Collect emails and respond automatically with **Resend**.

    **Use case:**

    - Contact Sales form
    - Confirmation email to user
    - Notification email to your team

    **Prompt:**

    ```
    Implement a contact form that uses Resend.
    Send a confirmation email to the user and a notification to my team.
    ```

    
Need to limit usage or detect abuse? Add IP tracking with Supabase fingerprinting.

</details>
  <details>
<summary>What Type of Landing Page Should You Build?</summary>
Here’s what you can build:

    - Blog
    - Portfolio
    - SaaS site
    - Nonprofit
    - Course signup
    - Event promotion

    👉 Try building one of each to get comfortable.
</details>
  <details>
<summary>Conversion Rate Optimization (CRO) 101</summary>
Your landing page’s goal = 1 action.

    **That might be:**

    - Booking a call
    - Buying a seat (like HorseX)
    - Signing up for a waitlist

    **CRO best practices:**

    - Limit CTAs
    - Keep headlines clear
    - Match layout to audience expectations
    - Use social proof \+ trust signals

    Lovable understands the term “CRO optimized,” so use it in your prompts.
</details>
  <details>
<summary>Static vs Dynamic Pages</summary>
Lovable builds static pages by default.

    To make it dynamic:

    - Add forms (e.g., to collect leads)
    - Connect to Supabase
    - Add checkout using Stripe
    - CMS integration (e.g., with Strapi)
</details>
  <details>
<summary>Final Polish = Razzle Dazzle</summary>
Here’s what separates a $$2K site from a $$

    10K site:

    - Animations
    - Fonts \+ spacing
    - Branding consistency
    - Copywriting polish
    - Loading speeds
    - SEO setup (Lovable now supports robots.txt and OG tags)
</details>
  <details>
<summary>Add Real Product Previews</summary>
Let visitors **test your product directly** from the landing page. You can embed mini-apps using Supabase and external APIs like GROQ.

    **Example:** A “Make it professional” email previewer powered by the GROQ API:

    - Connect to Supabase first to avoid wiring issues later
    - Use `chat mode` to help Lovable understand and implement new APIs
    - Ask for fingerprinting or usage limits via IP if needed

    **Prompt:**

    ```
    Add a section where users can preview our AI email assistant.
    Connect to Supabase. Use GROQ API for email enhancement.
    ```
</details>
  <details>
<summary>Use 21st.dev for Beautiful Animations</summary>
Enhance your visual design with high-quality animations and components:

    - Floating glowing particles
    - Scroll-based sticky sections
    - Timeline animations
    - Logo carousels
    - Modal popups for video demos

    
If animations don't show up, use chat mode to debug or re-implement from scratch. You can also upload screenshots and say:\
      _“Please animate this background section.”_

</details>
  <details>
<summary>Add Modal Popups (Videos & More)</summary>
Want to show a demo without cluttering the hero?

    **Use modals:**

    - Embed YouTube or demo videos
    - Trigger on button click (e.g. “Watch Demo”)
    - Common prompt term: `modal popup`

    **Prompt:**

    ```
    When the “Watch Demo” button is clicked, open a modal popup with this video.
    ```
</details>
  <details>
<summary>Add a Trust Section with Real Logos</summary>
Social proof matters.

    - Create a “Trusted By” section with animated company logos.
    - Ensure logos stay as image files, not SVG paths.
    - Avoid grayed-out overlays.

    **Prompt:**

    ```
    Add a “Trusted by” section using real company logos.
    Keep them as images, not SVGs. Use 21st.dev animations.
    ```
</details>
  <details>
<summary>Hero Animations & UI Polish</summary>
Don’t settle for static hero sections:

    - Animate words (cycle between phrases)
    - Add floating shapes (circles, gradients)
    - Match color palette across hero, headings, and timeline

    Example prompts:

    ```
    Animate the word in the hero title to cycle between "intelligence" and "assistance"
    Add floating purple circles in the background
    Make the heading text use the primary purple gradient
    ```
</details>
  <details>
<summary>Sticky Navigation + Custom Navbar</summary>
Want smooth scrolling to sections?

    - Use a sticky nav bar
    - Replace default nav with one from [21st.dev](http://21st.dev)
    - Make sure it links to **sections**, not new pages

    
Use screenshots and say: _“Make this navbar scroll to page sections and match our theme.”_

</details>
  <details>
<summary>Mobile Responsiveness</summary>
Lovable auto-generates mobile-friendly pages—but test and tweak:

    - Add margin and padding via visual edit
    - Test modals, animations, and layouts on mobile
</details>
  <details>
<summary>What’s the Parallax Effect?</summary>
**Parallax** creates a sense of **depth** by having background elements move at a different speed than foreground ones as you scroll. It’s like walking through a forest in a video game — trees in the front move faster than mountains in the back.

    **Why it’s cool:**

    - Adds immersion
    - Makes your landing page feel more dynamic and interactive
    - Visually separates sections in a subtle way

    **Prompt Example:**

    ```
    Add a parallax scroll effect to the background of the hero section.
    Make the stars move slower than the text and images.
    ```

    
Use it sparingly. Too much parallax = overwhelming.

</details>
  <details>
<summary>What’s Isometry (Isometric Design)?</summary>
**Isometric design** creates a 3D-like effect using 2D graphics, typically at a 30° angle. Think of games like _Monument Valley_ or old-school _Sim City_. Everything looks “tilted” but perfectly aligned — no perspective distortion.

    **Why use it:**

    - Clean, futuristic aesthetic
    - Makes your app visuals look more sophisticated
    - Great for tech, data, and AI themes

    **Prompt Example:**

    ```
    Use isometric illustrations for the product feature section.
    Make the graphics look like a futuristic dashboard in 3D.
    ```

    You can also import isometric illustrations from:

    - [Storyset](https://storyset.com)
    - [Icons8 Isometric](https://icons8.com/icons/set/isometric)
    - [3D Icons Library](https://www.3dicons.com/)

    
Isometric graphics pair really well with **glassmorphism** or dark-themed UIs for modern SaaS pages.

</details>

## Other tutorials