## Welcome to the CZ-Sync GitHub space 👋

The **CZ-Sync GitHub Organization** contains code repositories associated with the CZ Synchrony Working Group, which is a Powell Center working group. More details will be added as we begin working on this project.

Repo guide and organization:
- `code-sandbox` is a repo for putting test, example, or one-off code snippets
- `data-preprocessing` is a repo with a formal `targets` pipeline used to download, gather, harmonize, and munge any input data for later use in modeling. The data prepared through this repo's pipeline are pushed to Google Drive.
- `model-[domain]-[method]` refer to repos that contain modeling code (e.g. `model-streamflow-bayes`, `model-streamflow-lstm`). These repos are named following that convention to maintain organization.

### Quick example of using R code to download the Google Drive files in our Data folder 

Use this code as an example of how to pull down data from Google Drive so that you are using the most up-to-date info. Also, use code like this (or in Python) in any modeling repos so that it always starts with the same, shared data we are all working with. Note that you will have to login using the same credentials for which the CZ Synchrony Google Drive space is shared to run these commands.

```r
# Install this package if you do not already have it
library(googledrive) 

# Interatively authenticate to have access to Google Drive
drive_auth()

# Download a file
# By default, it will be downloaded with the same name to your current working directory
drive_download('ameriflux_site_info.csv')

```

<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
