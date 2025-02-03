<table>
  <tr>
    <td>
      <h1>Laboratorio No. 02 - Robótica Industrial</h1>
      <h2> Análisis y Operación del Manipulador Motoman MH6 </h2>
      <h3> Comparativa y Aplicaciones Prácticas </h3>
      <strong> Autores:</strong>
      <ul>
        <li>Daniel Mauricio Rivero Lozada </li>
        <li>Yeira Liseth Rodríguez Rodríguez</li>
      </ul>
    </td>
    <td>
      <img src="Images/Portada.jpeg" width="400">
    </td>
  </tr>
</table>

## Comparación Motoman MH6 y IRB ABB 140.

El Motoman MH6 es un robot versátil con un amplio alcance y alta velocidad, ideal para tareas como soldadura, manipulación de materiales y recubrimiento. Por otro lado, el ABB IRB 140 es un robot compacto con alta precisión y repetibilidad, adecuado para aplicaciones de ensamblaje, carga y descarga de máquinas y pulido.

<p align="center">
  <a href="url4"><img src="Images/TablaComparativa.png" width="200"></a>
</p>

Por otro lado, también hay un cambio en el espacio de trabajo de ambos robots

### Motoman MH6.

<p align="center">
  <a href="url4"><img src="Images/EspacioMotomanMH6.png" width="200"></a>
</p>

### ABB IRB 140

<p align="center">
  <a href="url4"><img src="Images/EspacioABBIRB140.png" width="200"></a>
</p>

La información anteriormente mostrada fue extraida de :
* https://www.yaskawa.fr/yaskawa.fr/Robots%20d%27occasion/Brochures/Flyer_Robot_MH6-10_E_06.2014.pdf
* https://library.e.abb.com/public/a7121292272d40a9992a50745fdaa3b2/3HAC041346%20PS%20IRB%20140-en.pdf

## Posiciones Home1 y Home2 del Motoman MH6.

Las configuraciones de Home1 y Home2 son posiciones de inicio con ligeras variaciones. En el primero se dispone del robot completamente extendido, es decir, los ángulos de sus articulaciones son todas cero. Por otro lado, para home2 se encuentra un cambio en las articulaciones 2 y 3 con ángulos de 45° y -45° respectivamente. Esto permite una posición más compacta del robot. 

<p align="center">
  <a href="url4"><img src="Images/PosicionesHome.png" width="200"></a>
</p>

La posición dependerá de la situación, en general se prefiere la segunda por la reducción del espacio ocupado y los riesgos de colisión. La primera posición es más usada para casos de mantenimiento, es decir, es útil calibraciones y diagnósticos iniciales.

## Procedimiento movimientos manuales

Los movimientos manuales en el Motoman MH6 se realizar de modo articular (moviendo cada articulación individualmente) o en modo cartesiano (trasladando o rotando el efector final en un sistema de coordenadas XYZ).

<p align="center">
  <a href="url4"><img src="Images/TeachPendant.jpg" width="200"></a>
</p>

El procedimiento es el siguiente

<ul>
  <li>Después de que el robot está encendido, segurarse de que está en modo manual ( Teach Mode) </li>
  <li>Girar la llave de habilitación en el Teach Pendant a la posición "Teach" </li>
  <li>Presionar el botón "Enable" en el Teach Pendant</li>
  <li>Presionar botón "Coordinate" y seleccionar el modo deseado (Joint - JNT o Cartesian - XYZ)</li>
  <li>Dependiendo del modo seleccionado seleccionar los botones para el movimiento deseado: para movimiento articular ±S, ±L, ±U, ±R, ±B, ±T, y para movimiento cartesiano ±X, ±Y, ±Z, (traslación) ±RX, ±RY, ±RZ (movimiento) </li>
  <li>Mantener presionado "Enable" y mover en la dirección deseada hasta alcanzar la posición requerida.</li>
</ul>

<p align="center">
  <a href="url4"><img src="Images/BotonesTeachPendant.jpg" width="200"></a>
</p>






