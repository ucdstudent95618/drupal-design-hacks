# Drupal Design Hacks [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/ucdstudent95618/drupal-design-hacks)
A collection of Drupal design hacks that avoid the use of external CSS files.


*Shortlink: ['https://git.io/fAQHX'](https://git.io/fAQHX)*

*Read this in other languages: [Spanish](README.es.md)*

## Table of Contents

## Buttons

In order to create a button you must do the following

1. Create a link in the editor:

   ```html
   <a href="http://www.google.com">button</a>
   ```

   ![Button Editor](/img/btn/btn-2.png)

2. Add CSS to **Style**.

   ```html
   <a href="http://www.google.com" style="display: block; background-color: blue; width: 175px; height: 45px; line-height: 45px; color: white; border-radius: 10px; font-size: 18px; text-decoration: none;" type="button">button</a>
   ```

   ```css
   display: block;
   background-color: blue;
   width: 175px;
   height: 45px;
   line-height: 45px;
   color: white;
   border-radius: 10px;
   font-size: 18px;
   text-decoration: none;
   ```

3. Add "button" to **Advisory Content Type**.

![Added CSS](/img/btn/btn-3.png)

Result: 

![button result](/img/btn/btn-4.png)



