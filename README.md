# Survey-Form

Simple survey form webpage made using pure HTML, CSS with dark theme 

## Live Preview

The webpage is live with the help of GitHub pages and you can visit it here: https://alkaison.github.io/Survey-Form/ 

## HTML Code

```HTMl
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="author" content="Alkaison">
    <meta name="description" content="Simple Survey Webpage for Web Developers">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Survey Form</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>
    <!-- Create Form -->
<form id="form" name="survey-form">

    <!-- Details -->
    <div class="form-control">
        <label for="name" id="label-name">
            Name
        </label>

        <!-- Input Type Text -->
        <input type="text"
               id="name"
               placeholder="Enter your name" />
    </div>

    <div class="form-control">
        <label for="email" id="label-email">
            Email
        </label>

        <!-- Input Type Email-->
        <input type="email"
               id="email"
               placeholder="Enter your email" />
    </div>

    <div class="form-control">
        <label for="age" id="label-age">
            Age
        </label>

        <!-- Input Type Text -->
        <input type="text"
               id="age"
               placeholder="Enter your age" />
    </div>

    <div class="form-control">
        <label for="role" id="label-role">
            Which option best describes you?
        </label>
         
        <!-- Dropdown options -->
        <select name="role" id="role">
            <option value="student">Student</option>
            <option value="intern">Intern</option>
            <option value="professional">Professional</option>
            <option value="other">Other</option>
        </select>
    </div>

    <div class="form-control">
        <label>
            Would you recommend Web Development to a friend?
        </label>

        <!-- Input Type Radio Button -->
        <label for="recommed-1">
            <input type="radio"
                   id="recommed-1"
                   name="recommed">Yes</input>
        </label>
        <label for="recommed-2">
            <input type="radio"
                   id="recommed-2"
                   name="recommed">No</input>
        </label>
        <label for="recommed-3">
            <input type="radio"
                   id="recommed-3"
                   name="recommed">Maybe</input>
        </label>
    </div>

    <div class="form-control">
        <label>Languages and Frameworks known
            <small>(Check all that apply)</small>
        </label>
        <!-- Input Type Checkbox -->
        <label for="inp-1">
            <input type="checkbox"
                   name="inp">HTML</input></label>
        <label for="inp-2">
            <input type="checkbox"
                   name="inp">CSS</input></label>
        <label for="inp-3">
            <input type="checkbox"
                   name="inp">JavaScript</input></label>
        <label for="inp-4">
            <input type="checkbox"
                   name="inp">React.js</input></label>
        <label for="inp-5">
            <input type="checkbox"
                   name="inp">Angular</input></label>
        <label for="inp-6">
            <input type="checkbox"
                   name="inp">Django</input></label>
        <label for="inp-7">
            <input type="checkbox"
                   name="inp">Node.js</input></label>
        <label for="inp-7">
            <input type="checkbox"
                   name="inp">Git</input></label>
        <label for="inp-7">
            <input type="checkbox"
                   name="inp">Mongo DB</input></label>
        <label for="inp-7">
            <input type="checkbox"
                   name="inp">Express.js</input></label>
    </div>

    <div class="form-control">
        <label for="comment">
            Any comments or suggestions
        </label>

        <!-- multi-line text input control -->
        <textarea name="comment" id="comment" rows="5" placeholder="Enter your comment here"></textarea>
    </div>
    <!-- Multi-line Text Input Control -->
    <button type="submit" value="submit">Submit</button>
</form>
</body>
</html>
```

## CSS Code

```CSS
:root{
    --theme: #262A33;
}

body {
    background-color: var(--theme);
    font-family: Verdana;
    text-align: center;
}

/* Styling the Form (Color, Padding, Shadow) */
form {
    background-color: #fff;
    max-width: 500px;
    margin: 50px auto;
    padding: 30px 20px;
    box-shadow: 2px 5px 10px rgba(0, 0, 0, 0.5);
}

/* Styling form-control Class */
.form-control {
    text-align: left;
    margin-bottom: 25px;
}

/* Styling form-control Label */
.form-control label {
    display: block;
    margin-bottom: 10px;
}

/* Styling form-control input,
select, textarea */
.form-control input,
.form-control select,
.form-control textarea {
    border: 1px solid #777;
    border-radius: 2px;
    font-family: inherit;
    padding: 10px;
    display: block;
    width: 95%;
    outline: none;
    max-width: 95%;
    max-height: 300px;
}

input:focus, textarea:focus{
    border: 3px solid black;
}

/* Styling form-control Radio
button and Checkbox */
.form-control input[type="radio"],
.form-control input[type="checkbox"] {
    display: inline-block;
    width: auto;
}

/* Styling Button */
button {
    background-color: var(--theme);
    color: white;
    border: 1px solid #777;
    border-radius: 7px;
    font-family: inherit;
    font-size: 21px;
    display: block;
    width: 100%;
    margin-top: 50px;
    margin-bottom: 20px;
    padding: 5px;
}

button:hover, input[type="radio"], input[type="checkbox"]{
    cursor: pointer;
}
```

## Screenshot

![Survey Form Webpage](https://github.com/Alkaison/Survey-Form/blob/main/image.png)