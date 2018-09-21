# Drupal Design Hacks [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/ucdstudent95618/drupal-design-hacks)
A collection of Drupal design hacks that avoid the use of external CSS files.

*Shortlink: [https://git.io/fAQHX](https://git.io/fAQHX)*

*Read this in other languages: [Spanish](README.es.md)*

## Table of Contents

## Buttons

Buttons can be created by using a link.

### **Single Button**

![Single-button](/img/btn/btn-4.png)

1. Create a link in the editor:

   ![Button Editor](/img/btn/btn-2.png)

   ```html
   <a href="http://www.google.com">button</a>
   ```

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

### **Inline Buttons**

**Method #1**: With a Table

![Inline Button w/o padding](/img/btn/inline-btn-5.png)

1. Create a **table** with the # of columns needed and the **width** to 100%.

   ![Table for Inline Buttons](/img/btn/inline-btn-2.png)

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

![Inline Button With Text](/img/btn/inline-btn-12.png)

1. Create a 2x1 **table** with an appropriate width (eg. 200px) and the **Border size** to 0.

   ![Inline Button Text](/img/btn/inline-btn-6.png)

2. Place the icon on the left **column** and the text on the right **column**.

   ![Inline button with text](/img/btn/inline-btn-7.png)

3. Adjust the left column size to **25 pixels**. 

   ![Adjusting left column](/img/btn/inline-btn-10.png)

4. Adjust **Cell Spacing** to 10 pixels.

   ![Cell Spacing](/img/btn/inline-btn-11.png)

   ```html
   <table align="center" border="0" cellpadding="1" cellspacing="10" style="width:200px">
   	<tbody>
   		<tr>
   			<td style="width:25px"><img alt="" src="http://www.aqua.gov/home/scvwd/main/drupal-w.png" style="height:25px; width:25px" /></td>
   			<td>Lorem Ipsum</td>
   		</tr>
   	</tbody>
   </table
   ```


## Div 



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

   ![Adding CSS to Div](/img/div/div-1.png)

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

2. Add CSS to **Style**.

   ![Adding CSS to Div](/img/div/div-3.png)

   ```css
   background-color: white; margin: 0; padding: 10px; width: 100%;
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


## Tables 

### Creating a Table

1. Create a **Table** of any given size (eg. 3 by 4)  with a **width** of 100% and **Headers** "First Row".

   ![Table settings](/img/table/table-1.png)

```html
<table align="center" border="1" cellpadding="1" cellspacing="1" style="width:100%">
	<thead>
		<tr>
			<th scope="col">&nbsp;</th>
			<th scope="col">&nbsp;</th>
			<th scope="col">&nbsp;</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
	</tbody>
</table>
```



### **Adding Background Color**

**Adding Color to Cell**

![Table with Blue Cell](/img/table/table-3.png)

1. Click on the **Cell**.

2. Go to **Cell Properties** and add the color to **Background Color**.

   ![Adding Background Color](/img/table/table-2.png)

```html
<table align="center" border="1" cellpadding="1" cellspacing="1" style="width:100%">
	<thead>
		<tr>
			<th scope="col" style="background-color: blue;">
			<p>&nbsp;</p>

			<p>&nbsp;</p>
			</th>
			<th scope="col">&nbsp;</th>
			<th scope="col">&nbsp;</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>
			<p>&nbsp;</p>

			<p>&nbsp;</p>
			</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>
			<p>&nbsp;</p>

			<p>&nbsp;</p>
			</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
		<tr>
			<td>
			<p>&nbsp;</p>

			<p>&nbsp;</p>
			</td>
			<td>&nbsp;</td>
			<td>&nbsp;</td>
		</tr>
	</tbody>
</table>
```



**Adding Color to Entire Table**

![Table With Color](/img/table/table-4.png)

1. Right Click on **Table**

2. Go to **Table** **Properties** and add `` Background-color: blue;`` to **Style**.

   ```html
   <table align="center" border="1" cellpadding="1" cellspacing="1" style="background-color:blue; width:100%">
   	<thead>
   		<tr>
   			<th scope="col">
   			<p>&nbsp;</p>
   
   			<p>&nbsp;</p>
   			</th>
   			<th scope="col">&nbsp;</th>
   			<th scope="col">&nbsp;</th>
   		</tr>
   	</thead>
   	<tbody>
   		<tr>
   			<td>
   			<p>&nbsp;</p>
   
   			<p>&nbsp;</p>
   			</td>
   			<td>&nbsp;</td>
   			<td>&nbsp;</td>
   		</tr>
   		<tr>
   			<td>
   			<p>&nbsp;</p>
   
   			<p>&nbsp;</p>
   			</td>
   			<td>&nbsp;</td>
   			<td>&nbsp;</td>
   		</tr>
   		<tr>
   			<td>
   			<p>&nbsp;</p>
   
   			<p>&nbsp;</p>
   			</td>
   			<td>&nbsp;</td>
   			<td>&nbsp;</td>
   		</tr>
   	</tbody>
   </table>
   ```
