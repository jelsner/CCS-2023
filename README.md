# CCS-2023

This repo contains all the notes for Climate Change & Storms, Florida State University, Spring 2023

## Contact information

Professor James B. Elsner (he/his/him)

Bellamy Room 314

Lesson hours MW 3:05-4:20 p.m.

Student hours TR 9:15-10:30 a.m.

[jelsner\@fsu.edu](mailto:jelsner@fsu.edu){.email}

This course is for students who want to learn more about the relationships between climate change and Earth's most powerful storms through the analysis and modeling of data

All the course slides are available on GitHub

## Class structure

Each class period I will prepare a small set of slides using [Quarto](https://quarto.org/). Quarto is an open-source scientific publishing system

Quarto allows me to weave together narrative text and code to produce formatted output. Quarto documents are reproducible

The slides (`_.qmd` files) are available on GitHub. The slide files are opened using an application called RStudio

In-person lessons will be held in this room (Bellamy 208)

## Do this 1st

-   Download and install Quarto by going to <https://quarto.org/docs/get-started/>

## Do this 2nd

-   Download and install {{< fa brands r-project >}} by going to <https://cloud.r-project.org/>
-   If you are using {{< fa brands windows >}}: Click on *Download R for Windows*, then click on *base*, then click on the *Download* link
-   If you are using a {{< fa brands apple >}}: Click on *Download R for (Mac) OS X*, then under *Latest release:* click on *R-X.X.X.pkg*, where R-X.X.X is the version number. If you have the newer Mac with the Apple silicon chip (M1) use the *R-X.X.X-arm64.pkg*
-   For example, the latest version of {{< fa brands r-project >}} as of November 18, 2022 is R-4.2.2

## Do this 3rd

-   Download and install RStudio desktop by going to <https://posit.co/download/rstudio-desktop/> *Step 2:*
-   Scroll down to find your computer's operating system and select the appropriate file to download
-   Click on the downloaded file to install

## Do this 4th

-   [Install Git](https://happygitwithr.com/install-git.html)
-   [Configure Git](https://happygitwithr.com/hello-git.html)

## Do this 5th

-   Go to <https://github.com/>
-   Click on `Sign up`
-   Enter your email, Create a password, Enter a username 
-   Solve the puzzle
-   Enter the code sent to your email
-   How many team members: 1, Student
-   Collaborative coding
-   Continue for free

## Do this 6th

-   Go to <https://github.com/jelsner/>
-   Click on the link `jelsner/CCS-2023`
-   In the upper right click on scroll down arrow next to `Fork`
-   Add your name (no spaces) to the `Repository name`
-   Click on the green `Create fork`

## Do this 7th

-   Open RStudio. You should now see a `Git` tab
-   Under `File` > `New Project` select `Version Control`
-   Select `Git`
-   Repository URL: `https://github.com/[your GitHub username]/CCS-2023-[your name].git`
-   Project directory name: `CCS-2023-[your name]`
-   Create a project as a subdirectory of: <Browse to Desktop>
-   Select Create Project

## At the start of each class 

-   Go to `https://github.com/[your GitHub username]`
-   Select the `Sync fork` button under the green `Code` button
-   Click `Update branch`
-   Open the Folder `CCS-2023-[your name]` on your Desktop
-   Open the file `CC-2023.Rproj`
-   Under the `Git` tab select blue arrow (pointing down) to `Pull` down changes from your GitHub
-   Select the `XX-name-of-lesson.Rmd` file
-   Add your own notes to the file and/or `Render`

## Push your notes to your repo

-   Make changes then select check the `Staged` button under the `Git` tab
-   Then select the `Commit` button
-   Add a note to the `Commit message` section (e.g., my updates from today)
-   Select the green arrow (pointing up) to `Push` changes to your GitHub
-   The first time you will need to include your GitHub username and Personal access token

## Get a personal access token

-   Go to your GitHub account
-   In the far upper right pull down menu select `Settings` then `Developer settings`
-   In the left menu select `Personal access tokens` > `Tokens (classic)`
-   Follow instructions to generate a PAT
-   Use your PAT as your password when pushing changes made on your computer to your GitHub account
