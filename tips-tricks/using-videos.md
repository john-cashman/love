---
title: Using Videos
description: >-
  Learn how to embed videos in your projects using external links or GitHub
  uploads
icon: film
---

# Using Videos

Lovable offers two methods for embedding videos into your projects. Below, we’ll cover both options step by step:

<details>

<summary>Linking to an external video</summary>



</details>

<details>

<summary>Using a video from your GitHub public folder</summary>

```
You can upload videos to your project’s GitHub repository and reference them directly. Here’s how:

```

#### Connect your GitHub repository

First, make sure your project is linked to a GitHub repo. [Here’s how to set up your repo](https://docs.lovable.dev/integrations/git-integration).

#### Access the public folder

Inside your connected repository, navigate to the `public` directory. This folder is specifically used for hosting project assets like images, videos, and other media.

#### Upload a video

You can now add your video to the public folder by either dragging and dropping it or clicking **"choose your files"** to browse and upload the file from your local machine.

#### Commit the file

After selecting your video file, enter a brief commit message (e.g., "Adds a Mars video to be used in the app") and click **"Commit changes"**.

<figure><img src="../assets/using-videos-github-commiting.png" alt="Committing video file"><figcaption></figcaption></figure>

#### Get the video path

Once the upload is complete, click on the video file and use the copy icon :octicons-copy-16: to copy its path. You’ll need this path in the next step.

<figure><img src="../assets/using-videos-github-selecting.png" alt="Copy video file path"><figcaption></figcaption></figure>

#### Reference the video in Lovable

Now, you can embed the video by specifying the file path in your prompt. For example, you can use a prompt like this one:

```
    Ensure you use the exact file path you copied earlier.

To see these methods in action, explore one of the example projects: [Lovable using videos example project](https://lovable.dev/projects/380835ab-c8d7-4f45-9b0d-51ec04294457). You’ll find real prompts demonstrating how videos are integrated using both methods.

Additionally, for a more technical look at the video adding process, check out this public repository: [GitHub: Video Upload Example](https://github.com/viborc/adding-videos-example). It includes the video upload and the implementation details used in the project.
```

</details>
