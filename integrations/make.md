---
title: "Integration with Make"
description: "Learn how to integrate Make with your Lovable application"
icon: "wand-sparkles"
---

## What is Make

<figure><img src="/images/make-hero.png" alt="Make website"><figcaption></figcaption></figure>

[Make](https://www.make.com) is a powerful no-code automation platform that lets you visually build workflows across apps, APIs, and data sources.

Instead of writing backend logic, you drag, drop, and connect modules in a flowchart-style canvas. It’s ideal for:

- **Non-developers** who want automation without writing code
- **Developers** who want fast prototyping or extendability via APIs
- **Teams** looking to connect tools like Slack, Airtable, Notion, Calendly, Supabase, and more

With Make, you can:

- **Trigger actions** from your Lovable app (e.g., when a button is clicked)
- **Send and receive data** via webhooks and APIs
- **Connect with 1,500\+ tools** or custom APIs
- **Automate** tasks like emailing, AI calling, enrichment, and reminders

## Why Use Make with Lovable?

In this below tutorial, Make acts as your **AI-enabled backend**, while Lovable powers the frontend. The result: a custom CRM, built in minutes, fully automated.

This setup is ideal for:

- Non-developers needing advanced logic
- Sales teams with evolving workflows
- Fast iteration without backend overhead
- API-powered automations with real-time UI responses

## Step-by-Step tutorial

### What we'll Build

You're going to create a CRM with three core data models:

- **Deals** (with stage-based tracking)
- **Contacts** (with inline editing)
- **Companies** (with enrichable data)

Each entity interacts with automations via Make. By the end, you’ll be able to:

- Move a deal and trigger an email
- Click a contact and start an AI sales call
- Click a company and fetch real-time data
- Secure everything via Supabase Edge Functions

### How are we going to build it

Building your own CRM can take months. With **Lovable** and **Make**, you can ship one in under an hour — and automate the entire sales workflow without writing backend code. In this step-by-step guide, you’ll learn how to build a **fully functional, AI-powered CRM**, complete with:

- Visual deal pipelines (drag-and-drop)
- Editable contact and company modals
- AI call agents using [Vapi](https://vapi.ai/)
- Company data enrichment via [Apollo.io](http://Apollo.io)
- Email workflows and security with Supabase
- Real-time automations using [Make](https://www.make.com)

### Setting Up Your CRM in Lovable

    
  

    
  </Step>
  

    
  </Step>
  
        <figure><img src="/images/call-customer-make.png" alt="Call Customer Make Pn"><figcaption></figcaption></figure>

  </Step>
  

### Call Apollo.io API
<figure><img src="/images/apollo-make-lovable.png" alt="Apollo Make Lovable Pn"><figcaption></figcaption></figure>

        - Use Apollo’s [Organization Enrichment API.](https://apollo.io/docs)
        - Fetch:
          - Industry
          - Employee count
          - Address
          - Website
          - Funding
        - Return the enriched data to Lovable.

### Parse Response into Modal View
<figure><img src="/images/webhook-apollo-webhook-make.png" alt="Webhook Apollo Webhook Make Pn"><figcaption></figcaption></figure>

        - Dynamically generate fields in the Lovable modal from the JSON.
        - Present data in a readable UI (not raw JSON).

        

  </Step>
  
    
  </Step>
  
  </Step>
  
  
</Steps>

## Pro Tips from the Live Session

- Use **select \+ prompt** inside Lovable for precision edits
- Use **Make’s Visual Canvas** to map out flows before connecting them
- Dynamically parse unknown JSON fields into modals for UX win
- Combine Vapi \+ Apollo \+ Make for real-time AI workflows
- Use Supabase Edge Functions to mask all public API/webhook calls

## FAQ

  <details>
<summary>What is Make?</summary>
Make is a visual automation platform that lets you connect tools and build workflows using drag-and-drop modules. Think of it as Zapier but more flexible and developer-friendly.
</details>
  <details>
<summary>Why use Make with Lovable?</summary>
- No need to write backend code
    - Trigger workflows from your UI (buttons, forms, modals)
    - Build automations visually (call agents, enrichment, email flows)
    - Connect to 1,500\+ apps (Slack, Notion, Calendly, Airtable, and more)
</details>
  <details>
<summary>How does Make communicate with Lovable?</summary>
Lovable sends data (usually as JSON) via **HTTP webhooks** to Make scenarios. Make receives that data, processes it (e.g., calls an API), and can respond back to Lovable.
</details>
  <details>
<summary>What are Scenarios in Make?</summary>
Scenarios are automation workflows. You define:

    - Triggers (e.g., Webhook)
    - Actions (e.g., API call, email send)
    - Logic (routers, filters, iterations)
</details>
  <details>
<summary>Can I secure my Make Webhooks?</summary>
Yes. Use:

    - **IP restrictions** (limit who can call the webhook)
    - **Supabase Edge Functions** to proxy and hide sensitive URLs
    - **API Key authentication** in headers
</details>
  <details>
<summary>What’s the difference between Make and Supabase Edge Functions?</summary>
- **Make** is a visual automation tool (great for workflows, API integrations, AI triggers).
    - **Supabase Edge Functions** are serverless backend code (great for logic, auth, and security).

    Use them **together** for best results.
</details>
  <details>
<summary>What happens if I exceed my Make plan's operations?</summary>
Your scenario will pause. Make sends alerts, and you can upgrade or optimize your flows. For this guide, the **free pro plan** from the webinar includes **20,000 operations** — more than enough to prototype.
</details>
  <details>
<summary>Can I test my Make Scenarios without Lovable?</summary>
Yes\! Use **manual data input** in the Webhook or trigger the scenario via Postman or curl. This is great for debugging before connecting to Lovable.
</details>

## Resources

- [Make](https://www.make.com)
- [Vapi AI](https://vapi.ai/)
- [Apollo.io Enrichment API](https://apollo.io/docs)
- [Supabase Edge Functions](https://supabase.com/docs/guides/functions)
- Explore **Make Academy**: [academy.make.com](https://academy.make.com)