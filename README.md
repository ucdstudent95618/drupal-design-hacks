# Drupal Design Hacks [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/ucdstudent95618/drupal-design-hacks)
A collection of Drupal design hacks that avoid the use of external CSS files.

*Shortlink: [https://git.io/fAQHX](https://git.io/fAQHX)*

*Read this in other languages: [Spanish](README.es.md)*

## Table of Contents

## Buttons

Buttons can be created by using a link.

### ***Single-Button***

 ![button result](/img/btn/btn-4.png)

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

### ***Inline Buttons***


## Divs 

![Div Example](/img/div/div-2.png)

1. Create at **table** that is 1x1.

   ```html
   <table border="1" cellpadding="1" cellspacing="1">
   	<tbody>
   		<tr>
   			<td>
   			</td>
   		</tr>
   	</tbody>
   </table>
   ```

   ![Adding CSS to Div](/img/div/div-1.png)

2. Add CSS to **Style**.

   ```css
   background-color:white;
   margin:0;
   padding:10px;
   width:100%;
   ```

   ```html
   <table border="1" cellpadding="1" cellspacing="1" style="background-color:white; margin:0; padding:10px; width:100%">
   	<tbody>
   		<tr>
   			<td>
   			<p>Lorem ipsum dolor sit amet, eu graece mentitum principes nec, et eam homero quaeque. An vim purto velit veritus. Sint aperiri eloquentiam usu ei, sint tota graeco at has, ne eius graeci conclusionemque ius. Sint mollis laoreet has ei. Has ea quod solet, cu error iisque nam, ea quo dolorum senserit postulant. Et sonet consetetur sea, quo et detraxit facilisis delicatissimi.</p>
   			</td>
   		</tr>
   	</tbody>
   </table>
   ```

   ![Adding CSS to Div](/img/div/div-3.png)

## Tables 

