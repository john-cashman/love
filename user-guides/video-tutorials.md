---
title: Video tutorial
description: >-
  Check out these videos to get a full overview of how to build an app with
  Lovable.
icon: video
---

# Video Tutorials

### Welcome to Lovable

<details>

<summary>Lovable 101</summary>

#### Getting started with Lovable basics

#### Understanding the interface and controls

#### Working with editing features and version history

#### Implementing authentication and user management

#### Using ‪Supabase‬ databases and edge functions

#### GitHub integration and code management

#### Sharing projects and community feedback

#### Exploring additional resources and templates

</details>

### Lovable Tutorials

<details>

<summary>Build an AI-Powered Calorie Tracking WebApp</summary>

```
This tutorial, we'll walk you through creating an AI-powered calorie tracking app with [Lovable](/lovable-f9060f1e/lovable-f9060f1e/editor/main.md#build-an-ai-powered-calorie-tracking-webapp), complete with authentication, a beautiful responsive design, OpenAI integration, and deployment to production.

```

#### Setting Up the Foundation

The foundation of any Lovable project is a good prompt. For this app, here’s an example:

````
    ```
    Create a calorie tracking app with the following features:
    Landing page, dashboard, and a meals page.
    Input fields for meal descriptions or images, with analysis powered by GPT-4.
    Daily progress tracking and integration with Supabase for authentication and database management.
    Beautiful and mobile-responsive UI.
    ```

    Once Lovable generates the UI skeleton:

    - Review the navigation setup and landing page design.
    - Iterate on the prompt to refine the layout and ensure mobile responsiveness.

    
````

#### Designing the UI

Lovable emphasizes a step-by-step approach, akin to constructing a building:

```
    - Start with **scaffolding**: Plan your app structure (e.g., user experience flow, page layout).
    - Add the **first layer**: Create empty pages with basic design elements.
    - Refine the **details**: Add colors, animations, and mobile responsiveness.

    
```

#### Integrate Supabase for Backend and Authentication

Once the UI is ready, it’s time to add backend functionality:

```
    1. Set up a [**Supabase**]() **account** and create a project.
    2. Link it to Lovable by pressing the "Connect Supabase" button.
    3. For data storage, Lovable will generate SQL tables. For instance:

    - A `profiles` table to store user information.
    - A `meals` table linked to users for tracking daily entries.

    
```

#### Integrating OpenAI for Meal Analysis

The magic of this app lies in its AI capabilities. To analyze meals:

```
    1. Obtain an [OpenAI API key]() from your developer dashboard.
    2. Use [GPT-4]() for analyzing meal descriptions or images.
    3. Ensure API keys are securely stored in Edge functions to prevent unauthorized access.

    **Features to include:**

    - **Analyze meal descriptions**: Estimate nutritional values (calories, protein, carbs, fat).
    - **Image recognition**: Upload a meal photo, and GPT-4 will extract a description and nutritional data.

    
```

#### Implementing Payments with Stripe

To monetize the app, add subscription-based payments:

```
    1. Create a [Stripe]() account and set up a product (e.g., “Standard Plan” for $12/month).
    2. Integrate Stripe with Lovable by adding the API key and product price ID.
    3. Redirect non-paying users to the landing page. Only paying users can access the main app.

    
```

#### Testing and Debugging

Errors are a natural part of development, and Lovable simplifies debugging:

```
    - Use the **"Try to Fix"** button whenever a build error occurs.
    - For backend issues, check Supabase logs for detailed error reports.
    - If deploying to [Netlify](), review deployment logs for any build issues. Share logs with Lovable to get tailored fixes.

    
```

#### Deploying Your App

Once your app is ready, deploy it with Lovable or Netlify:

```
    1. Use Lovable’s deploy feature to host the app on a default domain.
    2. For custom domains:

    - Connect your [GitHub repository]() to Netlify.
    - Purchase a domain and configure [DNS settings]() to link it to Netlify.

    
```

</details>

<details>

<summary>Build a SaaS Landing Page with Groq API</summary>

```
In this tutorial, we’ll show you how to create a stunning, fully interactive landing page for an AI-powered email assistant using [Lovable](/lovable-f9060f1e/lovable-f9060f1e/editor/main.md#build-a-saas-landing-page-with-groq-api), 21st.dev, and Supabase—complete with animations, API integrations, and seamless deployment\\\\\!

- AI-powered design & UI enhancements
- Adding animations & interactive elements
- Integrating AI email enhancements with the Groq API
- Setting up a contact form with Resend
- Deploying the page using Lovable Launch
```

</details>

<details>

<summary>Build a Feedback Tool</summary>

The session showcased \[Lovable]\(/lovable-f9060f1e/lovable-f9060f1e/editor/main.md#build-a-feedback-tool)’s capabilities to iterate quickly and deliver production-ready results.

#### Authentication

* Users can sign up, log in, and manage profiles using Supabase integration.\
  \- Secure user sessions enable tailored experiences.

#### Feedback Submission and Voting

* Users can submit feedback with titles, descriptions, and images.\
  \- Each feedback entry displays vote counts and supports real-time upvoting.

#### Admin Dashboard with AI Summaries

* Admins can review all feedback, filter by votes, and sort entries.\
  \- AI-powered summaries identify actionable insights using OpenAI and Supabase Edge Functions.

#### User Presence Tracking

Real-time presence indicators show active users on the platform.

#### Detailed Feedback Pages with Comments

Each feedback entry has a dedicated page for discussions, enabling teams to collaborate and prioritize efficiently.

#### File Attachments

Users can attach images to feedback, stored securely using Supabase’s storage capabilities.

</details>

<details>

<summary>Build a Productized Development Agency</summary>

```
The goal for this session was to build an app that allows developers, designers, or consultants to offer subscription-based services—a business model inspired by platforms like DesignJoy.

```

#### Authentication and User Management

Authentication was the first feature implemented, setting up a robust framework for managing users. The team emphasized the importance of integrating authentication early to prevent issues when scaling the app.

```
    - Supabase integration for user sign-ups, logins, and profile management.
    - Persistent user sessions to improve app usability.
```

#### Stripe Subscription Integration

The session demonstrated how to integrate Stripe for subscription management:

```
    - Enabled users to subscribe to different pricing tiers.
    - Managed subscription status, ensuring only paid users access premium features.
```

#### Dashboard and Task Management

* User-specific dashboards with task boards and drag-and-drop functionality.\
  \- Real-time task updates for seamless collaboration.

#### AI Chatbot

The session concluded with the integration of an AI chatbot, illustrating how OpenAI can add dynamic functionality to apps. This feature could be extended to serve as a virtual assistant, concierge, or data query interface.

```
    - Integrated OpenAI to provide a chatbot capable of responding intelligently to user queries.
    - Built in a single prompt, showcasing Lovable's efficiency.
```

#### Iterative Debugging and Refinement

The team tackled real-time debugging challenges, offering valuable insights into troubleshooting. Techniques included:

```
    - Using console logs and error messages to identify issues.
    - Reverting to previous app versions to avoid getting stuck in broken states.
    - Guiding Lovable’s AI with detailed prompts to ensure accurate fixes.
```

</details>

<details>

<summary>Prompting Advice with Lovable</summary>

```
In this tutorial, we deep-dive into AI-powered app development, prompt engineering, and workflow automation with [Lovable](https://lovable.dev/)'s special guest ‪[Mark Kashef‬](https://www.youtube.com/@Mark_Kashef)\!

- Understanding effective AI prompting
- The four tiers of prompt engineering
- Meta prompting techniques & best practices
- Debugging strategies for AI workflows
- Building an AI app using Lovable & Make.com
- Integrating Visual Edits & Tailwind CSS for UI design
```

</details>

<details>

<summary>Build a Luma Copycat with Supabase &#x26; Lovable</summary>

```
In this tutorial, we will build a Luma-style event platform using Lovable and [Supabase](https://docs.lovable.dev/integrations/supabase) – live\\\\\!

- How to integrate Supabase with Lovable
- Setting up authentication & user management
- Configuring databases & real-time comments
- Testing performance & handling multiple users
- Live debugging & performance optimization
```

</details>

<details>

<summary>Build an AI-Enhanced Web App</summary>

```
In this tutorial, we’ll show you how to use Lovable, an AI-enhanced no-code builder, to create a full-stack journaling app without writing a single line of code\\\\\!

- Design your app UI instantly
- Upload your design & generate a working app
- Connect Supabase for backend & authentication
- Implement GPT-4o for AI-powered features
- Deploy a full-stack app in minutes\\\\\\\!
```

</details>

<details>

<summary>Build a Simple CRM with Resend</summary>

```
In this tutorial, we'll walk through creating a simple yet powerful CRM using [Lovable](/lovable-f9060f1e/lovable-f9060f1e/editor/main.md#build-a-simple-crm-with-resend) for development, Supabase for data storage, and [Resend](https://docs.lovable.dev/integrations/resend) for email automation.

- How Resend works for email automation
- Setting up authentication emails with Supabase
- Building an admin dashboard & contact management system
- Creating & customizing email templates
- Adding newsletter signup & broadcast email functionality
```

</details>

<details>

<summary>Build Interactive Elements in Web Development</summary>

```
Building engaging, interactive web experiences just got easier with Lovable’s latest updates\\\!

```

#### Effortless UI Customization with Visual Edits

One of the biggest upgrades to Lovable is the ability to modify UI elements instantly without consuming AI credits. You can now:

```
    - Edit text directly on your project.
    - Adjust button colors and styles in real-time.
    - Upload and swap images seamlessly.
    - Hover over elements to make quick adjustments.

    
```

#### Advanced Debugging and API Error Handling

Previously, users faced challenges when dealing with third-party API integration errors. Lovable now:

```
    - Surfaces richer error messages for easier debugging.
    - Eliminates irrelevant popups, improving focus on critical issues.
    - Enables AI-driven error detection for automatic fixes.

    
```

#### Creating Dynamic Backgrounds and Animations

Lovable now supports seamless integration of animated and interactive elements using **p5.js** and other libraries.

```
    #### **Example Project: Travel Agency Website with Interactive Flags**

    A recent live demo showcased how to build a travel agency landing page featuring:

    1. **An animated hero section** with flags dynamically appearing and moving in response to mouse interactions.
    2. **A sticky-scroll section** that changes based on the user’s scroll position.
    3. **Interactive hover effects** where images react to user movements.

    #### **How to Implement Animated Effects**

    To create these effects, users followed this simple process:

    - **Define the desired animation:**

    
    - **Use p5.js to generate effects:**
      - Implement a chromatic smoke pattern.
      - Swap out static images for dynamic flag animations.
    - **Enhance user experience with physics-based interactions:**
      - Make elements move dynamically based on user actions.

    
```

#### Importing Custom Elements from External Libraries

With [**21st.dev**](video-tutorials.md), users can now integrate pre-built UI components seamlessly into Lovable projects.

```
    1. Browse **21st.dev** for a button design.
    2. Copy the AI-generated prompt.
    3. Paste it into Lovable and replace an existing button.

    This approach accelerates design workflows and allows for more polished, visually cohesive interfaces.

    
```

</details>

<details>

<summary>Clerk Authentication, Custom Domains &#x26; Waitlists</summary>

```
In this tutorial, we'll walk through building a **custom CRM** (Customer Relationship Management system) using [**Lovable**](/lovable-f9060f1e/lovable-f9060f1e/editor/main.md#clerk-authentication-custom-domains-and-waitlists) and [**Clerk**](https://docs.lovable.dev/integrations/clerk).
```

</details>

<details>

<summary>How to Build a Custom CRM with Lovable and Make</summary>

```
In this tutorial, we'll walk through building a **custom CRM** (Customer Relationship Management system) using [**Lovable**](/lovable-f9060f1e/lovable-f9060f1e/editor/main.md#how-to-build-a-custom-crm-with-lovable-and-make) and [**Make**](https://docs.lovable.dev/integrations/make).
```

</details>

<details>

<summary>Building a $10K Landing Page in 1 Hour</summary>



</details>

### Build, Brand, and Launch a real micro-SaaS, live!

Learning Spanish has never been this interactive! Imagine an app that not only teaches you Spanish through conversations but also creates real-time voice interactions, dynamic courses, and visually engaging content—powered entirely by AI. This tutorial can help follow step-by-step what Kristian and Harry built:

<details>

<summary>Step 1: Designing the Core Features</summary>

#### Laying the Foundations

Before implementing AI features, we focused on **building a strong foundation** for the app using **Lovable**. This included setting up authentication, structuring the dashboard, and implementing user management.

#### Authentication System

* Integrated **Supabase** for backend authentication.\
  \- Enabled sign-up/login with email and password.\
  \- Created a profile system to store user preferences and learning progress.

#### Dashboard & Navigation

* Designed an intuitive sidebar for navigation.\
  \- Created sections for chat, courses, and user settings.\
  \- Ensured responsive UI for a seamless experience across devices.

#### User Profiles & Data Storage

* Added a database structure to store user progress.\
  \- Designed profile management settings where users can adjust learning preferences.

</details>

<details>

<summary>Step 2: AI-Powered Learning Features with Replicate</summary>

#### AI-Generated Courses

To make learning interactive, we implemented an AI-driven course generation system using [OpenAI’s GPT model](video-tutorials.md). Here's how it works:

```
    1. Users select a topic (e.g., “Questions to ask at a barbecue”).
    2. Lovable calls an [OpenAI Edge function]() to generate **10 engaging Spanish-language questions**.
    3. Users complete quizzes, track progress, and receive AI feedback on their answers.
```

#### Enhancing User Engagement

* **Dynamically Generated Questions**: Each quiz is AI-generated, ensuring fresh, unique content every time.\
  \- **Interactive Feedback**: The AI provides explanations for correct and incorrect answers to improve learning.\
  \- **Progress Tracking**: Users can save and revisit courses, enhancing retention and practice.

#### Enhancing Visual Engagement with Replicate

To add a visual learning element, we integrated [**Replicate’s Flux Schnell**](video-tutorials.md) image generation model:

```
    - **Automated Course Banners**: Every course dynamically generates an image matching the topic.
    - **Visually Immersive Experience**: AI-driven visuals enhance user engagement and retention.
    - **Fast Image Processing**: Using Replicate’s API, images are generated in real time without slowing down the experience.
```

#### Real-Time Voice Conversations

A major milestone in the app's development was the addition of **real-time Spanish-speaking practice** using [OpenAI’s real-time WebRTC API](video-tutorials.md) :

```
    - **Interactive AI Tutor**: Users can speak directly with an AI that dynamically responds in Spanish.
    - **Pronunciation Assistance**: The AI provides real-time corrections and suggestions.
    - **Seamless Conversations**: The natural flow of conversation makes it feel like interacting with a human tutor.
```

</details>

<details>

<summary>Step 3: Branding the App</summary>

#### Establishing the Concept and Audience

Before branding, we defined our core goals:

```
    - **AI-powered chat** for real-time Spanish conversations.
    - **Automated quizzes** for quick practice sessions.
    - **Structured learning** with lesson storage and progress tracking.

    This helped shape our branding choices, ensuring they aligned with the app’s purpose.
```

#### Naming & Domain Selection

We aimed for a short, memorable name that reflected the **learning journey**. Using AI, we brainstormed and landed on **Ruta** (Spanish for “route” or “path”).

```
    #### **Process:**

    - **Brainstormed names** using AI for catchy Spanish words.
    - **Tested options** like "Camino" and "Verbo," but "Ruta" stood out.
    - **Checked domain availability** and secured **rutaapp.com** immediately.
```

#### Creating a Visual Identity

We quickly designed the brand:

```
    - **Logo**: A **compass-themed** icon sourced from design libraries and edited in Figma.
    - **Font Pairing**: Used a **bold, modern typeface** for the logo and a readable UI font for the app interface.
    - **Color Palette**: A **Tailwind CSS blue** scheme to symbolize travel and discovery.
    - **Styling Inspiration**: Experimented with **neo-brutalism**, tweaking contrast, shadows, and borders to create a visually engaging UI.
```

#### Building a Cohesive User Experience

Using Lovable, we ensured **visual consistency** across the app:

```
    - **Landing Page**: AI-generated with a dynamic, engaging hero section.
    - **Dashboard & Course Pages**: Styled to match the brand’s identity.
    - **Iterative Styling**: Applied **neo-brutalist** elements to test different design styles.
    - **User Flow Testing**: Ensured seamless navigation from signup to real-time chat.
```

</details>

<details>

<summary>Step 4: Final Tweaks, Big Bets &#x26; Live Launch</summary>



</details>

### Community Tutorials

<details>

<summary>Build a Car Prompt Engineering Agent</summary>



</details>

<details>

<summary>Build a SaaS Landing Page</summary>



</details>

<details>

<summary>Build an AI Coding Agent with Supabase &#x26; Stripe</summary>



</details>

<details>

<summary>Build a Chat-Based Interface</summary>



</details>

<details>

<summary>Build a Course Platform</summary>



</details>

<details>

<summary>Build SaaS Startup with Supabase</summary>



</details>

<details>

<summary>Build an AI-powered Web Application with OpenAI API</summary>



</details>

<details>

<summary>Build an SEO Landing Page</summary>



</details>

<details>

<summary>Build a Marketing Landing Page</summary>



</details>

<details>

<summary>Build a Todo List App</summary>



</details>

<details>

<summary>Build AI Agents</summary>



</details>

<details>

<summary>Build a Recipe Tracking App</summary>



</details>

<details>

<summary>Build a Fullstack Social Networking App</summary>



</details>

<details>

<summary>Lovable + Cursor</summary>



</details>

<details>

<summary>Build Text-to-Web App Platform</summary>



</details>

<details>

<summary>Build an AI-powered Note Taker</summary>



</details>

<details>

<summary>Build a Wealth Tracker App</summary>



</details>

<details>

<summary>Build an SEO Lead Generation Website</summary>



</details>

<details>

<summary>Build a Hiring Platform with Advanced Troubleshooting and Cursor</summary>

#### Start with Inspiration

Every project starts with a clear vision. For this MVP, the client wanted an **AI-powered dashboard**.

```
    To kickstart the design process:

    - Took a screenshot of a relevant landing page.
    - Asked [**ChatGPT**]() to describe the design in detail—layout, sections, colors, and typography.
    - Used this breakdown as the **foundation for building in Lovable**

    
```

#### Build the Core with Lovable

Once the blueprint was ready, Lovable handled the **entire foundation of the app**.

#### GitHub Integration

Lovable **automatically creates a** [**GitHub repository**](video-tutorials.md) for your project, syncing updates effortlessly. **Workflow:**

```
  </Step>
  
  </Step>
  
    This feature **saves hours** by keeping teams aligned on progress.
  </Step>
  
  </Step>
  
  </Step>
  
  </Step>
  
</Steps>
This streamlined workflow—**ChatGPT for planning, Lovable for building, and Cursor for refining**—significantly **reduces MVP development time**.
```

</details>

<details>

<summary>Build an MVP with Lovable</summary>



</details>

<details>

<summary>Build a Business Offer Comparison Tool</summary>



</details>

<details>

<summary>Build a Website Connected to Airtable</summary>



</details>

<details>

<summary>Build a Responsive Search Bar</summary>



</details>

<details>

<summary>Build a Personalized Healthcare Management for Individuals and Families</summary>



</details>

<details>

<summary>Build a Pet Shop App</summary>



</details>

<details>

<summary>Build an Intelligent Photo Organizer</summary>



</details>

<details>

<summary>Build a Personal Website</summary>



</details>

<details>

<summary>Build a Youtube Clone</summary>



</details>

<details>

<summary>Build an AI Automation Tool with Zapier &#x26; Lovable</summary>



</details>

<details>

<summary>Build a Trickle AI Review Copycat</summary>



</details>

<details>

<summary>Build a Trello Clone</summary>



</details>

<details>

<summary>Build a Student Discovery Platform</summary>



</details>

<details>

<summary>Build an AI Book Generator</summary>



</details>

<details>

<summary>Build a PDF Editor</summary>



</details>

<details>

<summary>Build a Cryptocurrency Dashboard</summary>



</details>

<details>

<summary>Build a Shopify Scrapping Tool with Firecrawl</summary>



</details>

More videos available [here](https://www.youtube.com/playlist?list=PLbVHz4urQBZkJ6WMXlIGc3NGsufrleogY).

### Comparison to other tools

<details>

<summary>AI Coding tools</summary>



</details>

<details>

<summary>Bolt vs Lovable</summary>



</details>

<details>

<summary>Databutton vs Lovable</summary>



</details>

<details>

<summary>Figma vs Lovable</summary>



</details>
