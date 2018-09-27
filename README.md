# Basic-Portfolio

Build a professional portfolio site using HTML & CSS

## Project Files and Folders

* Create a project folder named `Basic-Portfolio`.
* In the `Basic-Portfolio` project folder create the following directories:
    - `assets/images`
    - `assets/css`
* In the `Basic-Portfolio` project folder create the following files:
    - `index.html`
    - `contact.html`
    - `portfolio.html`
    - `assets/css/style.css`.

## Style Specifications

* **Images and locations**:
    - Save all images to the `Basic-Portfolio/assets/images/` folder.
    - For the Portfolio images, use placeholder images.
    - For the Profile image, use a picture from one of your professional online profiles.
    - For the page background pattern, consider something from [Subtle Patterns](https://www.toptal.com/designers/subtlepatterns/ "Subtle Patterns").
* **Content Area**:
    - The width of the content area on the page is not to exceed `960px`.
    - The site header, footer backgrounds, and associated borders will use the entire width of the browser.
    - The name plate and menu in the site header are bounded by the `960px` width of the content area.
    - The site footer should stick to the bottom of the page **_[Bonus]_**.
    - The content area should float between the site header and footer, and should have a minimum distance of `32px` from the site header.
    - The content area should extend for a minimum of `32px` past the end of the content, but should not extend to the site footer, **unless** that's the amount of space used by the content.
    - Buttons use the accent color for their backgrounds.
    - Headings use the accent color as the text color.
* **Colors**:
    - Accent color: `#4aaaa5` ![#4aaaa5](https://placehold.it/15/4aaaa5/000000?text=+)
    - Base text color: `#777` ![#777](https://placehold.it/15/777/000000?text=+)
    - Main Header background color: `#fff` ![#fff](https://placehold.it/15/fff/000000?text=+)
    - Main Header border color: `#ccc` ![#ccc](https://placehold.it/15/ccc/000000?text=+)
    - Footer background color: `#666` ![#666](https://placehold.it/15/666/000000?text=+)
    - The Footer top border color: `#4aaaa5` ![#4aaaa5](https://placehold.it/15/4aaaa5/000000?text=+)
    - Main content background color: `#fff` ![#fff](https://placehold.it/15/fff/000000?text=+)
    - Main content border color: `#ddd` ![#ddd](https://placehold.it/15/ddd/000000?text=+)
* **Fonts**:
    - Headings: `Georgia, 'Times New Roman', Times, serif`
    - Body: `Arial, 'Helvetica Neue', Helvetica, sans-serif`
* **Border Sizes**:
    - The Footer border is `8px`
    - The Header border is `1px`
    - The Main content box has a `1px` border.

# Project Setup Script

>**Note:**
>To execute the following, you will need to have the `hub` commanline utility installed.
>On macOS with Homebrew run `brew install hub`.

```bash
#! /usr/bin/env bash

# Define the Project Name and Folder Name.
PROJECT_NAME='Basic-Portfolio'

# Define the parent location for the project files.
BASE_DIR="${HOME}/Projects/Homework"

# Define the complete project location.
PROJECT_DIR="${BASE_DIR}/${PROJECT_NAME}"

# Make sure the parent project directory exists
mkdir -p "${BASE_DIR}"

# Change to the parent project path.
cd "${BASE_DIR}"

# Create the local Git repository for the project.
hub init -g "${PROJECT_NAME}"

# Change into the project folder.
cd "${PROJECT_DIR}"

# Create the project repository on GitHub.
hub create "${PROJECT_NAME}"

# Add the project README
echo "# Basic-Portfolio" >> README.md

# Create the project folder structure.
mkdir -p assets/{images,css}

# Create the files needed in this project.
touch {index,contact,portfolio}.html assets/css/style.css

# Add the project files to version control and push them to the GitHub
# remote repository.
git add . && git commit -m "Initial Project Setup"
git push -u origin master
```

# References

- The JavaScript snippet used to update the Copyright in the footer came from [Update Your Footer](http://updateyourfooter.com/ "Update Your Footer")

# Credits

- The profile photo was taken by my friend and fellow photographer Jeff Acker.

- Images on the Portfolio page were provided courtesy of [Lorem Picsum](https://picsum.photos "Lorem Picsum") and [Unsplash](https://unsplash.com "Unsplash").
- The following images from Lorem Picsum were used on the Portfolio page.
    - _Project_: Wire Frame
        - _Picsum Image_: [618](https://unsplash.com/photos/ypVM8PnygUo), _Author_: [Mika Ruusunen](https://unsplash.com/@mikaruusunen)
    - _Project_: Giftastic
        - _Picsum Image_: [373](https://unsplash.com/photos/i8CYGnoerR0), _Author_: [Jay Wennington](https://unsplash.com/@jaywennington)
    - _Project_: Rock, Paper, Scissors
        - _Picsum Image_: [817](https://unsplash.com/photos/ssrbaKvxaos), _Author_: [Alex wong](https://unsplash.com/@killerfvith)
    - _Project_: Train Scheduler
        - _Picsum Image_: [821](https://unsplash.com/photos/2TlAsvhqiL0), _Author_: [Eutah Mizushima](https://unsplash.com/@eutahm "Eutah Mizushima")
    - _Project_: Liri Bot
        - _Picsum Image_: [688](https://unsplash.com/photos/a_xa7RUKzdc), _Author_: [Benjamin Sloth Lindgreen](https://unsplash.com/@benjaminslothlindgreen "Benjamin Sloth Lindgreen")
    - _Project_: Word Guess
        - _Picsum Image_: [345](https://unsplash.com/photos/S_mEIfXRzIk), _Author_: [Mario Calvo](https://unsplash.com/@mariocalvo "Mario Calvo")
    - _Project_: Friend Finder
        - _Picsum Image_: [662](https://unsplash.com/photos/ILz31HBGEak), _Author_: [Caleb Ekeroth](https://unsplash.com/@calebekeroth "Caleb Ekeroth")
    - _Project_: Burger 2: The Sequel
        - _Picsum Image_: [1074](https://unsplash.com/photos/sseiVD2XsOk), _Author_: [Samuel Scrimshaw](https://unsplash.com/@samscrim "Samuel Scrimshaw")
    - _Project_: Clicky Game
        - _Picsum Image_: [366](https://unsplash.com/photos/6PF6DaiWz48), _Author_: [Rayi Christian Wicaksono](https://unsplash.com/@mumolabs "Rayi Christian Wicaksono")
    - _Project_: News Searcher
        - _Picsum Image_: [342](https://unsplash.com/photos/r4He4Btlsro), _Author_: [Steven Lewis](https://unsplash.com/@stevenlewis "Steven Lewis")
    - _Project_: News Fit to Scrape
        - _Picsum Image_: [1073](https://unsplash.com/photos/Oaqk7qqNh_c), _Author_: [Patrick Tomasso](https://unsplash.com/@impatrickt "Patrick Tomasso")

- The background image is from [Subtle Patterns](https://www.toptal.com/designers/subtlepatterns/ "Subtle Patterns").
    - The image used on this site is [White Sand](https://www.toptal.com/designers/subtlepatterns/?s=white_sand), by [Atle Mo](http://www.atlemo.com "Atle Mo").
    - The images from [Subtle Patterns](https://www.toptal.com/designers/subtlepatterns/ "Subtle Patterns") use the following [license](https://creativecommons.org/licenses/by-sa/3.0/ "Attribution-ShareAlike 3.0 Unported (CC BY-SA 3.0)")

## The Unsplash License

All photos published on Unsplash can be used for free. You can use them for commercial and noncommercial purposes. You do not need to ask permission from or provide credit to the photographer or Unsplash, although it is appreciated when possible.

More precisely, Unsplash grants you an irrevocable, nonexclusive, worldwide copyright license to download, copy, modify, distribute, perform, and use photos from Unsplash for free, including for commercial purposes, without permission from or attributing the photographer or Unsplash. This license does not include the right to compile photos from Unsplash to replicate a similar or competing service.
