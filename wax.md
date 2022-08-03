---
title: Wax integration
layout: default
nav_order: 13
---

This functionality is not avaliable in Annonatate yet. It is being worked on. I am updating the documentation as I am writing the code. This currently does not work.

# How to create a new Wax instance
1. Go to the profile page [https://annonatate.herokuapp.com/profile/](https://annonatate.herokuapp.com/profile/)
2. Scroll to "Create a new workspace" section
3. Enter the name of the wax workspace
4. Make sure "Create Wax website" is checked
5. Click "Submit" button
6. Wait for a minute for site to build
7. Switch to site in the section labeled Workspaces


# How to Integrate Wax with Existing Wax website
1. [Enable GitHub pages on your site](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)
2. Go to your repo's code page, add "annonatate-wax" to the description field.
3. Go to [annonatate.herokuapp.com/profile](annonatate.herokuapp.com/profile)
4. Under workspaces switch to the Wax workspace **This will not work, for Wax to work with Annonatate, we have to write some files, this does that.**
5. Wait a minute
6. Try switching again. It should work. Please let use know if it doesn't.


# How to Process a Collection
1. Once you are in the Wax workspace, go to the upload tab
2. Click on the tab named "Process Wax Collection"
3. Upload your images to the folder listed on this page
4. Once your image upload is finished, upload your csv file
5. Make sure your collection name matches the folder of the images you uploaded (if it doesn't the site will warn you). Enter the name in the form.
6. Press "Upload collection" button
7. Wait, this will probably take a while to process, especially if you have a large number of items
8. You are done!
