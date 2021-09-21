<h1 align="center">Nexter</h1>

![Website Main Mockup](https://github.com/tsokac2/18_nexter/blob/main/public/img/nexter.jpg)

# ["Nexter"](https://res-nexter.herokuapp.com/)

## Contents
* **[Objective](#OBJECTIVE)**
* **[Technologies used](#TECHNOLOGIES-USED)**
* **[Deployment](#DEPLOYMENT)**

****
# OBJECTIVE

Usingcombination of advance CSS Grid by Node.js partials implementation in a single project scop

Project is ready for real-world adjustment and expanding of layout and sub-pages.

Fully responsive to any device/screen and ready for property business implementation and branding.

****
# TECHNOLOGIES USED

## # [HTML](https://en.wikipedia.org/wiki/HTML)
**Semantic elements**: _nav_, _section_, _footer_, _div_(content division element), _span_(inline container), _i_ (text element).

## # [CSS3](https://en.wikipedia.org/wiki/CSS)
**Modules:** Borders, Background and text-effects, Flexible Box Layout, CSS Grid Layout, CSS Transitions, CSS Image Values & Replaced Content, CSS Values & Units.

## # [SASS PRE-PROCESSOR](https://sass-lang.com/)
**TOOLS INCLUDED:**
* SASS interpolation
* SASS Mixings - Responsive layout functions
* SASS Variables
* SASS Nesting
* SASS Compiler

**COMPILER IMPLEMENTATION:**
* Open Command Prompt
* Navigate to the root project folder
* Enter commands in the following order:
  * `npm init --yes` - **PRESS ENTER**
  * `npm i -g node-sass` - **PRESS ENTER**
  * In `{} package.json` file under the `"scripts"` type the **[FOLLOWING](https://github.com/tsokac2/newirishlife/blob/main/static/wireframes/sass_01.png)**
* To start **SASS Compiler** enter the following command: `npm run watch` - **PRESS ENTER**
* If no errors the compilation process _NPM SERVER_ will start with the following console log message:
    ```
    > new@1.0.0 watch C:\Users\Tomislav\Desktop\new
    > node-sass -o assets/css assets/scss/index.scss -w
    ```
**SASS IMPLEMENTATION AND FOLDER STRUCTURE**
* Create the following folder structure:
  * assets/scss/abstracts - global SASS **variables** and **mixins** function
  * assets/scss/base - global styles for html, body and special helper classes
  * assets/scss/components - carousel image slideshow, small screen navigation menu
  * assets/scss/layout - styling for _HOME_, _TRIP_, _WORK_, _LIFE_, _SHOP_, _SIGNUP_, _LOGIN_, _BAG_, _PRODUCT DETAILS_, _CHECKOUT_, _FOOTER_
  * assets/scss/_index.scss - referencing all `*.scss` files in folder structure, **[EXAMPLE](https://github.com/tsokac2/newirishlife/blob/main/static/wireframes/sass_02.png)**
  * **SASS RESPONSIVE Mixins** function **[EXAMPLE](https://github.com/tsokac2/newirishlife/blob/main/static/wireframes/sass_03.png)**
* All files in the above folders **MUST** be named with the following naming conventions: `_filename.scss`

**[Back to content](#contents)**

## # [NODE.JS](https://nodejs.org/en/)
* Use for NPM `package.json` file implementation into the project root

## # [NPM](https://www.npmjs.com/)
* Package manager - Use package - `node-sass`

## # [JAVASCRIPT](https://www.javascript.com/)
Features: _Dom Events_, _Validation of User’s Input_, _Else and If Statement_, _Handling Events_,  _In-Built Function_


## # [GOOGLE CDN's](https://fonts.google.com/)
* Google Fonts - **[Merienda](https://fonts.google.com/specimen/Merienda?preview.text=&preview.text_type=custom&query=mer)**
* Google Fonts - **[Lato](https://fonts.google.com/?preview.text=&preview.text_type=custom&query=LATO)**
* Google Fonts - **[Josefin](https://fonts.google.com/specimen/Josefin+Sans?preview.text_type=custom)**

**[Back to content](#contents)**

## # [HEROKU](https://www.heroku.com)
* Cloud platform service used for hosting a "live" version of the project


## # [FONTAWESOME](https://fontawesome.com/) 
* Use mostly for menu items and across projects elements

## # [GIT](https://git-scm.com/)
* Distributed version control system

## # [GITHUB](https://github.com/)
* Project files hosting platform

## # [IDE Visual Studio Code](https://code.visualstudio.com/)
* Project code editor 

## # [ADOBE PHOTOSHOP](https://www.adobe.com/)
* Images preparation - Logo Design

## # [ADOBE ILLUSTRATOR](https://www.adobe.com/)
* Logo Design 

## # [BALSAMIQ WIREFRAMES](https://balsamiq.com/) 
* Wireframes Design

**[Back to content](#contents)**

****

# DEPLOYMENT

**[PROJECT LINK](https://newirishlife.herokuapp.com/)**

### LOCAL PROJECT SETUP:
* Create a new repository on **[GitHub](https://github.com)**
* Create a project folder on the local device
* Start **[CMD](https://en.wikipedia.org/wiki/Cmd.exe)** on the local device and navigate to the root folder of the project
* Initialize project root folder with the following CMD command: `git init`
* Create _README.MD_ file with CMD command: `echo #New Irish Life > README.md`
* Initiate `git add .` command in CMD project root folder
* Initiate commit `git commit -m "Test first commit"` command in CMD project root folder
* Create a connection with the local device and GitHub repository with the CMD command 
  ```
  git remote add origin https://github.com/username/project_repo_name.git
  ```
* Initiate push command `git push -u origin master`
* Make regular commits after every project change with proper commit message more info in **[Git Commit Message](https://chris.beams.io/posts/git-commit/#separate)**
* Use `git push` command in CMD for code commits 

**[Back to content](#contents)**

## DEPLOYMENT TO HEROKU
### Create application:
**1.** Navigate to **[HEROKU](https://id.heroku.com/login)** and log in

**2.** Click on the _New_ button

**3.** Select Create a _New App_

**4.** Enter the app name

**5.** Select region

### Configure the connection to Github Repository
**1.** Click the **_Deploy_** tab and select **_GitHub - Connect to GitHub_**

**2.** Select GitHub

**3.** Enter the repository name for the project and click search

**4.** When repo has been found, click the _connect_ button

### Enable automatic deployment:
**1.** Select the _Deploy_ tab and click _Enable Automation Deploys_

**2.** Click the _Deploy_ button

**3.** When the app is created check the logs for deployment errors, if none, click the _"View"_ button

**[Back to content](#contents)**
