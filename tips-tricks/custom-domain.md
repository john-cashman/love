---
title: "Custom domain"
description: "Add your own domain to any Lovable site app."
icon: "earth-europe"
---

When you create a project, Lovable makes it easy to [publish it](../features/deploy) with the click of a button.

By default, your Lovable app is accessible via a Lovable staging subdomain (e.g., `yoursite.lovable.app`). However, you can connect your site to a custom domain (e.g., `yourdomain.com`) or a subdomain (e.g., `subdomain.yourdomain.com`) that you own.

Using a custom domain enhances your brand, improves [SEO](https://docs.lovable.dev/tips-tricks/seo) discoverability, and makes your site easier to find and remember.

If you want to have a custom domain, see below.

## Using Entri

To connect a custom domain, navigate to **Project \> Settings \> Domains** in Lovable.

### Requirements

- A **paid Lovable plan** is required to connect a custom domain.
- You **must own** a domain before proceeding. If you don’t have one, you can purchase it from a domain provider such as:
  - [Namecheap](https://www.namecheap.com)
  - [GoDaddy](https://www.godaddy.com)
  - [View full list of domain providers](https://developers.entri.com/provider-list)

Lovable uses [**Entri**](https://www.entri.com/) to facilitate quick and seamless domain connections.

### Step-by-Step Guide

### Step 1
Navigate to **Project \> Settings \> Domains** and click **Connect Domain**.

    <figure><img src="/images/project-setting.png" alt=""><figcaption></figcaption></figure>

### Step 2
Click **Continue**.

### Step 3
Enter the domain you want to connect (e.g., `yourdomain.com`).

    <figure><img src="/images/connect-entri.png" alt=""><figcaption></figcaption></figure>

### Step 4
Click **Continue**.

### Step 5
Search for and select your **DNS provider** (the service where you purchased your domain).

    <figure><img src="/images/dns-provider.png" alt=""><figcaption></figcaption></figure>

    
Domain providers are amongst many: _123-Reg, Amazon Route 53, arsys, Aruba IT, Bluehost, Cloudflare, Crazy Domains, DigitalOcean, DNSimple, Domain.com, DreamHost, Dynadot, EasyDNS, Enom, Gandi, Hetzner, Home PI, HostGator, Hostinger, Hover, Inmotion Hosting, IONIS, iwantmyname, Localweb, Name.com, NameBright, Namecheap, NameSilo, Netlify, Network Solutions, One.com, OpenSrs, OVH Global, Porkbun, Register.com, Register.it, Registro, Shopify, SiteGround, Spaceship, Strato, TransIP, United Domains DE, Web.com, WordPress and Xneelo._

### Step 6
Follow the on-screen instructions to **sign in to your DNS provider** and authorize the connection to [Entri](https://www.entri.com/).

### Step 7
Click **Close Window** to complete the connection and return to **Site Settings**.

### Step 8
Click **Done**.

    
DNS changes may take up to **48 hours** to propagate globally, though most updates occur within a few hours.

### You're All Set! 🎉 
Your Lovable app is now available on your custom domain.

  <details>
<summary>My custom domain is connected, but my site isn’t live. What should I do?</summary>
DNS propagation can take up to **48 hours** due to factors such as TTL (Time to Live) and internet service provider delays. If your site isn’t live yet:

    - Wait a bit longer for DNS changes to fully update.
    - Use a tool like [whatsmydns](https://www.whatsmydns.net/) to check the status of your DNS records.
    - Clear your browser cache to ensure you’re viewing the latest version of your site.
</details>
  <details>
<summary>My site isn’t appearing after 48 hours. What now?</summary>
- Double-check that your **DNS records** are correctly set in your domain provider’s settings.
    - If issues persist, contact your **domain provider’s support team**.
    - If your DNS settings are correct but the site still doesn’t load, reach out to **Lovable’s customer support** for assistance.
</details>
  <details>
<summary>Can I buy a domain through Lovable?</summary>
For this launch, Lovable will **not** support buying domains. We may launch domain purchasing later if these issues are resolved.
</details>
  <details>
<summary>How does connecting a custom domain impact my site's SEO?</summary>
Using a custom domain improves your site's SEO by enhancing brand credibility, allowing for better indexing by search engines, and enabling features like custom meta tags and structured data. For more SEO tips, visit [Lovable SEO Guide](https://docs.lovable.dev/tips-tricks/seo).
</details>
  <details>
<summary>How to remove a custom domain?</summary>
1. Access the **Project \> Settings \> Domains.**
    2. Click "Remove domain" next to your custom domain.
    3. Remove the DNS records fro your domain provider.
</details>

## Using Netlify

You can host on Netlify for free with a custom domain.

### Step-by-Step Guide

### Step 1
Ensure that your project is successfully transferred to GitHub. In the Lovable editor, click on "Transfer to GitHub" located in the top right corner.

### Step 2
Head over to Netlify and log in using your GitHub credentials.

### Step 3
In Netlify, you'll need to follow these simple steps: Click on "Import from Git" \> Authorize Netlify to access your GitHub repositories \> Select your Lovable repository from the provided list \> Click "Deploy"

### Step 4
Let's proceed to configure your custom domain directly within Netlify: Go to "Domain Management" \> Click "Add a domain" \> Enter your domain name \> Click "Verify" \> Follow the DNS configuration prompts

### Step 5
Your Lovable app will automatically redeploy to Netlify whenever you make changes in Lovable.

You will need to bring an existing domain or purchase one.

## Using Vercel

### Step-by-Step Guide

### Create a Github repository
Open your project in Lovable and click GitHub then "create repository" if you haven't already done so. This will commit your code to the `main` branch and create a repository. Once you do this, all changes made to code in your app will automatically be commited to your Github repository on each change.

### Set up Vercel
Go to the [Vercel website](https://vercel.com/) and create an account. Configure your domain and set the necessary GitHub permissions (make sure to handle DNS settings properly).

### Automatic deployments
Vercel will automatically deploy the latest changes from the `main` branch each time it is updated. You can make one or two small changes to your app on Lovable and then visit Vercel deployments to ensure updates are being redeployed from `main`. Once confirmed, do the next step:

### Create a Development branch
In your GitHub repository settings in Lovable, commit all new changes to a second branch called `dev` (or whatever you want).

### Configure Vercel Builds
Go back to Vercel and adjust your settings to ensure it only builds production deployments from the `main` branch.

### Make changes in Development
Work on your app in the Lovable. Any changes will go to the `dev` branch now and wont automatically be deployed via Vercel.

    <figure><img src="https://github.com/user-attachments/assets/08f6cd18-5d12-44da-a2cf-c07687eeab44" alt="image"><figcaption></figcaption></figure>

### Deploy new changes
When you're ready to push new changes to your domain, go to GitHub and perform a pull request from `dev` to `main`. Once you complete and merge the pull request, Vercel will automatically deploy the updates in about one minute.

    <figure><img src="https://github.com/user-attachments/assets/77244d5d-f9e1-4e5b-b372-5e1ea4003d63" alt="image"><figcaption></figcaption></figure>

### Notes

- If you hit the 100/day deployment limit in Vercel (it builds your `dev` branch but doesn't deploy it). You can ask Lovable chat to build you vercel.json file which will force Vercel to not build development builds at all.

  <figure><img src="https://github.com/user-attachments/assets/1b29581f-0942-432b-af30-71be43a921db" alt="image"><figcaption></figcaption></figure>
- **Supabase Consideration**: Currently, you can only utilize one Supabase instance. So, if you make extensive SQL changes, it could potentially break production. Unfortunately, we can't yet provide specific guidelines for this scenario as it's complex. Frequently test your production environment if you make changes related to Supabase.

## Using Namecheap

### Step-by-Step Guide

### Transfer Your Lovable Project to GitHub
First, you need to transfer your Lovable project to GitHub if you haven't already done so.

    In your Lovable project, click on the "Transfer to GitHub" button at the top of the interface.

    
This step is required before proceeding with the custom domain setup.

### Purchase a Domain from Namecheap
Start by acquiring your domain (e.g., mysimpledomain.com) from [Namecheap](https://www.namecheap.com/).

### Access Advanced DNS Settings
Navigate to the [Advanced DNS](https://ap.www.namecheap.com/Domains/DomainControlPanel/mysimpledomain.com/advancedns) settings for your domain.

### Configure DNS Records
Add the following DNS records to your domain configuration:

    <figure><img src="/images/dns-record.png" alt="DNS record"><figcaption></figcaption></figure>

### Set Up GitHub Workflow
Create a GitHub workflow file for deployment:

    ```
    name: Deploy to GitHub Pages
    
    on:
      workflow_dispatch:
    
    jobs:
      deploy:
        runs-on: ubuntu-latest
        steps:
          - uses: actions/checkout@v3
    
          - uses: actions/setup-node@v3
            with:
              node-version: '18'
    
          - run: npm install
    
          - run: npm run build
    
          - name: Copy index.html to 404.html
            run: cp dist/index.html dist/404.html
    
          - name: Debug build output
            run: |
              echo "Listing contents of the root directory..."
              ls -la
              echo "Listing contents of the dist directory..."
              ls -R dist
    
          - name: Deploy to GitHub Pages
            uses: peaceiris/actions-gh-pages@v3
            with:
              github_token: ${}
              publish_dir: ./dist
              cname: mysimpledomain.com
              force_orphan: true
    ```

### Generate GitHub Access Token
Create a classic token at [GitHub](https://github.com/settings/tokens):

    Keep the token page open—you'll need it for the next step.

### Add Repository Secret
Add your token as a repository secret named `GH_PAT`.

### Configure GitHub Pages
Navigate to your repository's GitHub Pages settings and:

    - Select Build from a branch
    - Choose the gh-pages branch
    - Save the settings

### Run the GitHub Workflow
Your website will be updated each time you run the GitHub workflow:

    1. Go to your repository's Actions page
    2. Select the Deploy to GitHub Pages workflow
    3. Click Run workflow button
    4. This will publish the latest version of your GitHub repository to your custom domain

### You're All Set! 🎉 
Your Lovable app is now available on your custom domain.

For more information, you can check out [this site](https://custom-domain.lovable.app/).