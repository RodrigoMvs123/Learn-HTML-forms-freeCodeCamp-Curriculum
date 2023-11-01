# Learn-HTML-forms-freeCodeCamp-Curriculum

https://www.youtube.com/watch?v=vsBZTLE8xHs 

https://raw.githubusercontent.com/RodrigoMvs123/Learn-HTML-forms-freeCodeCamp-Curriculum/main/README.md

Visual Studio Code
EXPLORER
OPEN EDITORS
html-form
index.html

index.html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Registration Form</title>
        <link rel="stylesheet" href="styles.css"/>
    </head>
    <body>
        <h1>Registration Form</h1>
        <p>Please fill out this form with the required information</p>
        
    </body>
</html>

Visual Studio Code
EXPLORER
OPEN EDITORS
html-form
index.html
styles.css

styles.css
body {
    width: 100%;
    height: 100vh; 
    margin: 0;
    background-color: #1b1b32;
    color: #f5f6f7
}

Visual Studio Code
EXPLORER
OPEN EDITORS
html-form
index.html
styles.css

index.html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Registration Form</title>
        <link rel="stylesheet" href="styles.css"/>
    </head>
    <body>
        <h1>Registration Form</h1>
        <p>Please fill out this form with the required information</p>

        <form action="https://register-demo.freecodecamp.org" method="post">
            <fieldset>
                <label>Enter Your First Name:</label>
                <label>Enter Your Last Name:</label>
                <label>Enter Your Email:</label>
                <label>Create a New Password:</label>
            </fieldset>

            <fieldset></fieldset>

            <fieldset></fieldset>
        </form>
        
    </body>
</html>

Visual Studio Code
EXPLORER
OPEN EDITORS
html-form
index.html
styles.css

styles.css
body {
    width: 100%;
    height: 100vh; 
    margin: 0;
    background-color: #1b1b32;
    color: #f5f6f7
}

label {
    display: block;
    margin: 0.5rem 0;
}

Visual Studio Code
EXPLORER
OPEN EDITORS
html-form
index.html
styles.css

index.html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Registration Form</title>
        <link rel="stylesheet" href="styles.css"/>
    </head>
    <body>
        <h1>Registration Form</h1>
        <p>Please fill out this form with the required information</p>

        <form action="https://register-demo.freecodecamp.org" method="post">
            <fieldset>
                <label for="first-name">
                    Enter Your First Name: 
                    <input name="first-name" id="first-name" type="text" required/>
                </label>
                <label for="last-name">
                    Enter Your Last Name: 
                    <input name="last-name" id="last-name" type="text" required/>
                </label>
                <label for="email">
                    Enter Your Email: 
                    <input name="email" id="email" type="email" required/>
                </label>
                <label for="new-password">
                    Create a New Password: 
                    <input name="new-password" id="new-password" type="password" required pattern=[a-z0-5]{8,} />
                </label>
            </fieldset>

            <fieldset>
                <label for="personal-account">
                    <input name="personal-account" id="personal-account" type="radio" name="account-type"/>
                     Personal Account
                </label>
                <label for="business-account">
                    <input name="business-account" id="business-account" type="radio" name="account-type"/>
                     Business Account
                </label>
                <label for="terms-and-conditions">
                    <input name="terms-and-conditions" id="terms-and-conditions" type="checkbox" required/>
                     I accept the <a href="https://www.freecodecamp.org/news/terms-of-service/">terms and conditions</a>
                </label>
            </fieldset>

            <fieldset>
                <label for="profile-picture">
                    Upload a profile picture:
                    <input name="profile-picture" id="profile-picture" type="file"/>
                </label>
                <label for="age">
                    Input your age (years):
                    <input name="age" id="age" type="number" min=13 max=120 />
                </label>
                
                <label for="referrer">
                    How did you hear about us? 
                   <select id="referrer" name="referrer">
                        <option value="">(select one)</option>
                        <option value="1">freeCodeCamp News</option>
                        <option value="2">freeCodeCamp Youtube Channel</option>
                        <option value="3">freeCodeCamp Forum</option>
                        <option value="4">Other</option>
                   </select>
                </label>

                <label for="bio">
                    Provide a bio:
                    <textarea 
                            id="bio" 
                            rows="3" 
                            cols="30"
                            placeholder="I like code on the beach"
                            name="bio"
                    ></textarea>
                </label>

            </fieldset>

            <input type="submit" value="submit"/>
        </form> 
        
    </body>
</html>

Visual Studio Code
EXPLORER
OPEN EDITORS
html-form
index.html
styles.css

styles.css
body {
    width: 100%;
    height: 100vh; 
    margin: 0;
    background-color: #1b1b32;
    color: #f5f6f7;
    font-family: Tahoma;
    font-size: 16px;
}

label {
    display: block;
    margin: 0.5rem 0;
}

h1, p {
    margin: 1em auto;
    text-align: center;
}

form {
    margin: 0 auto;
    max-width: 500px;
    min-width: 300px;
    width: 60vw;
}

fieldset {
    border: none;
    padding: 2rem 0;
    border-bottom: 3px solid #3b3b4f;
}

fieldset:last-of-type {
    border-bottom: none;
}

input, textarea, select {
    width:100%;
    margin: 10px 0 0 0;
}

Visual Studio Code
EXPLORER
OPEN EDITORS
html-form
index.html
styles.css

index.html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Registration Form</title>
        <link rel="stylesheet" href="styles.css"/>
    </head>
    <body>
        <h1>Registration Form</h1>
        <p>Please fill out this form with the required information</p>

        <form action="https://register-demo.freecodecamp.org" method="post">
            <fieldset>
                <label for="first-name">
                    Enter Your First Name: 
                    <input name="first-name" id="first-name" type="text" required/>
                </label>
                <label for="last-name">
                    Enter Your Last Name: 
                    <input name="last-name" id="last-name" type="text" required/>
                </label>
                <label for="email">
                    Enter Your Email: 
                    <input name="email" id="email" type="email" required/>
                </label>
                <label for="new-password">
                    Create a New Password: 
                    <input name="new-password" id="new-password" type="password" required pattern=[a-z0-5]{8,} />
                </label>
            </fieldset>

            <fieldset>
                <label for="personal-account">
                    <input class="inline" name="personal-account" id="personal-account" type="radio" name="account-type"/>
                     Personal Account
                </label>
                <label for="business-account">
                    <input class="inline" name="business-account" id="business-account" type="radio" name="account-type"/>
                     Business Account
                </label>
                <label for="terms-and-conditions">
                    <input class="inline" name="terms-and-conditions" id="terms-and-conditions" type="checkbox" required/>
                     I accept the <a href="https://www.freecodecamp.org/news/terms-of-service/">terms and conditions</a>
                </label>
            </fieldset>

            <fieldset>
                <label for="profile-picture">
                    Upload a profile picture:
                    <input name="profile-picture" id="profile-picture" type="file"/>
                </label>
                <label for="age">
                    Input your age (years):
                    <input name="age" id="age" type="number" min=13 max=120 />
                </label>
                
                <label for="referrer">
                    How did you hear about us? 
                   <select id="referrer" name="referrer">
                        <option value="">(select one)</option>
                        <option value="1">freeCodeCamp News</option>
                        <option value="2">freeCodeCamp Youtube Channel</option>
                        <option value="3">freeCodeCamp Forum</option>
                        <option value="4">Other</option>
                   </select>
                </label>

                <label for="bio">
                    Provide a bio:
                    <textarea 
                            id="bio" 
                            rows="3" 
                            cols="30"
                            placeholder="I like code on the beach"
                            name="bio"
                    ></textarea>
                </label>

            </fieldset>

            <input type="submit" value="submit"/>
        </form> 
        
    </body>
</html>

Visual Studio Code
EXPLORER
OPEN EDITORS
html-form
index.html
styles.css

styles.css
body {
    width: 100%;
    height: 100vh; 
    margin: 0;
    background-color: #1b1b32;
    color: #f5f6f7;
    font-family: Tahoma;
    font-size: 16px;
}

label {
    display: block;
    margin: 0.5rem 0;
}

h1, p {
    margin: 1em auto;
    text-align: center;
}

form {
    margin: 0 auto;
    max-width: 500px;
    min-width: 300px;
    width: 60vw;
    padding-bottom: 2em;
}

fieldset {
    border: none;
    padding: 2rem 0;
    border-bottom: 3px solid #3b3b4f;
}

fieldset:last-of-type {
    border-bottom: none;
}

input, textarea, select {
    width:100%;
    margin: 10px 0 0 0;
    min-height: 2em;
}

.inline {
    width: unset;
    margin: 0 0.5em 0 0;
    vertical-align: middle;
}

input, textarea {
    background-color: #0a0a23;
    border: 1px solid #0a0a23;
    color: #fff;
}

input[type="sumit"] {
    display: block;
    width: 60%;
    min-width: 300px;
    margin: 1em auto;
    height: 2em;
    font-size: 1.1rem;
    background-color: #3b3b4f;
    border-color: white;
}

input[type="file"] {
    padding: 1px 2px; 
}

a {
    color: #dfdfe2;
}


