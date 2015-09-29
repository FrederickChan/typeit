# TypeIt: A jQuery Animated Typing Plugin

##Description
A light jQuery plugin that outputs text like it's being typed. 

##Setup

1. Create an empty HTML element to select.

  ```<span class="type-it"></span>```

2. Load jQuery, typeit.js, and typeit.css in your page. 

  ```
  <link rel="stylesheet" type="text/css" href="typeit.css">
  
  <script src="jquery-2.1.4.min.js"></script>
  <script src="typeit.js"></script>
  ```

3. Select the element and initialize the `typeit()` function. While you're doing this, enter the string you'd like to output.

  ``
  $('.type-it').typeit({
    stringToType:'Enter your string here!'
  });
  ``
  
##Usage

You can modify the options for the plugin in two different ways -- either by inserting them directly into the function call, or by using data attributes. 
  
  ```
  <span class="type-it" 
  data-typeit-string="A new string to type." 
  data-typeit-speed="100" 
  data-typeit-lifelike="true" 
  data-typeit-showcursor="true">
  
  </span>
  ```
  
  ``
  $('.type-it').typeit();
  ``

  or...

  ``
   <span class="type-it"></span>
  ``

 ```
  $('.type-it').typeit({
    stringToType:'Enter your string here!',
    typeSpeed: 300,
    lifeLike: false,
    showCursor: true
  });
  ```
##Options

There are a number of options you may use to customize typeIt. 

| Option        | Description   | Default Value
| ------------- | ------------- | ------------- |
| stringToType  | The string to be typed.       | 'This is the default string. Please replace this string with your own.' |
| typeSpeed     | The typing speed.             | 500  |
| lifeLike      | Will make the typing pace irregular, as if a real person is doing it.  | true |
| showCursor    | Show a blinking cursor at the end of the string.  | true  |

