---
title: "realizar un formulario freecodecamp"
date: 2023-11-19T08:43:36-05:00
draft: true
---

# creacion de un formulario
## cuerpo de **HTML_5**

```
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Registration Form</title>
<link rel="stylesheet" href="style.css"> 
</head>
<body>
</body>
</html>
```


```
 <form action='https://register-demo.freecodecamp.org'></form>
```
## The Action Attribute
The action attribute defines the action to be performed when the form is submitted.

Usually, the form data is sent to a file on the server when the user clicks on the submit button.

the form data is sent to a file called "action_page.php". This file contains a server-side script that handles the form data:

## The Method Attribute

The method attribute specifies the HTTP method to be used when submitting the form data.

The form-data can be sent as URL variables (with method="get") or as HTTP post transaction (with method="post").

The default HTTP method when submitting form data is GET. 



List of All <form> Attributes
|Attribute|	Description|
|---------|------------|
| accept-charset	| Specifies the character encodings used for form submission |
|action	|Specifies where to send the form-data when a form is submitted|
|autocomplete	|Specifies whether a form should have autocomplete on or off|
|enctype	|Specifies how the form-data should be encoded when submitting it to the server (only for method="post")|
|method	|Specifies the HTTP method to use when sending form-data|
|name	|Specifies the name of the form|
|novalidate	|Specifies that the form should not be validated when submitted|
|rel	|Specifies the relationship between a linked resource and the current document|
|target	|Specifies where to display the response that is received after submitting the form|

```
 <form method="post" action='https://register-demo.freecodecamp.org'>
    
    </form>
```

The first fieldset will hold name, email, and password fields. Start by adding four label elements to the first fieldset.
```
<form method="post" action='https://register-demo.freecodecamp.org'>
      <fieldset>

      </fieldset>
      <fieldset></fieldset>
      <fieldset></fieldset>
    </form>
```

2023-11-19-10:38

---
title: "realizar un formulario freecodecamp"
date: 2023-11-21T06:43:36-05:00
draft: true
---

## How do you link labels and inputs in HTML?
There are two ways to pair a label and an input. One is by wrapping the input in a label (implicit), and the other is by adding a for attribute to the label and an id to the input (explicit). Think of an implicit label as hugging an input, and an explicit label as standing next to an input and holding its hand

```
 <fieldset>
        <label for="first-name">Enter Your First Name: <input id="first-name" /></label>
        <label for="last-name">Enter Your Last Name: <input id="last-name" /></label>
        <label for="email">Enter Your Email: <input id="email" /></label>
        <label for="new-password">Create a New Password: <input id="new-password" /></label>
 </fieldset>
```

rem means root of em

## type attribute.

Specifying the type attribute of a form element is important for the browser to know what kind of data it should expect. If the type is not specified, the browser will default to text.

```
   <form method="post" action='https://register-demo.freecodecamp.org'>
      <fieldset>
        <label for="first-name">Enter Your First Name: <input id="first-name" type="text" /></label>
        <label for="last-name">Enter Your Last Name: <input id="last-name" type="text" /></label>
        <label for="email">Enter Your Email: <input id="email" type="email" /></label>
        <label for="new-password">Create a New Password: <input id="new-password" type="password" /></label>
       
      </fieldset>
      <fieldset></fieldset>
      <fieldset></fieldset> <input type="submit" value="Submit"/>
```
![adding submit button](img/submitButtom.png)

## intective form
To make the form interactive, add the required attribute to the input elements in the first fieldset.

