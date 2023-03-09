# Simple-Alert
Simple alerta para páginas webs hecho en JavaScript y CSS.
***  
![ezgif com-video-to-gif](https://user-images.githubusercontent.com/75407068/221650829-351c072f-2ee1-4a01-9fa2-769a29415dc8.gif)

***  
### <ins>Modo de uso:</ins>  

Las alertas se invocarán con el llamado a la función: <code>alertaokgo(msg, color, tiempo)</code>, en donde:  
- <ins>Msg</ins>: Mensaje que contendrá la alerta.
- <ins>Color</ins>: Color que contendrá la alerta.  
    Para usar una alerta predefinida como en el video, ingrese uno de los siguientes 3 textos: <code>info</code>, <code>error</code>, <code>success</code>.
- <ins>Tiempo</ins>: Tiempo que se mostrará la alerta. (En milisegundos).

Cabe recalcar que los parámetros: <code>msg</code> y <code>color</code> deberán ser ingresados entre comillas.  
#### <ins>Ejemplo de alerta:</ins>  
```javascript
alertaokgo("Ingrese un valor válido", "#FFB600", 3000)
```
![Captura](https://user-images.githubusercontent.com/75407068/221650680-facbafc8-5e76-4279-950b-9e600c3b8f4c.PNG)
***
### <ins>Instalación:</ins>  
- <ins>1</ins>: Clone o descargue los archivos del repositorio en la carpeta raiz de su proyecto.  
- <ins>2</ins>: Añada el siguiente código CSS en su archivo de estilos:  
```css
@import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');

.okalert{
    position: fixed;
    display: flex !important;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    opacity: 0;
    pointer-events: none;
    z-index: 20;
    justify-content: flex-end;
    align-items: flex-end;
  }
  
  #alert{
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 15px;
    color: white;
    font-size: 17px;
    z-index: 20;
    font-family: "Roboto";
    font-weight: 100;
    margin: 0 50px 30px 0;
    padding: 15px 20px;
    position: relative;
    left: 300px;
    box-shadow: 5px 5px 20px rgb(0, 0, 0);
  }
  ```  
  o agréguelo como un archivo separado e impórtelo en su head: 
  ```html
  <link href="/style.css" rel="stylesheet" type="text/css">
  ```  
  ___
  - <ins>3</ins>: Añada el siguiente código justo antes de ```</body>```:  
  ```html
    <script src="/alerta.js"></script>
    <section class="okalert">
        <div id="alert"></div>
    </section>
  ```
