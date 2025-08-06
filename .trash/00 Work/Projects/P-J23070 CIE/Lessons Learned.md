# `= this.file.link`
>[!Properties]- | `= this.Parent.Parent.Parent.Parent` |  `= this.Parent.Parent.Parent` | `= this.Parent.Parent` | `= this.Parent` | `= this.file.link` |`BUTTON[note]` 
>Version:: 2.1
>Parent:: [[P-J23070 CIE]]
>Tags: #Notes
```meta-bind-embed
[[Search note]]
```
Source::
Related To::
***
# Body:

Buenas Carlos,

Quería aprovechar, para dar un poco de feedback constructivo de cositas que se podrían mejorar.

Hay cosas que no dependen de ti directamente y quizás no puedas hacer nada, pero quería reflejarlas.

- Identificar postes de Tool Stand con un 1 y un 2
- Identificar bayonetas con un 1 y un 2 à Por lo que me comento Rodri, mejor no mezclar las bayonetas con los TS ya que no son exactamente iguales
- Bumpers DKT se pasivan muy fácilmente à Se Deberían hacer pruebas en el taller, para ver si es un problema del sensor, ajuste mecánico o de parametrización.
- Punto inserción Cámara Visión   à El nuevo software de la Cognex, permite editar el punto de inserción, pero no hay ningún punto de referencia donde colocarlo à En el VCNV en un rincón del área de visión se debería poner una pequeña diana, para colocar el punto de inserción de forma repetible.
- No tengo claro para que y como usar la fotocélula de inicio del ECNV
- El Cartel de “Leds” del EOL, Lo ideal sería a ver probado en el taller/ buyoff para no perder tiempo de instalación aprendiendo como funciona y haciendo experimentos.
- El Tablero de Calibración de la Cámara, estaba partido justo por la marca fiducial, se tenía que mantener una distancia concreta entre tableros.  à Si es posible mejor en una pieza, o una pieza central y extensiones en los laterales.
- El Tablero de Calibración de la Cámara estaría bien tener una forma de posicionarlo repetidamente en el mismo sitio
- El Power Point y material de Formación se debería revisar y darle una vuelta. Es muy denso, faltan imágenes y es difícil de seguir.
- Sergio Debería haber continuado con el proyecto en lugar de involucrar a innova, cuantas menos manos mejor.
- En la Puerta enrollable de SMT hay una foto barrera que no es utilizada, ya que las maquinas solo se mueven en manual, no tienen opción de automático.
- Expectativas del cliente, cliente tenía la impresión de que después del Ghost mode ya toda funcionaria a la primera. (ya se que es un cliente especial)

- **Mi propuesta:**

1. Pre- aceptación de línea, todo el material instalado y probado à Después de Safety test y Ghost mode.
2. Primeras 1000 piezas de la primera referencia al ritmo de ABB para debugar y estabilizar. Siguientes Referencias 250-500 piezas para Fiabilizar.
3. Inicio Seguimiento
4. Puntos Abiertos
5. Aceptación

**Problemas Estándar PLC Y Robot: (No debería a ver problemas, pero hay muchos)**

- Secuencia ATC ( PLC y Robot)
- HMI en general
- OTAs
- IO con programa de visión
- Multiplicar coordenadas de visión para gestionar decimales, robot no preparado.
- Variables de visualización Flex pendant R1 no se escriben ( PLC)
- Exportar he importar recetas de PLC
- Robot a PLC Activar vacío =1 à Si se apaga Robot con pieza esta cae, ya que se pierde la señal, se debería invertir en Robot y PLC

**Puntos Positivos:**

- El equipo tanto de ABB es como MEX
- Comunicación con Oficina
- Electricista de “Naucal”, muy profesional.

Cualquier feedback sobre mi trabajo es bienvenido,

Muchas Gracias por todo Carlos.







# Foot
```meta-bind-embed
[[Foot note]]
``` 