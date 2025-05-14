---
title: "Integration with Replicate"
description: "Learn how to integrate Replicate with your Lovable application"
icon: "robot"
---

## What is Replicate

[Replicate](https://replicate.com/) lets you run open-source machine learning models with just a few lines of code—no ML expertise required.

It’s an API platform where developers can generate images, videos, audio, and more using community-built or custom AI models. Whether you’re building an MVP, prototyping creative features, or adding production-grade AI to your app, Replicate gives you fast, flexible access to state-of-the-art models.

## Why use Replicate with Lovable?

Replicate fits naturally into Lovable’s AI-first app-building workflow. You can:

- Generate dynamic visuals (e.g. course banners, avatars, scenes)
- Use multimodal AI (image, video, speech, text-to-speech)
- Add real-time content generation without running your own model infrastructure

With Lovable’s built-in knowledge of Replicate’s API and models, integration takes minutes—not days. Just describe what you want, and Lovable handles the rest.

## Step by Step Tutorial

In this tutorial, we walk through how to integrate Replicate into a Lovable application to dynamically generate course banner images, adding a new layer of interactivity and polish to your product. You’ll also learn how Replicate fits into Lovable’s broader AI workflow—including how to pair it with OpenAI for course content, Superbase for backend logic, and real-time AI conversations using [OpenAI’s WebRTC API](https://platform.openai.com/docs/guides/realtime#connect-with-webrtc).

### Step 1 – Build a Language Tutor App
We start by creating a Spanish-learning web app with Lovable. This includes:

    - A user login flow
    - AI-powered chat for Spanish tutoring
    - Voice recording and playback
    - Translation features

    This gives users a personalized AI tutor that they can talk to, type to, and learn with.

    <figure><img src="/images/course-dashboard.png" alt="Course Dashboard Pn"><figcaption></figcaption></figure>

### Step 2 – Generate Courses with AI
We enhance the app with AI-generated courses:

    <figure><img src="/images/course-creation-ai.png" alt="Course Creation Ai Pn"><figcaption></figcaption></figure>

    - Users define a topic (e.g., _Questions to ask at a barbecue_).
    - An OpenAI-powered function creates 10 multiple choice questions in Spanish.
    - Courses are saved to the user's account with Supabase and can be revisited anytime.
      <figure><img src="/images/course-creation-ai-2.png" alt="Course Creation Ai 2 Pn"><figcaption></figcaption></figure>
    - Users get feedback on each question with explanations.
    - Automatically generate a **course banner image** that matches the topic. Replicate uses the **Flux Schnell** model for fast image generation and dynamically inject the image into the course page.

    
### **How it Works:**
1. We call the Replicate API when a new course is created.
      2. The prompt is dynamically generated based on the course topic.
      3. Replicate returns an image URL, which is used as the banner for the course.

    <figure><img src="/images/replicate-real-time.png" alt="Replicate Real Time Pn"><figcaption></figcaption></figure>

### Step 3 – Add Visuals with Replicate
Now, let’s make things visual with Replicate.

    <figure><img src="/images/replicate-image.png" alt="Replicate Image Pn"><figcaption></figcaption></figure>

    **Example Prompt:**

    
A beautiful, educational, and engaging scene about topic in digital art style. Vibrant colors. No text on image.

    **Example Response Handling:**

    Some Replicate models return a single image URL, others return an array. Make sure your Lovable function correctly extracts the output, e.g.:

    ```
    const imageUrl = response.output[0]
    ```

### Step 4 – Use Replicate Playground for Fine-Tuning
Replicate’s Playground makes it easy to test prompts and get code snippets:

    - Tweak prompts until you're happy with the output
    - Use the API snippet generator for Node.js, Python, etc.
    - Copy-paste directly into Lovable's backend functions

    
Use Playground Beta to compare multiple outputs at once.

    <figure><img src="/images/replicate-playground.png" alt="Replicate Playground Pn"><figcaption></figcaption></figure>

### Step 5 – Real-Time Conversations with OpenAI
To simulate human conversations, we added a real-time Spanish-speaking feature using OpenAI’s WebRTC API:

    - Users can speak directly to their AI tutor.
    - The AI understands, responds, and corrects pronunciation in real time.
    - This makes language learning much more immersive and practical.

    This feature integrates smoothly with Lovable’s voice input, WebRTC handling, and frontend chat UI.

    <figure><img src="/images/course-voice-ai.png" alt="Course Voice Ai Pn"><figcaption></figcaption></figure>

## Tips & Gotchas

- **Model Output Variance**: Replicate models differ in how they return outputs. Always inspect the actual JSON returned from the playground.
- **Prompt Iteration is Key**: Small prompt changes can greatly affect image quality. Use the playground to experiment.
- **Backend Logs**: Use Supabase Edge logs to debug your API calls. Lovable supports in-app log fetching.
- **Version Control in Lovable**: Each prompt edit is auto-committed, but you can manually track checkpoints using the “Deploy” feature for production-ready states.

## FAQ

  <details>
<summary>What is Replicate, in simple terms?</summary>
Replicate is a platform that lets you run powerful machine learning models (like image or video generation) using a simple API—no need to train or host models yourself.
</details>
  <details>
<summary>Who typically uses Replicate?</summary>
Replicate is popular with indie hackers, startup builders, and large enterprises alike. Whether you're prototyping an AI feature or deploying at scale, Replicate supports both quick hacks and robust deployments.
</details>
  <details>
<summary>Do I need my own Replicate API key?</summary>
Yes. Lovable securely stores your keys and handles API calls for you once added.
</details>
  <details>
<summary>What models can I use on Replicate?</summary>
Replicate supports many modalities including:

    - Image generation (e.g. Flux Schnell)
    - Video generation
    - Audio and text-to-speech
    - Language models (though not Replicate’s main focus)
    - Custom Cog models (open-source Dockerized models you can deploy)

    Explore them all at [replicate.com/explore](https://replicate.com/explore).
</details>
  <details>
<summary>How do I know which model is right for my use case?</summary>
Use Replicate’s **Playground** to test different models before integrating them. The Playground lets you tweak prompts, compare outputs, and copy working code snippets for your app.
</details>
  <details>
<summary>What’s the difference between Replicate's old and new API endpoints?</summary>
Replicate has two API formats:

    - The original (`/predictions`) endpoint: most widely known and used.
    - The newer `/models///versions//predictions` endpoint: more efficient and flexible.

    Lovable integrates with both depending on the model’s requirements.
</details>
  <details>
<summary>What if a model returns a different JSON structure than expected?</summary>
Model outputs vary. Some return a string URL, others return an array. Use the Replicate Playground to inspect the real response and update your parsing logic accordingly.

    Example fix:

    ```
    const imageUrl = Array.isArray(output) ? output[0] : output;
    ```
</details>
  <details>
<summary>Can I trigger Replicate image generation only once, or on every course view?</summary>
You can choose:

    - **One-time generation on course creation**: Saves compute costs and creates a consistent visual identity.
    - **Dynamic generation per session**: If you want fresh visuals each time.

    In the tutorial, we chose to generate the image once when the course is first created.
</details>
  <details>
<summary>Does Lovable know how to work with Replicate out of the box?</summary>
Yes\! Lovable has built-in knowledge about Replicate and many of its popular models. It can auto-generate integration code for you using the right packages and prompt structure.
</details>
  <details>
<summary>How does Lovable handle package installation like replicate for Node.js?</summary>
Lovable automatically installs and configures packages when needed, based on your prompt and integration context. You don’t have to npm install manually unless debugging locally.
</details>
  <details>
<summary>What’s the workflow for debugging Replicate errors in Lovable?</summary>
- Use Lovable’s **Superbase Edge function logs** to trace issues.
    - If there’s a mismatch between expected vs. actual Replicate response, update your JSON handling.
    - Use the **“Fix this”** button in Lovable to retry or refactor the function logic.
</details>
  <details>
<summary>Can I checkpoint my working app state in Lovable?</summary>
Currently, every prompt change creates a commit. You can:

    - Use the **History** tab to navigate commits (including bookmarking commits)
    - **Deploy** a version to make it a production checkpoint
    - GitHub sync is available for custom version control
</details>
  <details>
<summary>How does GitHub integration work with Lovable?</summary>
You can export your Lovable project to GitHub with **two-way sync**:

    - Lovable pushes changes to GitHub
    - You (or your team) can make changes in an IDE and push back
    - Works great for frontend in Lovable \+ backend in your own editor
</details>
  <details>
<summary>What are LLM-friendly .lm.txt or .lm.md files?</summary>
These are simplified markdown-based docs optimized for language models. Replicate is actively working on adding these to help Lovable (and other tools) better understand its models automatically.
</details>
  <details>
<summary>Do I need to handle prompt tuning myself?</summary>
Yes, prompt crafting is essential. Lovable helps with auto-prompting and templating, but you should always test in the Replicate Playground to refine the inputs for best results.
</details>

## Resources

- Explore [Replicate API Docs](https://replicate.com/docs), [Replicate’s model catalog](https://replicate.com/)
- Learn more about [OpenAI Function Calling](https://platform.openai.com/docs/guides/function-calling), [OpenAI WebRTC](https://platform.openai.com/docs/guides/speech/real-time-speech)