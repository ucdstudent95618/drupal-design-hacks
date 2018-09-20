# Drupal Design Hacks [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/ucdstudent95618/drupal-design-hacks)
A collection of Drupal design hacks that avoid the use of external CSS files.

*Shortlink: [https://git.io/fAQHX](https://git.io/fAQHX)*

*Read this in other languages: [Spanish](README.es.md)*

## Table of Contents

## Buttons

Buttons can be created by using a link.

### ***Single-Button***

![Single-button](/img/btn/btn-4.png)

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

**Method #1**: With a Table

![Inline Button w/o padding](/img/btn/inline-btn-5.png)

1. Create a **table** with the # of columns needed and the width to 100%.

   ```html
   <table border="0" cellpadding="0" cellspacing="0" style="width:100%">
   	<tbody>
   		<tr>
   			<td>&nbsp;</td>
   			<td>&nbsp;</td>
   			<td>&nbsp;</td>
   		</tr>
   	</tbody>
   </table>
   ```

![Table for Inline Buttons](/img/btn/inline-btn-2.png)

2. Change **cellpadding** and **cellspacing** to zero.

   ![Cell padding/spacing set to zero](/img/btn/inline-btn-3.png)

   ```html
   <table border="0" cellpadding="0" cellspacing="0" style="width:100%">
   	<tbody>
   		<tr>
   			<td></td>
   			<td></td>
   			<td></td>
   		</tr>
   	</tbody>
   </table>
   ```



3. Add **buttons** to **table columns** and change the width to the sum of button widths ``style="width:525px;"`` .

   ``` html
   <table align="center" border="0" cellpadding="0" cellspacing="0" style="width:525px">
   	<tbody>
   		<tr>
   			<td><a href="http://www.google.com" style="display: block; background-color: blue; width: 175px; height: 45px; text-align: center; line-height: 45px; color: white; font-size: 18px; text-decoration: none;" type="button">button</a></td>
   			<td><a href="http://www.google.com" style="display: block; background-color: blue; width: 175px; height: 45px; text-align: center; line-height: 45px; color: white; font-size: 18px; text-decoration: none;" type="button">button</a></td>
   			<td><a href="http://www.google.com" style="display: block; background-color: blue; width: 175px; height: 45px; text-align: center; line-height: 45px; color: white; font-size: 18px; text-decoration: none;" type="button">button</a></td>
   		</tr>
   	</tbody>
   </table>
   ```



**Method #2**: With CSS

![Inline Buttons](/img/btn/inline-btn.png)

1. Create a set of **buttons** side by side.

   ``` html
   <a href="http://www.google.com" style="display: block; background-color: blue; width: 175px; height: 45px; text-align: center; line-height: 45px; color: white; font-size: 18px; text-decoration: none;" type="button">button</a> 
   <a href="http://www.google.com" style="display: block; background-color: blue; width: 175px; height: 45px; text-align: center;line-height: 45px; color: white; font-size: 18px; text-decoration: none;" type="button">button</a> 
   <a href="http://www.google.com" style="display: block; background-color: blue; width: 175px; height: 45px; text-align: center;line-height: 45px; color: white; font-size: 18px; text-decoration: none;" type="button">button</a>
   ```

2. Add ``  display: inline-block; `` to their **style**.

   ```html
   <a href="http://www.google.com" style="display: block; background-color: blue; width: 175px; height: 45px; text-align: center; line-height: 45px; color: white; display: inline-block; font-size: 18px; text-decoration: none;" type="button">button</a> 
   <a href="http://www.google.com" style="display: block; background-color: blue; width: 175px; height: 45px; text-align: center;line-height: 45px; color: white; display: inline-block; font-size: 18px; text-decoration: none;" type="button">button</a> 
   <a href="http://www.google.com" style="display: block; background-color: blue; width: 175px; height: 45px; text-align: center;line-height: 45px; color: white; display: inline-block; font-size: 18px; text-decoration: none;" type="button">button</a>
   ```



### Inline Button With Text 



## Divs 

<table border="1" cellpadding="1" cellspacing="1" style="background-color:white; margin:0; padding:10px; width:100%">
	<tbody>
		<tr>
			<td>
			<p>Lorem ipsum dolor sit amet, eu graece mentitum principes nec, et eam homero quaeque. An vim purto velit veritus. Sint aperiri eloquentiam usu ei, sint tota graeco at has, ne eius graeci conclusionemque ius. Sint mollis laoreet has ei. Has ea quod solet, cu error iisque nam, ea quo dolorum senserit postulant. Et sonet consetetur sea, quo et detraxit facilisis delicatissimi.</p>
			</td>
		</tr>
	</tbody>
</table>

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
   background-color: white;
   margin: 0;
   padding: 10px;
   width: 100%;
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

