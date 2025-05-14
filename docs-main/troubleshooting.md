---
title: "Troubleshooting"
description: "Actionable steps to resolve issues in your development lifecycle."
icon: "toolbox"
---

## "Try to Fix" error loops

Building with Lovable makes coding faster and more intuitive—but even the best AI development tools can occasionally hit a snag. Sometimes your code won't run as expected, or you might notice unexpected behavior where the AI interprets your intent incorrectly.

Here's a step-by-step guide to help you navigate issues and get back on track:

### Use the Try to Fix Button First
Click the **Try to Fix** button when an error shows up. Lovable will scan your logs, detect the issue, and attempt a quick fix. It's your fastest first move. If that doesn't work, it's time to dig deeper.

### Diagnose Unexpected Behavior
Your code may run without errors but not behave as intended. That's **unexpected behavior**—harder to spot and harder to fix. Try this:

    - **Review your original prompt** to confirm your instructions.
    - **Break it down**: Check individual components and logic.
    - **Add visuals**: Use screenshots to clarify what went wrong.

### Write More Effective Prompts
Clear, structured prompts lead to better results. Use this format:

    1. **Project Overview** – What are you building?
    2. **Page Structure** – List key pages/components.
    3. **Navigation Logic** – Describe user flow.
    4. **Visual Aids** – Upload wireframes or screenshots.
    5. **Implementation Steps** – Lay out the build order.

### Build in Logical Order
Structure matters. Follow this recommended flow:

    1. Create layout and pages.
    2. Connect Supabase or your backend.
    3. Set up authentication and user roles.
    4. Plan and organize feature logic.
    5. Prompt Lovable to implement features.

### Use Chat Mode for Clarity
When unsure, switch to **Chat Mode**:

    - Ask Lovable to **analyze your project state**.
    - Request a **recap of attempted solutions**.
    - Prompt for **new directions** to solve persistent problems.

### If You're Still Stuck: Advanced Tactics
Still no luck? Try this:

    - **Be exact** – Describe the bug and your expectations clearly.
    - **Use images** – Screenshots or videos help illustrate problems.
    - **Ask directly** – "What else can we try?"
    - **Rollback** – Restore to a working version and rebuild incrementally.

## What's Going Wrong? Common Troubleshooting Areas

Troubleshooting generally falls into these categories:

1. **UI or Layout Glitches**
2. **API or Backend Issues**
3. **Prompt Misinterpretations**
4. **AI Unresponsiveness or Misbehavior**
5. **Platform or Integration Errors**

Use the accordions below to identify specific issues and actions:

### General issues

  <details>
<summary>Need a fast diagnosis?</summary>
Jump into Chat-Only Mode and type: "Something's off. Can you walk me through what's happening and what you've tried?"
</details>
  <details>
<summary>UI or Layout Problems</summary>
- Check component hierarchy and styles.
    - Use screenshots to explain visual bugs.
    - Prompt Lovable with: "Why is this element misaligned? Fix it."
</details>
  <details>
<summary>When completely stuck</summary>
- Prompt: "Take a step back. Analyze the error and suggest a different approach."
    - Break the task into smaller parts.
    - Use the revert button if errors persist.
</details>
  <details>
<summary>Code sandbox error</summary>
This should not happen. Please report it to the support team.
</details>
  <details>
<summary>Not found preview or spinning up sandbox</summary>
Try a hard refresh. If unresolved, contact support.
</details>

### AI Reliability

  <details>
<summary>Avoiding AI mistakes in prompt engineering</summary>
- Keep prompts clear and structured.
    - Use reverse meta prompting.
    - Test in Chat-Only Mode before applying big changes.
</details>
  <details>
<summary>AI not responding</summary>
This shouldn't happen. Please report it to the support team.
</details>
  <details>
<summary>Persistent Fix error loops</summary>
Adjust your prompt to help the AI understand your goal or ask for step-by-step debugging help.
</details>
  <details>
<summary>Refactor broke everything</summary>
Make small, incremental changes. If the issue persists, roll back to a stable version or debug in chat.
</details>
  <details>
<summary>Error loops, hallucinations, or broken logic</summary>
Revert to a stable version and provide more context in your next prompt. Use visual editor or attach a knowledge file.
</details>
  <details>
<summary>AI not doing changes</summary>
The AI might be editing the wrong files or misinterpreting. Be very specific or edit manually.
</details>
  <details>
<summary>Chat mode not responding or incomplete</summary>
This was fixed by engineering. Please report if it happens again.
</details>
  <details>
<summary>Unexpected Crashes, Errors, or Loops</summary>
- Don't retry the same prompt. Simplify or rephrase.
    - Ask: "What fixes have we already tried?"
    - Rebuild from a previous working state.
</details>

### Core functionalities

  <details>
<summary>Preview is white</summary>
- Likely a runtime error. Check browser console logs.
    - Use chat to troubleshoot.
    - Try a hard refresh or revert.
</details>
  <details>
<summary>Rollback fails</summary>
Report to the support team if you can't revert your project.
</details>
  <details>
<summary>Unpublish or deactivate projects</summary>
This action isn't currently supported.
</details>
  <details>
<summary>Kicked out of project</summary>
This issue has been resolved. Report it if it recurs.
</details>
  <details>
<summary>Remix doesn't work (no Supabase connection)</summary>
Shouldn't happen. Contact support.
</details>
  <details>
<summary>Loading profile error</summary>
Shouldn't happen. Report to the support team.
</details>
  <details>
<summary>Email unsubscribe not working</summary>
This is a serious issue likely related to our email provider. Contact support immediately.
</details>
  <details>
<summary>Unexpected logout or access loss</summary>
Reach out to support directly.
</details>
  <details>
<summary>Challenges with larger projects</summary>
- Break up large changes into smaller steps.
    - Restart your browser if it slows down.
    - If it persists, report your use case to support.
</details>

### Domain Issues

  <details>
<summary>Custom Domain Setup</summary>
To connect your custom domain to your Lovable app:

    1. Navigate to Project → Settings → Domains in Lovable
    2. Click "Add Domain" and enter your domain name
    3. Update your DNS settings as instructed
    4. Wait for DNS propagation (can take up to 48 hours)

    
</details>
  <details>
<summary>DNS Configuration</summary>
Example DNS settings for your domain registrar:

    ```
    # For apex domain (example.com):
    Type: A
    Name: @
    Value: 76.76.21.21
    
    # For www subdomain:
    Type: CNAME
    Name: www
    Value: yourapp.lovable.app
    ```

    #### **DNS Settings Explanation:**

    - **A Record:** Points your root domain to Lovable's IP address
    - **CNAME Record:** Creates an alias from www to your Lovable app
    - **TTL (Time-to-Live):** Set to 3600 (1 hour) or lower for faster propagation

    #### **DNS Verification:**

    To verify your DNS settings are correct, you can use:

    - [**<u>DNSChecker.org</u>**](https://dnschecker.org/)
    - [**<u>MXToolbox</u>**](https://mxtoolbox.com/)
    - Command line: `dig example.com` or `nslookup example.com`
</details>
  <details>
<summary>SSL Certificate Issues</summary>
Lovable automatically provisions SSL certificates for custom domains. If you're experiencing SSL issues:

    - Ensure your DNS is properly configured
    - Check if your domain has CAA records that might restrict certificate issuance
    - Wait up to 24 hours for the certificate to be issued
    - Verify your browser isn't caching an old certificate
    - Check for certificate transparency logs to see if a certificate was issued
    - Contact Lovable support if issues persist

    #### **Common SSL Errors:**

    - **ERR_CERT_COMMON_NAME_INVALID:** Domain doesn't match certificate
    - **ERR_CERT_AUTHORITY_INVALID:** Certificate not trusted by browser
    - **SEC_ERROR_UNKNOWN_ISSUER:** Certificate issuer unknown
    - **SSL_ERROR_BAD_CERT_DOMAIN:** Domain doesn't match certificate

    
</details>
  <details>
<summary>Deployment Process</summary>
To deploy your Lovable app:

    1. Click the "Publish" button in the top-right corner
    2. Wait for the build process to complete
    3. Your app will be available at [yourapp.lovable.app](http://yourapp.lovable.app)
    4. Review deployment logs for any issues

    #### **Deployment Strategies:**

    - **Preview Deployments:** Test your app before publishing to production
    - **Automatic Deployments:** Configure your project to deploy automatically on Git changes
    - **Rollbacks:** Revert to previous versions if needed
</details>
  <details>
<summary>Removing Lovable Badge</summary>
To remove the Lovable badge from your deployed app:

    1. Go to Project Settings
    2. Find "Show Lovable Badge" option
    3. Toggle it off (requires paid plan)
    4. Redeploy your application

    
</details>
  <details>
<summary>Published version not showing latest version</summary>
Current workaround is user having to add both the domain as well as [www](http://www). domain counterpart to get the updates to sync.
</details>

### Supabase issues

  <details>
<summary>Error with Edge Functions</summary>
- **l Scope:** Use the principle of least privilege for all credentials

    When using Lovable with Supabase, always store sensitive API keys as Supabase Edge Function secrets rather than environment variables or in source code.
</details>
  <details>
<summary>Setting Environment Variables</summary>
Double-check syntax and variable names. See the [Supabase docs](https://supabase.com/docs).
</details>
  <details>
<summary>Supabase connection is lost</summary>
Disconnect and reconnect. Might be caused by an integration update.
</details>
  <details>
<summary>Remix does not work with Supabase</summary>
Remixing is blocked for Supabase-connected projects for security reasons.
</details>
  <details>
<summary>Project not found</summary>
Please report to support.
</details>
  <details>
<summary>HTTP Fetch failures</summary>
Usually means a backend server isn't responding. Use chat mode to debug.
</details>
  <details>
<summary>Connecting Supabase</summary>
To connect your Lovable project to Supabase:

    1. Click the Supabase menu in the top right of the editor
    2. Select "Connect to Supabase"
    3. Follow the prompts to connect to your Supabase project
    4. Once connected, Lovable can see your tables, RLS policies, and functions
</details>

### Stripe issues

  <details>
<summary>Stripe error</summary>
Try a different card or payment method. Contact support if unresolved.
</details>
  <details>
<summary>Two active subscriptions</summary>
Don't worry—support can easily fix this.
</details>
  <details>
<summary>Cancel your subscription</summary>
Go to your settings and cancel via Stripe account.
</details>

### GitHub issues

  <details>
<summary>Can't push to GitHub</summary>
You may have deleted your repo. [Restore it here](https://docs.github.com/en/repositories/creating-and-managing-repositories/restoring-a-deleted-repository).
</details>
  <details>
<summary>Branches are broken</summary>
Branch switching is experimental. Use at your own risk.

    Once connected to GitHub, you can work with different branches:

    #### **Branch Switching Steps**

    ```
    # To switch from main to dev:
    1. In Dev Mode, open the Git panel
    2. Select the branch dropdown
    3. Choose "dev" or click "Create new branch" if it doesn't exist
    4. Your workspace will update to reflect the selected branch
    ```

    
    #### **Branch Management:**

    - **Create a new branch:** Click "Create new branch" in the Git panel
    - **Delete a branch:** Use the GitHub interface (not available directly in Lovable)
    - **Default branch:** Set in GitHub repository settings

    If you can't switch branches:

    - Commit or stash any uncommitted changes
    - Check if you have untracked files that would be overwritten
    - Try refreshing the Lovable editor
</details>
  <details>
<summary>Repository sync issues</summary>
- Check your [GitHub permissions](https://docs.lovable.dev/integrations/git-integration).
    - Use rollback to undo unwanted changes.
</details>
  <details>
<summary>Deleted repository, now nothing works</summary>
[Restore your GitHub repo](https://docs.github.com/en/repositories/creating-and-managing-repositories/restoring-a-deleted-repository).
</details>
  <details>
<summary>Connecting GitHub</summary>
To connect your Lovable project to GitHub:

    1. Click the GitHub button in the top right of the editor
    2. Authorize Lovable to access your GitHub account
    3. Choose whether to create a new repository or use an existing one
    4. Follow the prompts to complete the connection

    #### **Repository Access Levels:**

    When connecting Lovable to GitHub, you can choose different access levels:

    - **All repositories:** Access to all your GitHub repositories
    - **Only select repositories:** Choose specific repositories to connect

    
</details>
  <details>
<summary>Authentication Issues</summary>
If you're having trouble with GitHub authentication:

    - Reconnect your GitHub account in Lovable
    - Check if your GitHub access token has expired
    - Verify you have the necessary permissions for the repository
    - Ensure two-factor authentication isn't blocking access
</details>
  <details>
<summary>Failed Pushes</summary>
If your push is rejected:

    1. Pull the latest changes from the remote repository
    2. Resolve any conflicts
    3. Try pushing again
    4. If still failing, check if the branch is protected
</details>
  <details>
<summary>Branches are broken</summary>
This is an experimental feature. Expect occasional instability.
</details>
  <details>
<summary>Deleted your repository</summary>
[Restore your GitHub repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/restoring-a-deleted-repository).
</details>

### Need more help?

Still stuck? Try this:

1. Use [Chat Mode](https://lovable.dev/chat) for step-by-step help.
2. Submit a bug through our [Feedback Portal](https://feedback.lovable.dev/).
3. If you're a paid customer, contact [Support](https://lovable.dev/support).

## Comprehensive Debugging Manual

[This document](https://docs.google.com/document/d/1dfIy5rtkPN9Zi4smX1VAbfbhAiEyBvVw8p7B8kJiEVs/edit?tab=t.0) or [this website](https://kb-lovable.netlify.app/?tab=errors#errors) were written by a Lovable power user in our Discord community.

### How to use it

1. **Download** it as `Comprehensive_Debugging_Manual.md`.
2. **Upload** it to your GitHub project.
3. Prompt Lovable: "Read this document. Let me know if it helps. Then create a prompt I should use to troubleshoot this issue."
4. After Lovable responds, say: "Before you proceed, explain in detail why you think this will work. Wait for my approval."

This ensures deeper understanding before implementing any fix.