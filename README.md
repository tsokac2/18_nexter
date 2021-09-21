<h1 align="center">Nexter</h1>

![Website Main Mockup](https://github.com/tsokac2/18_nexter/blob/main/public/img/w_nexter.jpg)

# ["Nexter"](https://res-nexter.herokuapp.com/)

## Contents
* **[Technologies used](#TECHNOLOGIES-USED)**
* **[Deployment](#DEPLOYMENT)**

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

## # [JQUERY](https://fonts.google.com/)
**APPLIED jQuery DOM EVENTS** for highlighting **_"Quick Links"_** cards elements.

**[TRIP](https://newirishlife.herokuapp.com/trip)**, **[WORK](https://newirishlife.herokuapp.com/work)**, and **[LIFE](https://newirishlife.herokuapp.com/life)** sections are containing **_Quick Links_** card elements.

Every card element contains the _MAIN LINK_ source to the external services provider and a **_"Quick Links..."_** button element for loading detailed links when the user chose the services provider destination. **[EXAMPLE](https://github.com/tsokac2/newirishlife/blob/main/static/wireframes/quicklinks_life.png)**

**_base.html_** template contains <div class="blur"> just after opening tag for the background _"fade-out"_  effect 

**jQuery DOM Events** used for above-mentioned cards element functionality:

* Element with id **#showLinks1** was clicked
* `var thisCardLinkShow = "." + this.id + "-grid";` checking for `<div>` element with class `.showLinks1-grid`
* `$(thisCardLinkShow).show(300)` referring to `this` element to `.show()` with speed of 300 milliseconds
* `$(".blur").fadeIn(400)` loading background "blur" effect with speed of 400 milliseconds
* `$(thisCardLinkShow).addClass("rel-card");` adding class `.addClass("rel-card")` to element that is referring to `this` element
* `$("#Card1").addClass("wrap-rel");`  adding class `.addClass("rel-card")` to element with id **Card1**

The process is replicated for the `<button id="#hideLinks1">` element with the id of `#hideLinks1` for the "hiding" effect with `.removeClass("wrap-rel");` - **[SOURCE CODE](https://github.com/tsokac2/newirishlife/blob/main/static/js/cards.js)** from lines **9 - 14** 

If user click anywhere on the screen _"loaded"_ elements will _"hide"_ and that is achieved with following `.click()` DOM effect on `<div class="blur>`.
`.blur` element contains absolute position properties with a z-index of 1000: **[SOURCE CODE](https://github.com/tsokac2/newirishlife/blob/main/static/js/cards.js)** from lines **34 - 38** 

**FULL SOURCE CODE:** for jQuery Cards DOM Events **[cards.js](https://github.com/tsokac2/newirishlife/blob/main/static/js/cards.js)**

**[Back to content](#contents)**

## # [BOOTSTRAP v4.5.2](https://getbootstrap.com/docs/4.5/getting-started/introduction/)
* Bootstrap was used to assist with the responsiveness and styling of the website
* Mani layout control - responsive layout usage - helper classes included - example -  .mt, .pt, .d-none .d-md-block, .col, col-sm, col-md, col-lg, etc...

## # [PYTHON DJANGO](https://www.djangoproject.com/)
Python Modules Full list in **[requirements.txt](https://github.com/tsokac2/newirishlife/blob/main/requirements.txt)**

## # [POSTGRESQL](https://www.postgresql.org/)
PostgreSQL open source object-relational database system.

## # [STRIPE](https://stripe.com/ie)
Stripe's software and APIs online payments provider.

More details for the **"CHECKOUT"** testing steps view in _*.xlsx_ file test case number: **[TC021](https://github.com/tsokac2/newirishlife/blob/main/static/wireframes/M4_Testing.xlsx)**

#### Test Card

| Card | Test number |
| ----------- | ----------- |
| Card Number | **4242 4242 4242 4242** |
| Expiry Date | any valid date ex. **02/25** | 
| CVC Number | any 3 digits number ex. **555**| 


## # [AWS S3](https://aws.amazon.com/s3/)
Amazon Simple Storage Service (Amazon S3) object storage service.

AWS S3 bucket was used for storing the following static files:
* Image file for a specific section and custom png icons
* JavaScript files
* Global index.css file
* Downloads files
* Media files for SHOP section - 3 images pre one product item

**[Back to content](#contents)**

## # [EMAILJS](https://dashboard.emailjs.com/sign-in)
**IMPLEMENTATION**
* Add New Service - Gmail
* Email Templates - Create New Template
* Use following syntax for form attributes, syntax {{form_name}}
* SENT Email content from a user
* Select the Auto-Reply option and place the following: **_SUBJECT**: On behalf of all of us from New Irish Life, welcome onboard!_
* **WELCOMING** **[Email](https://github.com/tsokac2/newirishlife/blob/main/static/wireframes/email.png)** content sent to the user after successful submission

**SCRIPTS INTEGRATION:**
 * Before closing **`<head>`** element place following **CDN** script tag:
    * `<script src="https://cdn.jsdelivr.net/npm/emailjs-com@2/dist/email.min.js"></script>`
  * Place following call-back function after **CDN** link

  ```
  <script type="text/javascript">
        (function() {
        emailjs.init("user_hI6S08d1aK1XKKU2VWtOI");
        })();
  </script>
  ```
  * Check `User ID` under "Integration" option on EmailJS dashboard
  * Create `sendEmail` function **[CODE EXAMPLE](https://github.com/tsokac2/newirishlife/blob/main/static/js/emailnews.js)** from lines **88 - 103** 

**FROM VALIDATION DEVELOPMENT**
* Create **[EventTarget](https://github.com/tsokac2/newirishlife/blob/main/static/js/emailnews.js)** method addEventListener() sets up a function that will be called whenever the specified event is delivered to the target, in this case `newsletter()` function - **[CODE EXAMPLE](https://github.com/tsokac2/newirishlife/blob/main/static/js/emailnews.js)** from lines **1 - 3** 
*  Create 2 validation function for UX purposes, `validateName()` and `validateEmail()` function.
* `validateName()` function is _**returning**_ Boolean value `true` or `false` that is stored in empty variable `var valid;` depending of a user input string value - **[CODE EXAMPLE](https://github.com/tsokac2/newirishlife/blob/main/static/js/emailnews.js)** from lines **5 - 22**
* Implement call-back functions regarding what kind of input value was submitted by a user.
* `pushSuccessFor()` function is adding a `.success` class to the input element when user input is valid - **[CODE EXAMPLE](https://github.com/tsokac2/newirishlife/blob/main/static/js/emailnews.js)** from lines **55 - 58**
* User email validation is stored in the `validateEmail()` function with a call-back function that is checking user email - **[SOURCE](https://github.com/tsokac2/newirishlife/blob/main/static/js/emailnews.js)**
* To get a valid email id we use a regular expression
* Regular Expression Pattern : `/^(([^<>()\[\]\\.,;:\s@"]+(\.[^<>()\[\]\\.,;:\s@"]+)*)|(".+"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/`
* `testEmail()` function:

  ```
    function testEmail(email) {
        return /^(([^<>()\[\]\\.,;:\s@"]+(\.[^<>()\[\]\\.,;:\s@"]+)*)|(".+"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/.test(email);
    };
  ```

* To submit user data to the server we are declaring `send()` function in variable `var send = function(){...};` and calling that function when submit `<button>` is triggered - **[CODE EXAMPLE](https://github.com/tsokac2/newirishlife/blob/main/static/js/emailnews.js)** from lines **60 - 76**

* Validation tests are covered in **[TESTING.MD](https://github.com/tsokac2/newirishlife/blob/main/TESTING.md)** file

**[Back to content](#contents)**

## # [GOOGLE CDN's](https://fonts.google.com/) and [GOOGLE API](https://developers.google.com/maps/gmp-get-started#quickstart)
* Google Fonts - **[Merienda](https://fonts.google.com/specimen/Merienda?preview.text=&preview.text_type=custom&query=mer)**
* Google Fonts - **[Lato](https://fonts.google.com/?preview.text=&preview.text_type=custom&query=LATO)**
* Google Fonts - **[Josefin](https://fonts.google.com/specimen/Josefin+Sans?preview.text_type=custom)**

**GOOGLE API IMPLEMENTATION STEPS:**
  * Pick Google Maps product **[More info](https://developers.google.com/maps/gmp-get-started#quickstart)**
  * Create a project.
  * Set up a billing account.
  * Enable APIs associated with the products you picked.
  * Create an API key-  documentation source - **[API Key](https://developers.google.com/maps/documentation/javascript/get-api-key)**
  * API keys for frontend-only applications cannot be hidden like is stated on the following link **[Hide API Keys](https://gist.github.com/derzorngottes/3b57edc1f996dddcab25)**, developers **[Comment](https://github.com/tsokac2/newirishlife/blob/main/static/wireframes/API_Secure.png)**

**SCRIPTS INTEGRATION:**
  * In `<head>` element place `<scripts>` in following order:

    ```
    <script src="assets/js/markerclusterer_compiled.js"></script>
    <script defer src="https://maps.googleapis.com/maps/api/js?key="YOUR API KEY"&callback=initMap"></script>
    <script src="assets/js/maps.js"></script>
    ```
  * Create `<div>` element with ID `<div id="map">` render map place
  * Marker Cluster CDN - **[SOURCE](https://cdnjs.com/libraries/js-marker-clusterer)**
  * Creating call-back function in `<script src="assets/js/maps.js"></script>` -  **[CODE EXAMPLE](https://github.com/tsokac2/newirishlife/blob/main/static/js/maps.js)** from lines **1 - 36** 

* `function initMap() {..}` maps location on a major scale in this case Dublin, Ireland
* `google.maps.event.addDomListener(window, "resize", function() {...}` adding Google Maps DOM listener
* `let busMarkerIcon = {...}` creating custom map marker with `scaledSize` property
* `const Bus747Stop = new google.maps.Marker({...});` pointing to Bus Stop for 747 Dublin Bus line for Dublin Airport

**FULL SOURCE CODE:** GOOGLE MAPS API **[maps.js](https://github.com/tsokac2/newirishlife/blob/main/static/js/maps.js)**

**[Back to content](#contents)**

## # [HEROKU](https://www.heroku.com)
* Cloud platform service used for hosting a "live" version of the project

## # [JASMINE BEHAVIOR-DRIVEN JavaScript](https://jasmine.github.io)
* Full testing and implementation process described in **[TESTING.MD](https://github.com/tsokac2/newirishlife/blob/main/TESTING.md)** file 

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

## # [AM I Responsive?](http://ami.responsivedesign.is/)
* Multi-Device Website Mockup Generator was used to create the project Mockup image

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

### Set environment variables:
* Click the **_Settings_** tab and then click the **_Reveal Config Vars_** button and add the following:

    **1.** AWS_ACCESS_KEY_ID

    **2.** AWS_SECRET_ACCESS_KEY

    **3.** DATABASE_URL

    **4.** EMAIL_HOST_PASS

    **5.** EMAIL_HOST_USER

    **6.** SECRET_KEY - **[Random Key Generator](https://randomkeygen.com/)**

    **7.** STRIPE_PUBLIC_KEY

    **8.** STRIPE_PUBLIC_KEY

    **10.** STRIPE_WH_SECRET

    **11.** USE_AWS

### Enable automatic deployment:
**1.** Select the _Deploy_ tab and click _Enable Automation Deploys_

**2.** Click the _Deploy_ button

**3.** When the app is created check the logs for deployment errors, if none, click the _"View"_ button

### LOCAL HOSTING
**Note:** The project will not run locally unless the user sets up a _SECRET-KEY_ with **[Random Key Generator](https://randomkeygen.com/)**

**_These details are private and not disclosed in this repository for security purposes._**

Once the project has been loaded into an IDE of choice, run the following command in the shell to install all the required packages: pip install -r requirements.txt.

To run a local Django server run the following command in CMD:
`python manage.py runserver`

**[Back to content](#contents)**
