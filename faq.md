---
title: "FAQ"
description: "Frequently asked questions about Lovable"
icon: "circle-question"
---

## Lovable Interface

  <details>
<summary>What is the Lovable dashboard?</summary>
The dashboard is where you manage your projects, view your credits, control project visibility, and access settings.
</details>
  <details>
<summary>How should I structure my prompts for the best results?</summary>
- Be **clear and specific** (e.g., _"Create a signup page with email and password using Supabase."_).
    - Avoid vague instructions.
    - Describe expected outcomes to guide the AI.

    More information [here](https://docs.lovable.dev/tips-tricks/prompting).
</details>
  <details>
<summary>How do I change my project’s visibility?</summary>
In your project settings, you can toggle your project between public and private mode.
</details>
  <details>
<summary>What does the chat feature do?</summary>
The chat feature allows you to interact with Lovable's AI without modifying your code. You can ask questions, get explanations, and debug issues.
</details>
  <details>
<summary>Can I see the code that Lovable generates?</summary>
Yes, you can toggle the code viewer to inspect the AI-generated code.
</details>
  <details>
<summary>Can I edit the generated code?</summary>
Yes, but full code editing is available only on certain paid plans. However, you can use Lovable’s edit mode to make changes visually.
</details>
  <details>
<summary>How do I create a landing page?</summary>
Simply type a prompt like:

    
    Lovable will generate a page based on your input.
</details>
  <details>
<summary>Can I import designs from Figma?</summary>
Yes, you can import Figma files to Lovable and use them as a starting point for your project.
</details>
  <details>
<summary>How do I add animations to my project?</summary>
Use a prompt like:

    
    Lovable supports frameworks like P5.js for animations.
</details>
  <details>
<summary>How do I connect my project to a database?</summary>
You can use **Supabase**, a backend-as-a-service solution that integrates seamlessly with Lovable.
</details>
  <details>
<summary>Can I add authentication to my project?</summary>
Yes, you can integrate authentication using Supabase, Clerk, or Magic.link by prompting Lovable to create login and signup pages.
</details>
  <details>
<summary>How do I track changes in my project?</summary>
Lovable provides a **history feature** where you can view and restore previous versions of your project.
</details>
  <details>
<summary>What is a remix?</summary>
Remixing a project creates a duplicate that you can modify separately, allowing you to explore different versions of your project.
</details>
  <details>
<summary>Can I copy and edit someone else’s project?</summary>
If a project is public and remixing is enabled, you can create your own copy and customize it.
</details>
  <details>
<summary>Can I export my project and host it elsewhere?</summary>
Yes\! By linking your project to **GitHub**, you can export your code and host it on your preferred server.
</details>
  <details>
<summary>Can I integrate payment systems?</summary>
Yes, Lovable supports **Stripe, PayPal, and other payment providers**. Just prompt Lovable to set up the payment system you prefer.

    Follow [this guide](https://docs.lovable.dev/tips-tricks/setting-up-payments) to set it up.
</details>
  <details>
<summary>Can I invite others to collaborate on my project?</summary>
Yes, view details on collaboration [here](https://docs.lovable.dev/user-guides/teams).
</details>
  <details>
<summary>Can I showcase my projects?</summary>
Yes\! You can share your project in the [**Lovable Launch**](https://launched.lovable.app/) section and on social media.
</details>
  <details>
<summary>Does Lovable support mobile app development?</summary>
No, Lovable is focused on **web applications**, but you can design mobile-friendly web apps.
</details>

## Getting Started

  <details>
<summary>What is Lovable?</summary>
Lovable is an AI-powered platform that enables users of any skill level to create full-stack web applications without requiring coding expertise by simply describing what they want in plain English. Instead of hiring developers, users can generate web apps or websites instantly.
</details>
  <details>
<summary>How do I sign up and get started?</summary>
Simply create an account on Lovable, explore the interface, and start building by typing prompts that describe what you want to create.
</details>
  <details>
<summary>What can I build with Lovable?</summary>
You can build landing pages, web applications, AI-powered tools, authentication systems, and more.
</details>
  <details>
<summary>Can I start from templates?</summary>
Yes\! Lovable offers pre-built templates to help you get started quickly. Browse them [here](https://lovable.dev/templates).

    

</details>
  <details>
<summary>Can I import existing code from GitHub?</summary>
Not yet, but we're exploring this [feature request](/lovable-f9060f1e/lovable-f9060f1e/editor/main.md#can-i-import-existing-code-from-github).
</details>
  <details>
<summary>How do I build a role-based system for a SaaS app?</summary>
Creating a secure, role-based system involves:

    - Using **Supabase authentication** to assign user roles (Admin, User, Guest, etc.).
    - Applying **Row-Level Security (RLS)** to control data access for different users.
    - Leveraging **Edge Functions** for API security, ensuring only authorized users can perform specific actions.
</details>
  <details>
<summary>Does prompt optimization count towards my usage limit?</summary>
Yes, prompt optimization may use tokens, but Lovable is designed to minimize unnecessary interactions and maximize efficiency.
</details>
  <details>
<summary>Do I need coding experience to build an app?</summary>
No\! Lovable is designed for all levels of experience. Whether you're a developer or a non-technical user, you can easily create projects using AI assistance.

    Lovable allows non-technical users to create apps through a structured workflow: **plan, prompt, scaffold, debug, and deploy.** You can generate project documentation, break the process into steps, and let AI guide you.
</details>
  <details>
<summary>Can I learn coding with Lovable?</summary>
Yes\! The best way to learn is by doing. Lovable helps you understand coding by:

    - Generating and explaining code.
    - Encouraging pattern recognition in AI-generated responses.
    - Allowing experimentation and debugging.

    **Recommended learning resources:**

    - [Coding with AI](https://www.loom.com/share/4820c0119b314b26af7faa515666be24?sid=4eac28fc-de30-4500-91d0-535c0b508907) by 50in50Challenge (free)
    - [Build & Launch with Lovable](https://aclasswithharry.com/) by [Harry](https://x.com/Harry_Aldian/status/1892636006056128703) ($20)
    - [Weekend Developer Live Sesh](https://ssdavidai.gumroad.com/l/weekendlivesesh) by [David Szabo-Stuban](https://ssdavidai.gumroad.com/) ($97)

    These courses provide hands-on learning experiences to help you master Lovable more effectively. 🚀
</details>
  <details>
<summary>How long does it take to build a full-stack app?</summary>
It depends on complexity. By breaking tasks into smaller steps, planning ahead, and refining based on feedback, you can move quickly while ensuring quality.
</details>
  <details>
<summary>How do I build my website with Lovable?</summary>
1. **Structure the site** – Define key sections like homepage, about, features, and testimonials.
    2. **Design** – Customize fonts, colors, and layouts for a professional look.
    3. **Add content** – Embed images, videos, and text to make it engaging.
    4. **Refine & launch** – Optimize responsiveness and ensure smooth interactions.
</details>
  <details>
<summary>Do I need a Chief Technical Officer (CTO) for my MVP?</summary>
No\! If your project is straightforward, Lovable’s AI can help you build and refine it. However, if you plan to scale rapidly or need advanced features, having technical support may be beneficial.
</details>
  <details>
<summary>What should I do if I encounter an issue with Lovable?</summary>
Lovable provides an AI-driven debugging tool that analyzes errors in real time. If an error occurs:

    - Click "Try to Fix."
    - Use **Chat Mode** to describe the issue and ask Lovable to debug it.
    - Review error logs and console output for additional details.

    Try refreshing your session or [reviewing documentation](https://docs.lovable.dev/tips-tricks/troubleshooting). If the issue persists, contact **Lovable Support** through our [support page](https://lovable.dev/support).
</details>
  <details>
<summary>What is Supabase and how does it help Lovable users?</summary>
Supabase is an open-source backend-as-a-service that provides authentication, databases (PostgreSQL), storage, and real-time capabilities. It helps Lovable users by handling data storage, authentication, and other backend functionalities without requiring manual setup.
</details>
  <details>
<summary>What’s the best way to structure a project in Lovable?</summary>
Start with **chat mode** to explore your idea and build a plan. Only move to **edit mode** once the vision is clear. Many users spend **80% of their time in chat**, not building—**planning**.
</details>
  <details>
<summary>Can I send diagrams or screenshots?</summary>
Yes\! Diagrams (from Miro/FigJam/etc.) and screenshots are super helpful—especially for flows and UI bugs. While videos aren’t supported yet, screenshots can often do the job.
</details>

## Development & Features

  <details>
<summary>Can I download the code Lovable generates?</summary>
Yes\! You can access and manage your generated code via our [GitHub integration](/integrations/git-integration.md).
</details>
  <details>
<summary>Does Lovable support custom backends?</summary>
Yes\! Lovable-generated code can connect to any backend, including [Supabase](https://docs.lovable.dev/integrations/supabase) for database management and authentication.
</details>
  <details>
<summary>What frameworks does Lovable support?</summary>
Currently, Lovable supports **Vite and React**. NextJS and React Native are not yet available.
</details>
  <details>
<summary>How does Lovable handle duplicate code?</summary>
AI now detects and removes duplicate files, preventing errors and ensuring clean project management.
</details>
  <details>
<summary>What is a webhook?</summary>
A webhook allows two applications to communicate in real-time by sending data when an event occurs (e.g., a new user signs up, triggering an email notification).
</details>
  <details>
<summary>What is refactoring, and why is it important?</summary>
Refactoring improves code structure and efficiency without altering functionality. It helps:

    - Optimize performance by removing redundancies.
    - Improve maintainability for future updates.
    - Prevent conflicts by structuring logic more clearly.
</details>
  <details>
<summary>Can I use Lovable for frontend development?</summary>
Yes\! Lovable is perfect for frontend development, offering:

    - **Component-Based Development** – Build with React and Vite.
    - **AI-Assisted Code Generation** – Generate layouts and UI components easily.
    - **Mobile-First Design** – Implement responsive designs with Tailwind CSS.
    - **Real-Time Preview** – See changes instantly and deploy efficiently.

    [Check out the full article.](https://lovable.dev/blog/frontend-development-with-lovable)
</details>
  <details>
<summary>How can I improve my project with Lovable?</summary>
- **Refine components** using AI-driven prompts.
    - **Add new features** with clear, detailed instructions.
    - **Edit UI elements directly** using select-to-edit.
    - **Track and revert changes** via version history.
</details>
  <details>
<summary>What’s the best way to prevent unexpected regressions when validating code?</summary>
- **Use chat mode** to verify changes before applying them.
    - **Lock critical files** to prevent unintentional edits.
    - **Implement version control** (GitHub) to track changes.
    - **Write detailed prompts** so the AI understands dependencies.
</details>
  <details>
<summary>How can I improve SEO for my Lovable app?</summary>
Lovable apps are single-page applications (SPAs), which can impact SEO. To improve SEO:

    - Use **metadata and Open Graph tags**.
    - Optimize for **server-side rendering (SSR)** using tools like Vercel.
    - Generate static pages for better indexing.

    To optimize your website for SEO & traffic, you can [check out this section](https://docs.lovable.dev/tips-tricks/seo).
</details>
  <details>
<summary>Can multiple users collaborate on a Lovable project?</summary>
This is a feature request under development.
</details>
  <details>
<summary>Can I use Lovable with a custom domain?</summary>
Yes, you can set up [custom domains](https://docs.lovable.dev/tips-tricks/custom-domain) using **Entri, Vercel, Netlify, or other hosting services**.
</details>
  <details>
<summary>How do I deploy a Lovable app?</summary>
1. Click the **Publish** button, and Lovable will deploy your project to a live URL.
    2. Lovable will generate a shareable URL.
    3. You can also connect for [custom domain](https://docs.lovable.dev/tips-tricks/custom-domain) hosting.
</details>
  <details>
<summary>Can I edit Lovable-generated code?</summary>
Yes\! Lovable provides a **Code Viewer** that allows paid users to view and make minor edits to the underlying project files. You can enable this feature in \*\*Account Settings \> \*\*
</details>
  <details>
<summary>What is an Edge Function?</summary>
An **Edge Function** is a small serverless function in [Supabase](https://docs.lovable.dev/integrations/supabase) that runs logic on the backend, such as sending emails or processing API calls.
</details>
  <details>
<summary>What should I include in my Knowledge File?</summary>
Everything. Treat it like a product brief:

    - Vision & goals
    - User persona & journey
    - Naming (project, company, pages)
    - Feature breakdown
    - Guidelines like:
      - “Be incremental when building.”
      - “Don’t over-engineer.”
      - “Stick to the design system.”

    Add it once and Lovable will use it in every prompt.
</details>

## Debugging & Troubleshooting

  <details>
<summary>What should I do when I hit an error that won’t go away?</summary>
**Great question\!** You’re not alone—everyone runs into these loops sometimes.

    Here’s what we recommend:

    

### Try to fix (free)
**Try fixing the error twice** using edit mode or chat mode.

### Chat Mode
If it still loops or creates more issues, **switch fully to chat mode** and debug by explaining what you're seeing.

        Use prompts like:

        - “Explain the error and how to fix it.”
        - “List the steps you're taking and why.”
        - “What's different between this and your previous solution?”

### Restore
If that doesn’t work, **restore a previous working version**, **remix the project**, or **report it** via Discord or paid support.

    
</details>
  <details>
<summary>Where can I get help if I'm stuck?</summary>
- Use [**Chat Mode**](https://docs.lovable.dev/features/labs#chat-mode) for AI assistance.
    - Check [**documentation**](https://docs.lovable.dev/) for guidance.
    - Join the [**Discord community**](https://discord.gg/lovable-dev) for real-time help.
</details>
  <details>
<summary>What should I do when my app breaks?</summary>
Here’s a safe recovery pattern:

    1. **Version tag** every stable moment.
    2. If something breaks, **don’t keep building**—revert.
    3. Remix from a working front-end version and re-implement backend or complex logic gradually.
</details>
  <details>
<summary>How do I avoid prompt confusion or loops?</summary>
Give _more_ context, not less. Long, structured prompts work better:

    - Describe what the user should see, click, and do.
    - Clarify what part of the app it affects.
    - Be explicit: “Add a login button that redirects to dashboard after login (Google, Slack, email).”
</details>
  <details>
<summary>What support options do I have?</summary>
2 options here:

    - **Free users**: Community help via [Discord](https://discord.gg/lovable-dev).
    - [**Paid users**](https://lovable.dev/support): Access to AI-powered support _plus_ the “Speak to a human” option anytime (platform-related issues). We respond same-day for paid users.
</details>

## AI and Automation

  <details>
<summary>Can I add third-party APIs to my project?</summary>
Yes, you can integrate APIs like OpenAI, Stripe, and more by specifying them in your prompt.
</details>
  <details>
<summary>Can I store sensitive API keys in Lovable?</summary>
No\! Never enter your API keys directly in Lovable. Use environment variables to keep them secure.
</details>
  <details>
<summary>How does Lovable AI remember context?</summary>
Lovable processes recent messages to maintain context. For the best results, include relevant details in each prompt to ensure clarity and accuracy.
</details>
  <details>
<summary>Can Lovable build complex B2B SaaS apps?</summary>
Yes\! Lovable supports:

    - **Workflow automation** for business processes.
    - **Role-based access controls** for different user levels.
    - **Document generation** with built-in logic for approvals and signatures.
    - & so much more.
</details>
  <details>
<summary>Why did Lovable switch from Python to Go?</summary>
Lovable migrated [from Python to Go](https://lovable.dev/blog/from-python-to-go) to improve performance, scalability, and developer experience. Go enables faster processing, lower latency, and better efficiency, especially for handling large-scale AI-driven tasks.
</details>
  <details>
<summary>What is the character limit for prompts?</summary>
Due to AI constraints, prompts are limited to **approximately 180K tokens (≈720K characters).**
</details>
  <details>
<summary>Can I run my AI model on Lovable without an API?</summary>
Probably not. Most AI models require an API for proper integration.
</details>

## Pricing & Account Settings

  <details>
<summary>What are credits in Lovable?</summary>
Credits are used for AI-powered actions like generating code or making edits. Each message you send to the AI costs one credit.
</details>
  <details>
<summary>Do long and short prompts cost the same?</summary>
Yes, each message sent counts as one credit, regardless of length.
</details>
  <details>
<summary>How do I get more credits?</summary>
You can upgrade your plan or purchase additional credits in Account Settings. More information [here](https://docs.lovable.dev/user-guides/messaging-limits#upgrading-and-downgrading-plans).
</details>
  <details>
<summary>When does my token count reset?</summary>
Monthly, on the same date you subscribed.
</details>
  <details>
<summary>Can I top up my monthly limit?</summary>
No, but you can upgrade or downgrade plans based on your needs.
</details>
  <details>
<summary>How can I check my remaining messages?</summary>
Go to **Account Settings** and check the **credits/messages left** section.
</details>
  <details>
<summary>Can I delete my account?</summary>
Yes, contact  for account deletion requests.
</details>
  <details>
<summary>Can I change my email?</summary>
Currently, it is not possible to change your email linked to the account.
</details>
  <details>
<summary>Can I delete a project?</summary>
Yes\! Navigate to **Project Settings → Danger Zone → Delete Project.**
</details>
  <details>
<summary>How does Lovable ensure data security?</summary>
Lovable follows [industry-standard security practices](https://lovable.dev/privacy), including encryption, secure API connections, and regular security audits to protect user data.
</details>

## About Lovable

  <details>
<summary>What is the difference between Lovable & other AI builders?</summary>
People say Lovable has higher quality outputs, ship faster, better at full stack and more.

    That's kind of the break-down why we would recommend Lovable:

    - **Supabase integration**: Lovable just makes it smoother. You connect with an API key and you're good to go. No hoops.
    - **Image uploads** actually work. Didn’t have to debug anything.
    - **GitHub commits** show up cleanly as external updates. Easy to track changes.
    - **Precision edits with the visual editor** — it’s free. You can tweak small UI things without breaking stuff. It just feels like Figma was naturally integrated.
    - **"Try to fix" is free**, too. You don’t get punished for iterating.
    - **Chat mode** is way more natural. Feels like pair programming with an actual teammate.
    - **UX/UI output** is just better. It looks like something you'd actually ship.
    - **Product output is usable**. You get real controls, working links, multiple pages — not just a static playground.
    - **Community** is much bigger & more helpful and active.
    - **We're more ambitious** in terms of what they’re enabling - product and brand itself.
    - **Attention to detail** shows everywhere — naming, layouts, error handling.

    Other AI builders may still be valid solutions, but [<u>Lovable.dev</u>](http://lovable.dev/) feels more full-stack ready and thoughtful.
</details>
  <details>
<summary>What is the difference between Lovable & Cursor?</summary>
**Lovable and Cursor are both $20/month tools that help you build software with AI.** But they serve different needs, especially if you're just starting out.

    Here’s the simplest way to think about it:

    |                   | [Lovable](https://lovable.dev/)                           | Cursor                                              |
    | ----------------- | --------------------------------------------------------- | --------------------------------------------------- |
    | Built for         | Non-technical creators                                    | Developers                                          |
    | What it gives you | Working full-stack web app (UI \+ Backend \+ Database)    | Smart coding assistant inside your code editor      |
    | Requires coding   | No coding needed                                          | Yes you need to understand code                     |
    | Setup complexity  | Minimal - Supabase, Auth, API, deploy are handled for you | You start from scratch and wire everything manually |
    | Best for          | Building your MVP fast                                    | Customizing and scaling your app                    |
    | Learning curve    | Friendly                                                  | Steep but powerful                                  |
    | Output            | Deployed app                                              | Code you need to run yourself                       |

    If you’re **non-technical** and want to launch your **AI-powered web app** fast — [**Lovable**](https://lovable.dev/)\*\* is the better choice\*\*. It does the heavy lifting for you:

    - Spins up your backend (like Supabase) automatically
    - Lets you prompt in plain English
    - Deploys your app with one click
    - Gives you full code access when you’re ready to go deeper

    > Many builders start with Lovable, then export the code and refine it in Cursor once they’re more confident.

    You don’t have to choose one forever. Start with Lovable. Grow at your own pace.
</details>
  <details>
<summary>Does Lovable have a partner program?</summary>
Yes\! Join our [Affiliate Program](https://friends.lovable.dev/) and earn 20% commission for customer referrals.
</details>
  <details>
<summary>Where is Lovable based?</summary>
Lovable is **100% made in Europe**, with headquarters in **Stockholm, Sweden.**
</details>
  <details>
<summary>Is Lovable hiring?</summary>
Yes\! Check out our open positions [here](https://lovable.dev/careers). 🚀
</details>