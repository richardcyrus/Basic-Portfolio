# Basic-Portfolio

Build a professional portfolio site using HTML/CSS

# Project Files and Folders

* Create a project folder named `~/${PROJECT_BASE_DIR}/Basic-Portfolio`.
* In the project folder create the following directories:
    - `~/${PROJECT_BASE_DIR}/Basic-Portfolio/assets/images`
    - `~/${PROJECT_BASE_DIR}/Basic-Portfolio/assets/css`
* In the project folder create the following files:
    - `~/${PROJECT_BASE_DIR}/Basic-Portfolio/index.html`
    - `~/${PROJECT_BASE_DIR}/Basic-Portfolio/contact.html`
    - `~/${PROJECT_BASE_DIR}/Basic-Portfolio/portfolio.html`
    - `~/${PROJECT_BASE_DIR}/Basic-Portfolio/assets/css/style.css`.

# Style Specifications

* **Images and locations**:
    - Save all images to the `~/${PROJECT_BASE_DIR}/Basic-Portfolio/assets/images/` folder.
    - For the Portfolio images, use placeholder images.
    - For the Profile image, use a picture from one of your professional online profiles.
    - For the page background pattern, consider something from [Subtle Patterns](https://www.toptal.com/designers/subtlepatterns/ "Subtle Patterns").
* **Content Area**:
    - The width of the content area on the page is not to exceed `960px`.
    - The site header and footer backgrounds and borders will use the entire width of the browser.
    - The Name Plate and menu in the site header are bounded by the `960px` width of the content area.
    - The site footer should stick to the bottom of the page.
    - The content area should float between the site header and footer, and should have a minimum distance of `16px` from the site header.
    - The content area should extend for a minimum of `32px` past the end of the content, but should not extend to the site footer, **unless** that's the amount of space used by the content.
    - Buttons use the accent color for their backgrounds.
    - Headings use the accent color as the text color.
* **Colors**:
    - Accent color: `#4aaaa5`
    - Base text color: `#777`
    - Main Header background color: `#fff`
    - Main Header border color: `#ccc`
    - Footer background color: `#666`
    - The Footer top border color: `${accent_color}`
    - Main content background color: `#fff`
    - Main content border color: `#ddd`
* **Fonts**:
    - Headings: `Georgia, 'Times New Roman', Times, serif`
    - Body: `Arial, 'Helvetica Neue', Helvetica, sans-serif`
* **Border Sizes**:
    - The Footer border is `8px`
    - The Header border is `1px`
    - The Main content box has a `1px` border.

# Scripted Project Setup

>**Note:** To execute the following, you will need to have the `hub` commanline utility installed. On macOS with Homebrew run `brew install hub`.

```bash
#! /usr/bin/env bash

# Define the Project Name and Folder Name.
PROJECT_NAME='Basic-Portfolio'

# Define the parent location for the project files.
BASE_DIR="${HOME}/BootCampProjects/GitHub"

# Define the complete project location.
PROJECT_DIR="${BASE_DIR}/${PROJECT_NAME}"

# Make sure the parent project directory exists
mkdir -p "${BASE_DIR}"

# Change to the parent project path.
cd "${BASE_DIR}"

# Create the Git repository for the project, and setup the capability to
# push changes to GitHub.
hub init -g ${PROJECT_NAME}

# Change into the project folder.
cd "${PROJECT_DIR}"

# Create the project folder structure.
mkdir -p assets/{images,css}

# Create the files needed in this project.
touch {index,contact,portfolio}.html assets/css/style.css

# Add the project files to version control and push them to the GitHub
# remote repository.
git add . && git commit -m "Initial Project Setup"
git push origin master
```

# References

- The JavaScript snippet used to update the Copyright in the footer came from [Update Your Footer](http://updateyourfooter.com/ "Update Your Footer")
