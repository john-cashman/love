---
title: "Integration with Resend"
description: "Learn how to integrate Resend with your Lovable application"
icon: "envelope"
---

## What is Resend

[Resend](https://resend.com/emails) is an email API built for developers. It focuses on high deliverability, ease of integration, and a clean developer experience for sending transactional and marketing emails.

## Step-by-step tutorial

This tutorial walks you through building a fully functional CRM in under an hour—complete with lead collection, email confirmation, newsletter subscription, and an internal admin dashboard. You'll use:

- **Lovable**: to generate the front end and backend logic.
- **Supabase**: for secure data storage and authentication.
- **Resend**: to automate and track transactional \+ marketing emails.

Let’s get started.

### Create a Landing Page with a Contact Form
Use Lovable's AI to quickly generate a landing page for your product or service.

    **Instructions:**

    
        <figure><img src="/images/landing-page-lovable-project.png" alt="Landing Page Lovable Project Pn"><figcaption></figcaption></figure>

### Inspect the generated code
Inspect the generated code or use the select tool to tweak elements.

### Add input validation
Add input validation and a `message` field for better user experience.

        <figure><img src="/images/email-resend-form.png" alt="Email Resend Form Pn"><figcaption></figcaption></figure>

  </Step>
  
  
  
  
  
  
  
  
</Steps>

## Want to go further?

- Add support for **scheduled emails** via Supabase cron jobs
- Build **automation flows** to trigger emails based on lead stages
- Style your UI for better brand trust and conversion

## Resend Integration FAQ

  <details>
<summary>What is Resend?</summary>
Resend is an email API built for developers. It focuses on high deliverability, ease of integration, and a clean developer experience for sending transactional and marketing emails.
</details>
  <details>
<summary>Do I need a paid Resend plan to follow this tutorial?</summary>
No. You can complete the entire CRM setup using **Resend’s free tier**, which supports sending emails from a verified domain and up to 3,000 contacts for marketing emails.
</details>
  <details>
<summary>How do I verify a domain in Resend?</summary>
Go to Resend → **Domains** → Add your domain. You’ll be given DNS records (TXT, MX) to add via your DNS provider (e.g., Cloudflare, Namecheap). Once added, click **Verify**.

    
</details>
  <details>
<summary>Why are my Resend emails going to spam?</summary>
There are a few common reasons:

    - You haven’t verified your domain
    - Your email lacks a plain-text version
    - You’re sending from a generic sender like `onboarding@resend.dev`
    - You’re not following best practices (e.g., missing unsubscribe links in marketing emails)

    Use Resend’s **Deliverability Insights** panel to get actionable tips.
</details>
  <details>
<summary>Can I customize the design of the emails I send?</summary>
Yes. Use [React Email](https://react.email/)—an open-source library by the Resend team—to design styled, responsive emails with React components.
</details>
  <details>
<summary>Does Resend support marketing emails or only transactional?</summary>
Resend supports **both**:

    - **Transactional emails** (confirmation, reset, notifications) using the API or SDK.
    - **Marketing emails** via the **Broadcast** feature and **Audiences**.

    You can create, preview, and track campaigns from the dashboard.
</details>
  <details>
<summary>How do I manage newsletter subscribers in Resend?</summary>
Use **Audiences**:

    - Add contacts manually, via CSV, or programmatically using the API.
    - Each Audience has a unique ID you can use to associate subscriptions.
    - Users can unsubscribe automatically via Resend’s built-in unsubscribe link.
</details>
  <details>
<summary>Can I set up double opt-in for newsletters?</summary>
Not by default, but you can implement it manually:

    1. On form submission, send an initial confirmation email.
    2. Ask users to click a link.
    3. On click, confirm their subscription and add them to your Resend audience.
</details>
  <details>
<summary>Can I schedule or automate email flows in Resend?</summary>
Not yet. Resend doesn’t currently support drip campaigns or automated sequences.

    
</details>
  <details>
<summary>How do I connect Resend to Supabase Auth?</summary>
Use the official Supabase Integration by Resend:

    1. Authenticate with your Supabase project.
    2. Provide a domain and sender name.
    3. Resend automatically configures your Supabase auth emails to use your Resend account.
</details>
  <details>
<summary>How does Resend handle unsubscribes?</summary>
Resend automatically processes unsubscribes:

    - You must include an unsubscribe link in broadcast emails.
    - When a user unsubscribes, they are removed from the selected audience.
    - This is required for email compliance (e.g., CAN-SPAM, GDPR).
</details>