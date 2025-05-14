---
title: "Using images in Lovable"
description: "Learn how to add images to your Lovable projects"
icon: "frame"
---

To add images you can do one of four things:

  <details>
<summary>Upload the image to the prompt chat</summary>
Simply upload them in the chat and explain to Lovable’s AI where and how you’d like them to appear in your project.

    

</details>
  <details>
<summary>Replace it on the visual editor</summary>
You can replace an existing image directly using the [visual editor](https://docs.lovable.dev/features/precision-edit#visual-edits) functionality: 

    

### Step 1
Click on "Edit" tool.

### Step 2
Select the image holder you would like to change.

        <figure><img src="/images/visual-edit-replace.png" alt="images/visual-edit-replace.png"><figcaption></figcaption></figure>

### Step 3
Change the image.

        <figure><img src="/images/visual-edit-image.png" alt="images/visual-edit-image.png"><figcaption></figcaption></figure>

</details>
  <details>
<summary>Using an external image URL</summary>
One way to add images to your project is by referencing an image from an external URL. This method allows you to use images hosted on external platforms like Unsplash, Imgur, or any other image-hosting service. Be mindful of use copyrights\!

    Here’s how to prompt Lovable to use an external image:

    

### Step 1
Find the image you want to use.

        For example, you can visit a site like Unsplash, select an image, and copy its URL.

### Step 2
In your project prompt, simply tell Lovable to use that image by specifying the URL. For example:

        ```
        Use the image from this URL 
        https://upload.wikimedia.org/wikipedia/commons/thumb/7/73/Pale_Blue_Dot.png/442px-Pale_Blue_Dot.png 
        for the hero section image.
        ```

</details>
  <details>
<summary>Using images from your GitHub public directory</summary>
Another method to add images to your Lovable project is by using images uploaded to the `public` directory of your connected GitHub repository. Here’s how you can do it:

    

### Connect your GitHub repository
Ensure your project is connected to your GitHub repo. [Here's how to connect your repo](https://docs.lovable.dev/integrations/git-integration).

### Locate the public folder
Inside your GitHub repository, navigate to the `public` directory. This folder is typically used for hosting assets like images that can be referenced in your project.

### Add file
Click on **Add file** and then from a dropdown, select **Upload files** option.
        <figure><img src="/assets/using-images-github-upload.png" alt="Selecting files for upload"><figcaption></figcaption></figure>

### Upload an image
The next step is to transfer your image to your repo:

        - Drag and drop the image into the public folder, or
        - Click on the **"choose your files"** link to browse and select the image file.
          <figure><img src="/assets/using-images-github-commiting.png" alt="Selecting files for upload"><figcaption></figcaption></figure>

### Commit the changes
After selecting your image, write a simple commit message (e.g., "Adding image files to be used in the app") and click **"Commit changes"** to save the file to your repo.

### Get the image path
Once the file is uploaded, select it and then click on the copy icon next to the file name to copy the image’s path. This path will be used in your Lovable prompt.
        <figure><img src="/assets/using-images-github-selecting.png" alt="Selecting files for upload"><figcaption></figcaption></figure>

### Use the image in Lovable
You can now reference this image in your project by using a prompt like the following:

        ```
        Add an additional image to the hero section. 
        This time, use this one from my local repo: public/c-64-close-up.jpg.jpeg
        ```

        Be sure to use your image name and path you copied in the previous step.

        

    To help you better understand how to integrate images using the methods outlined above, we have a project you can explore: [Lovable Project Example](https://lovable.dev/projects/e823fedf-238d-4313-86a8-1fd4bfc2a9ba). In this project, you can see the actual prompts and how each method works in practice.

    Additionally, here's a public GitHub repository that includes the commits, uploaded images, and full implementation details. You can view the repository here: [GitHub: Adding Images Example](https://github.com/viborc/adding-images-example).

    Feel free to explore the project and repository to deepen your understanding and improve your implementation skills.
</details>