---
title: "Integration with Clerk"
description: "Learn how to integrate Clerk with your Lovable application"
icon: "people-arrows"
---

## Why Clerk?

<figure><img src="/images/what-is-clerk.png" alt="What Is Clerk Pn"><figcaption></figcaption></figure>

[Clerk](https://clerk.com) handles authentication and user management so you don’t have to build it from scratch. With just a few prompts and config steps, you get:

- Secure sign-in & sign-up (social, password, MFA)
- Prebuilt UI components: user profiles, org management, impersonation
- Support for B2B apps (teams, roles, invitations)
- Integration with Supabase, Stripe (coming soon), and more
- Waitlist mode to manage early access
- Generous free tier: 10K MAUs

## Step-by-Step Integration Guide

Here is a step-by-step guide:

### Step 1
Create a Clerk Account → [Clerk.com](https://clerk.com)

### Step 2
In the Clerk dashboard, create a new app

        
      
            <figure><img src="/images/asana-clone-lovable.png" alt="Asana Clone Lovable Pn"><figcaption></figcaption></figure>

### Step 2
Paste your **Public API Key** when asked

### Step 3
Lovable scaffolds the login and sign-up pages

            <figure><img src="/images/waitlist-component-clerk.png" alt="Waitlist Component Clerk Pn"><figcaption></figcaption></figure>

### Step 4
Deploy & test — you’re now using Clerk Auth

      </Step>
    </Steps>
  </Step>
  
    Use Clerk’s built-in waitlist to collect users pre-launch.

    

### Step 1
In Clerk dashboard: **Configure \> Restrictions \> Waitlist**

### Step 2
New sign-ups will show as **pending**

### Step 3
- Users who sign up will now be **pending approval**
        - Admins can approve users from the Clerk dashboard

        <figure><img src="/images/clerk-waitlist-pending.png" alt="Clerk Waitlist Pending Pn"><figcaption></figcaption></figure>

### Step 4 (Bonus)
Customize waitlist emails (branding, content)

        <figure><img src="/images/clerk-email-templates.png" alt="Clerk Email Templates Pn"><figcaption></figcaption></figure>

        <figure><img src="/images/sms-code-verification.png" alt="Sms Code Verification Pn"><figcaption></figcaption></figure>

  </Step>
  
        <figure><img src="/images/clerk-organization-create.png" alt="Clerk Organization Create Pn"><figcaption></figcaption></figure>

    
  </Step>
  
    Troubleshoot your app as if you were a specific user.

    

### Step 1
In Clerk dashboard \> Users, click on a user

        <figure><img src="/images/impersonate-user-clerk.png" alt="Impersonate User Clerk Pn"><figcaption></figcaption></figure>

### Step 2
Click **Impersonate**

### Step 3
View your app from their perspective

### Step 4
Security: impersonators can’t perform sensitive actions (e.g. change password)

  </Step>
  
    **How to integrate:**

    

### Step 1
In Supabase, go to **Settings \> API \> JWT Secret (**[**documentation**](https://clerk.com/docs/integrations/databases/supabase)**)**

        <figure><img src="/images/supabase-clerk-integration-doc.png" alt="Supabase Clerk Integration Doc Pn"><figcaption></figcaption></figure>

        <figure><img src="/images/sql-editor-supabase.png" alt="Sql Editor Supabase Pn"><figcaption></figcaption></figure>

### Step 2
In Clerk: **JWT Templates \> Add Supabase**, paste JWT secret

        <figure><img src="/images/Supabase-api-key-clerk.png" alt="Supabase Api Key Clerk Pn"><figcaption></figcaption></figure>

        <figure><img src="/images/jwt-template-clerk.png" alt="Jwt Template Clerk Pn"><figcaption></figcaption></figure>

        <figure><img src="/images/jwt-template-clerk-configuration.png" alt="Jwt Template Clerk Configuration Pn"><figcaption></figcaption></figure>

### Step 3
Enable **Clerk as an authentication provider**

        Update RLS policies to use `auth.uid()` from Clerk

        Prompt Lovable to:

        

### Step 4
Confirm Clerk-issued tokens are accepted by Supabase

        <figure><img src="/images/supabase-tasks-table.png" alt="Supabase Tasks Table Pn"><figcaption></figcaption></figure>

  </Step>
  
    

### Step 1
In Lovable: **Settings \> Custom Domain**

        <figure><img src="/images/custom-domain-lovable.png" alt="Custom Domain Lovable Pn"><figcaption></figcaption></figure>

### Step 2
Enter your purchased domain (e.g. `app.yourcompany.com`)

### Step 3
Lovable auto-configures DNS (no need to leave Lovable)

### Step 4
Deploy & test your app with the new domain.

### Step 5
Done ✅ — your app is now white-labeled

  </Step>
  
</Steps>

## Bonus: Build B2B Features in Minutes

Clerk supports:

- Role-based access for organizations
- Invite flows (email-based, pre-built UI)
- Organization profile customization (logo, name)
- Multi-org switching (e.g. Slack-style)

**Ask Lovable to:**

## Tips & Troubleshooting

- **Already using Supabase Auth?** You can switch to Clerk without rewriting your app logic. Just configure JWT correctly and swap auth provider.
- **Email customization:** Clerk lets you edit all transactional email templates (waitlist, invitations, approvals).
- **Mobile login**: Clerk supports passkeys, OTP, and SMS — no extra config needed in Dev Mode.
- **Compliance**: Clerk is SOC2, HIPAA, and GDPR compliant.

## Frequently Asked Questions (FAQ)

  <details>
<summary>Can I switch from Supabase Auth to Clerk easily?</summary>
Yes. Clerk and Supabase work well together. You just need to:

    - Set up Clerk to issue JWTs
    - Add Supabase’s JWT secret in Clerk
    - Update Supabase RLS policies to use Clerk’s `auth.uid()`

    This lets you plug Clerk into an existing Supabase-backed app with minimal changes.
</details>
  <details>
<summary>Do I need to configure OAuth providers like Google or GitHub?</summary>
Only for production. In development mode, Clerk provides shared credentials for testing. For production:

    - Set up your own Google/GitHub/etc. credentials
    - Add them in Clerk under **OAuth settings**
</details>
  <details>
<summary>What’s the difference between Organizations and Users?</summary>
- **Users**: Individuals who can log in to your app
    - **Organizations**: Groups of users (teams, companies)

    Use organizations when you want:

    - Role-based access (Admin, Member, etc.)
    - Users to invite teammates
    - B2B SaaS-style flows
</details>
  <details>
<summary>What is “Impersonation Mode”?</summary>
It allows admins to log in as any user — super helpful for:

    - Debugging user issues
    - Understanding their experience
    - Providing live support

    
</details>
  <details>
<summary>Can I customize Clerk's UI components?</summary>
Yes. Clerk offers:

    - Full CSS support via `appearance` props
    - The option to build fully custom UIs using Clerk React hooks

    You can keep the out-of-the-box look or fully match your app’s brand.
</details>
  <details>
<summary>Can I email my waitlist users from Clerk?</summary>
Currently:

    - Users are auto-notified when approved from the waitlist
    - Bulk email support is **coming soon**

    For now, export emails and use your preferred email tool.
</details>
  <details>
<summary>Is Clerk free to use?</summary>
Yes\! Clerk has a generous free tier:

    - Up to **10,000 Monthly Active Users (MAUs)**
    - Paid plans start at **$25/month**, with usage-based pricing after

    You can use it in production without paying until you scale.
</details>
  <details>
<summary>Does Clerk support compliance (SOC2, HIPAA, GDPR)?</summary>
Yes. Clerk is:

    - **SOC 2 certified**
    - **HIPAA-compliant**
    - **GDPR-ready**

    Ideal for teams building in regulated industries.
</details>
  <details>
<summary>Can I use Clerk with Stripe for billing?</summary>
Coming soon. You’ll soon be able to:

    - Define plans (e.g. Free, Pro, Enterprise)
    - Let users/orgs manage subscriptions from Clerk’s UI
    - Automatically sync data to Stripe

    Follow [@clerkdev](https://x.com/clerkdev?lang=en) on X for updates.
</details>

Want a question added to this FAQ? [Let us know on Discord](https://discord.gg/lovable-dev)\!

## Final Thoughts

Clerk turns authentication into a prompt. You don’t need to build it yourself.

**With just a few clicks and prompts, your app now has:**

- Secure, scalable authentication
- Team & organization management
- Impersonation tools for debugging
- Supabase-backed data and access control
- Custom domain support for a polished UX