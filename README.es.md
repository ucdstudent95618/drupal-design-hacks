# # Drupal Design Hacks [![Impresionante](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/ucdstudent95618/drupal-design-hacks)
Una colección de hacks de diseño de Drupal que evitan el uso de archivos CSS externos.

*Enlace corto: [https://git.io/fAQHX](https://git.io/fAQHX)*

*Lea esto en otros idiomas: [Ingles](README.md)*

*Repo de Drupal*: https://git.io/fA5gb



## Compatibilidad

- Drupal *Versión 7* y otros

## Tabla de contenido

- [Botones](#botones)
    ​    - [Botón individual](#botón-individual)
    ​    - [Botones en línea](#botones-en-línea)
    ​    - [Botón en línea con texto](#en-línea-botón-con-texto)
- [Divs](#div)
        - [Creando una Div](#creando-una-div)
            - [Estilo de una Div](#estilo-de-una-div)
- [Imágenes](#imágenes)
    ​    - [Agregar una imagen](#adding-an-image)
      - [Cambiar el tamaño de una imagen](#redimensionar-una-imagen)
      - [Imagen circular](#imagen-circular)
      - [Esquinas redondeadas de la imagen](#esquinas-redondeadas-de-la-imagen)
- [Tablas](#tablas)
    ​    - [Creando una tabla](#creando-una-tabla)
    ​    - [Agregar color a una sola celda](#agregar-color-a-una-sola-celda)
    ​    - [Agregar color a toda la tabla](#agregar-color-a-toda-la-tabla)

## Botones

### **Botón individual**

![Botón único](/img/btn/btn-4.png)

1. Crea un enlace en el editor:

   ![Button Editor](/img/btn/btn-2.png)



   HTML

```html
   <a href="http://www.google.com"> botón </a>
```

2. Agregue CSS a **Estilo**.



   HTML

```html
<a href="http://www.google.com" style="display: block; background-color: blue; width: 175px; height: 45px; line-height: 45px; color: white; border-radius: 10px; tamaño de letra: 18px; text-decoration: none;" Botón type ="button"> </a>
```
```



   CSS

​```css
   bloqueo de pantalla;
   color de fondo: azul;
   ancho: 175px;
   altura: 45px;
   línea-altura: 45px;
   color blanco;
   radio del borde: 10px;
   tamaño de letra: 18px;
   texto-decoración: ninguno;
```

3. Agregue el "botón" a **Tipo de contenido asesor**.

   ![CSS agregado](/img/btn/btn-3.png)



### **Botones en línea**

**Método n. ° 1**: con una tabla

![Botón en línea sin relleno](/img/btn/inline-btn-5.png)

1. Cree una **tabla** con el # de columnas necesarias y el **ancho** al 100%.

   ![Tabla para botones en línea](/img/btn/inline-btn-2.png)



   HTML

```html
   <table border="0" cellpadding="0" cellspacing="0" style="width: 100%">
   	<tbody>
   		<tr>
   			<td> & nbsp; </ td>
   			<td> & nbsp; </ td>
   			<td> & nbsp; </ td>
   		</ tr>
   	</ tbody>
   </ table>
```



3. Agregue **botones** a **columnas de la tabla** y cambie el ancho a la suma del ancho de los botones ``style="width:525px;"`` .

 HTML

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



**Método n. ° 2**: con CSS

![Botones en línea](/img/btn/inline-btn.png)

1. Crea un conjunto de **botones** uno al lado del otro.

 HTML

   ``` html
   <a href="http://www.google.com" style="display: block; background-color: blue; width: 175px; height: 45px; text-align: center; line-height: 45px; color: white; font-size: 18px; text-decoration: none;" type="button">button</a> 
   <a href="http://www.google.com" style="display: block; background-color: blue; width: 175px; height: 45px; text-align: center;line-height: 45px; color: white; font-size: 18px; text-decoration: none;" type="button">button</a> 
   <a href="http://www.google.com" style="display: block; background-color: blue; width: 175px; height: 45px; text-align: center;line-height: 45px; color: white; font-size: 18px; text-decoration: none;" type="button">button</a>
   ```



2. Agregue `` display: inline-block; `` a su **estilo**.

HTML

   ```html
   <a href="http://www.google.com" style="display: block; background-color: blue; width: 175px; height: 45px; text-align: center; line-height: 45px; color: white; display: inline-block; font-size: 18px; text-decoration: none;" type="button">button</a> 
   <a href="http://www.google.com" style="display: block; background-color: blue; width: 175px; height: 45px; text-align: center;line-height: 45px; color: white; display: inline-block; font-size: 18px; text-decoration: none;" type="button">button</a> 
   <a href="http://www.google.com" style="display: block; background-color: blue; width: 175px; height: 45px; text-align: center;line-height: 45px; color: white; display: inline-block; font-size: 18px; text-decoration: none;" type="button">button</a>
   ```



