# Observaciones

Mica, felicitaciones por tu trabajo. Me encanta como quedó tu portfolio, se ve muy lindo, limpio y profesional. Me gustan los colores y tipografías, y tengo que destacar la increíble atención al detalle que demostrás y lo bien que anda tu responsive. 

Como dije en clase, este trabajo no se hace para que constates conocimientos, sino para que aprendas: en ese sentido, mi intencion es que estos comentarios te sirvan para aprender, mejorar tu codigo a futuro e ir apreciando mejor qué se espera de nosotras como desarrolladoras front end.

## Estructura correcta de documento HTML

Tu HTML esta realmente excelente. Claro, prolijo, muy bien comentado e identado. Lo único a comentar es que dejar un salto de linea entre cada etiqueta hace muy dificil la lectura. Privilegiá escribir uno debajo del otro sin un espacio entre cada uno. 

Algo que me llama la atención es tu `head`, dado que allí repetís innecesariamente el link de google fonts. No es necesario escribilo dos veces

```html
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
```

Cada uno de esos links hace exactamente lo mismo - traerse el css de google fonts para poder usar los fonts en tu sitio. Quizá estés bajo la impresión de que por cada uno de los fonts de tu web es necesario traerse nuevamente el css, pero no, no es necesario agregarlo más de una vez. Agregar muchos de estos links innecesarios impacta negativamente en la velocidad de carga de tu web, ya que por cada uno de ellos se hace un llamado a un css externo y se lo carga. 

## Respeta la consigna

- El portfolio cuenta con las secciones solicitadas
- Al clickear en los links de navegación, debe llevar a la sección correspondiente
- Al clickear en los links de contacto, debe llevar a la página externa
  correspondiente
- El portfolio debe tener un diseño responsivo y verse correctamente en distintos dispositivos
- El portfolio debe estar deployado y ser accesible desde una URL
- El repositorio en GitHub debe tener un readme adecuado

Todos estos puntos están cumplidos. Menciono especialmente tu responsive: es increíble lo bien que solucionaste las distintas resoluciones, siguiendo casi a la perfección el modelo y preocupandote para que todo se vea hermoso, veamos tu web desde cualquier dispositivo. La única observación acá sería, a nivel diseño, que las tarjetas de Mis Proyectos se ven algo alargadas en celulares pequeños: quiza quieras revisar su `height`.

### Respeta el diseño dado

Cumplido a la perfección. 

### Buena estructura de proyecto

Cumplido casi a la perfección, pero el favicon deberia estar en la carpeta principal (en mi computadora no se ve, por ejemplo). Notá también que tenés una carpeta innecesaria, `vscode`, que es agregada a veces automáticamente por Visual Studio. Es buena práctica borrarla antes de una entrega. 

### Código bien indentado

Tabulas muy bien, lo cual parece un detalle extra cuando una recien comienza pero ayuda un monton a su legibilidad, y que lo hayas logrado en esta etapa es un gran mérito. 

En tu CSS el tabulado está perfecto, pero no dejas el espaciado correcto en cada orden. En lugar de escribir por ejemplo `.name{`, deja un espacio entre el nombre de la clase y la llave: `.name {`

### Comentarios que permiten mejorar la legibilidad del código

Perfecto. 

### Uso correcto de etiquetas semánticas

En general usas bien las etiquetas semánticas. Me llama la atención que hayas usado `div` para las tarjetas de Mis Conocimientos: yo diría que deberían ser `article`. Pero es el único detalle a comentar aquí (y hay quien podría discutirme que deberían ser divs)

### Buenos nombres de clases

Cumplido la mayoría de las veces: en otras ocasiones se nota que te rendiste. La clase "ul" o la clase "li" no tienen sentido, porque no nos referimos con las clases a qué elemento de html son, sino a qué rol cumplen en nuestra página. 

Cuando decimos que un nombre de clase debe ser descriptivo, lo decimos en un sentido funcional: qué rol cumple este elemento en el código. Los colores de los elementos, su etiqueta de html, su forma, su estilo, su posición, todas esas cosas pueden cambiar y efectivamente cambian todo el tiempo en las webs que hacemos. El botón que hoy es violeta mañana será azul; la sección que estaba primera mañana estará tercera. Por lo tanto esos factores sos no son buenos descriptores, y no deberían ser parte de nuestros nombres de clases.

### Código CSS bien estructurado

Cumplido, te dejo algunos comentarios en el archivo. 

### Reutilización de estilos

Cumplido

### Cumple con criterios básicos de accesibilidad

- Los colores tienen un contraste adecuado

Cumplido 

- Las imágenes tiene el atributo `alt` que corresponde

Cumplido, aunque con una minima observacion. Como vimos en clase el lector de pantalla dice "Imagen" antes de leerlo asi que agregar "esta imagen representa..." o "imagen de..." es repetitivo y una pesima experiencia para el usuario. 

- Los íconos y elementos que no presentan texto agregan la información correspondiente por otros medios (etiquetas aria, texto oculto)

Como vimos, el lector de pantalla ignora los iconos a menos que les agreguemos role="img", asi que tus arias podrian no estar y no haria ninguna diferencia. 

- Los íconos y elementos que no necesitan ser anunciados por un lector de pantalla tienen la etiqueta aria
  correspondiente

No veo un caso donde lo uses, pero tampoco creo que lo necesites. 

- Commits con mensajes adecuados

Cumplido, noto muchos y buenos commits en tu proyecto, lo que siempre se agradece.

- Cuenta con un favicon

Cumplido, aunque debería estar en la carpeta principal

### Nota: 9
