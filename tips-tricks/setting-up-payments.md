---
title: "Stripe & Payments"
description: "How to set up payments in your app using our Stripe integration"
icon: "credit-card"
---

<figure><img src="/images/lovable-stripe.webp" alt="Integrate Stripe in Lovable"><figcaption></figcaption></figure>

Lovable now lets you set up Stripe entirely through **chat**.

**Chat‑driven auto‑setup (recommended)**  
   After you connect **Supabase** and save your **Stripe Secret Key** via **Add API Key**, just describe what you need:  
   - “Add three subscription tiers …”  
   - “Create a one‑time checkout for my e‑book at $29”  
   Lovable generates the checkout / portal edge functions, database tables with RLS, and UI buttons—no manual coding or webhooks unless you ask for them.

* For **one‑off sales**, be sure your cart or product page already works.
  * For **subscriptions**, confirm Supabase Auth is in place so Lovable can link Stripe customers to each user’s **id**

### Key Takeaways

- Use the **chat‑driven flow** for both subscriptions and one‑off payments.  
- **Never paste your Stripe Secret Key in chat.** Store it with **Add API Key**.  
- **Webhooks are opt‑in.** Lovable relies on edge‑function polling unless you request webhooks.  
- Debug in **Browser Console → Network/Errors**, **Supabase → Edge Functions → Logs**, and **Stripe Dashboard → Logs**.  
- Always test in **Stripe Test Mode**, then deploy.

## Requirements

Before integrating Stripe, ensure the following prerequisites are met:

- The project **must** be connected to Supabase. [Learn more about Supabase](https://docs.lovable.dev/integrations/supabase)
- A **Stripe account** with properly configured products.
- A working **frontend and backend**:
  - For individual product sales, ensure a shopping cart and checkout page are functional.
  - For subscriptions, set up login functionalities and different pricing tiers.

### **Please note**
Stripe integration doesn't work in preview. To test the integration, make sure to deploy. You should also make sure to be in test mode in Stripe when trying out the functionality. When testing payment, card number: 4242 4242 4242 4242, any 3 digits as CVC and any future date will work as a card.

## Stripe Payment Setup (No‑Code Chat Flow)

Lovable now generates all Stripe logic for you. Once your **Stripe Secret Key** is saved with **Add API Key** and your project is **connected to Supabase**, simply tell Lovable what you need in chat—no manual Payment Links required.

### Step 1
**Prep your project**

    - Supabase connected
    - Stripe Secret Key added via **Add API Key**
    - (Optional) Prices or product IDs handy

### Step 2
Examples:

    - Create a one-time checkout for my "Digital Course" at $29
    - Set up an annual Premium plan for $99, tied to each user's id

### Step 3
**Review & apply**
    Lovable auto‑scaffolds the Edge Functions, database tables, and UI components (all tied to the user's id in Supabase). Check the preview, then click **Apply** to deploy.

- Subscriptions should always linked to the authenticated user’s `id` in Supabase for secure, role‑based access.

## Advanced Integration: Webhooks & Supabase

For complex payment structures such as **subscriptions and role-based access**, Lovable recommends using **Supabase** to securely handle Stripe integration. This allows for proper webhook handling, subscription management, and role-based access control based on payment tiers.

The Edge Function that handles the necessary changes to the user account should be set up automatically by the AI.

### Connect Supabase to Your Project
Getting started is simple. Lovable makes connecting Supabase effortless with a built-in native integration:

    1. Click the **Supabase button** in the top right corner of Lovable.
    2. Follow the instructions to link your project.
    3. Once connected, Supabase enables secure payment processing, subscription management, webhook handling, customer data storage, and error handling.

### Secure Payment Processing
Initiate the process by prompting Lovable:

    
Let's connect Stripe to my project. We will begin with secure payment processing.

    Lovable will generate the necessary SQL schema for handling payments. This includes database tables for users, subscriptions, and payments. You can review and customize these tables to fit your specific product needs before applying changes.

### Implement Edge Functions for Webhooks
**Edge Functions** in Supabase act as small, high-performance serverless functions that run close to the user, ensuring fast responses. They help process webhook events, such as payment confirmations, before updating the database.

    
  
  
</Steps>

## Debugging & Troubleshooting

  <details>
<summary>Check Console Logs</summary>

### Step 1
Open **Developer Tools** (Right-click \> Inspect \> Console in Chrome).

### Step 2
Look for errors and review webhook event logs.

### Step 3
Copy error messages and ask Lovable for debugging assistance.

</details>
  <details>
<summary>Review Supabase Logs</summary>

### Step 1
Go to **Supabase Dashboard**

### Step 2
Edge Functions

### Step 3
Logs to check for webhook errors.

</details>
  <details>
<summary>Verify Webhook Events in Stripe</summary>

### Step 1
Navigate to **Stripe Dashboard**

### Step 2
Webhook logs

### Step 3
Confirm that Stripe is sending data correctly.

</details>
  <details>
<summary>Use Lovable Chat Mode</summary>

### Step 1
Switch to **chat mode** and ask Lovable follow-up questions.

### Step 2
Ask Lovable follow-up questions.

### Step 3
Use the **Rubber Duck Method** & explain your issue step by step to clarify the problem.

</details>