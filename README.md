# Frontend Mentor - Intro component with sign up form solution

This is a solution to the [Intro component with sign up form challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/intro-component-with-signup-form-5cf91bd49edda32581d28fd1). Frontend Mentor challenges help you improve your coding skills by building realistic projects.  

## Table of Contents

- [Overview](#overview)
  - [The Challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built With](#built-with)
  - [What I Learned](#what-i-learned)
  - [Continued Development](#continued-development)
  - [Useful Resources](#useful-resources)

## Overview 

### The Challenge

- View the optimal layout for the site depending on their device's screen size
- See hover states for all interactive elements on the page
- Receive an error message when the `form` is submitted if:
  - Any `input` field is empty. The message for this error should say *"[Field Name] cannot be empty"*
  - The email address is not formatted correctly (i.e. a correct email address should have this structure: `name@host.tld`). The message for this error should say *"Looks like this is not an email"*

### Screenshot

![Sign-up form page](images/signup.jpg)

### Links

- [GitHub Repo URL](https://github.com/adrvnc/sign-up-form)
- [Live Site URL](https://adrvnc.github.io/sign-up-form/)

## My Process


### Built With 

- HTML 
- CSS
- Bootstrap 5.1.3
- JavaScript 
### What I Learned 

I learned how to validate forms using Bootstrap's client-side 
custom validation styles. When a user submits an empty form, the JavaScript 
code below will prevent it from happening until the entire form is filled
out: 

```js 
// Example starter JavaScript for disabling form submissions if there are invalid fields
(function () {
  'use strict'

  // Fetch all the forms we want to apply custom Bootstrap validation styles to
  var forms = document.querySelectorAll('.needs-validation')

  // Loop over them and prevent submission
  Array.prototype.slice.call(forms)
    .forEach(function (form) {
      form.addEventListener('submit', function (event) {
        if (!form.checkValidity()) {
          event.preventDefault()
          event.stopPropagation()
        }

        form.classList.add('was-validated')
      }, false)
    })
})()
```
### Continued Development 

I plan to continue familiarizing myself with Bootstrap's grid system. 


### Useful Resources 

- [Bootstrap Form Validation](https://getbootstrap.com/docs/5.0/forms/validation/) - These are solutions for anyone learning how to validate forms using Bootstrap.  
