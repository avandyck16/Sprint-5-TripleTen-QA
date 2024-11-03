## Urban Lunch - Sprint 5
## Pruebas de App Móvil
### Axel Van Dyck, Grupo 14


## Descripción General
Durante este sprint, se realizaron pruebas exhaustivas en la aplicación móvil Urban.Lunch, enfocándose en las validaciones del sistema y las notificaciones de error en diversas funcionalidades clave. Estas pruebas incluyeron la selección del punto de recogida, elección de platillos, confirmación y seguimiento de pedidos, y mensajes de estado de entrega. Además, se documentaron los resultados de las pruebas en entornos específicos de dispositivos Android y se destacaron áreas grises y ambigüedades en los requisitos y diseños del proyecto.

## Tareas Realizadas

### Validaciones del Sistema y Notificaciones de Error
Se realizaron pruebas sobre diversas validaciones de la aplicación y casos de notificaciones de error para asegurar que los mensajes de estado y errores se comportaran correctamente. Las validaciones se organizaron en las siguientes categorías:

1. **Selección del Punto de Recogida**
   - Verificación de que la selección del punto de recogida funcione de acuerdo con los requisitos.

2. **Elección de Platillos**
   - Validación de que los usuarios puedan seleccionar platillos sin errores, incluso en casos extremos como cantidades grandes.

3. **Confirmación del Pedido**
   - Revisión de las condiciones para la confirmación del pedido y comportamiento esperado.

4. **Seguimiento de Pedidos**
   - Confirmación de que la función de seguimiento del pedido se muestre correctamente hasta la entrega.

5. **Entrega del Pedido**
   - Verificación de la notificación de entrega y cualquier mensaje de error asociado.

### Notificaciones de Error
A continuación, algunos ejemplos de los mensajes de error probados:

| Descripción | Estado | Enlace al informe de errores |
|-------------|--------|------------------------------|
| Aparece un mensaje de error si no permites que la aplicación acceda a la geolocalización (GPS). | APROBADO | N/A |
| No aparece un mensaje de error si permites que la aplicación acceda a la geolocalización (GPS). | APROBADO | N/A |
| Se muestra un mensaje de error si desactivas la geolocalización mientras usas la app. | NO APROBADO | [ULA-1](https://axelvandyck.atlassian.net/browse/ULA-1) |
| Aparece un mensaje de error si intentas hacer un pedido sin agregar ningún platillo. | APROBADO | N/A |
| No aparece un mensaje de error si intentas hacer un pedido al agregar un platillo. | APROBADO | N/A |
| No aparece un mensaje de error si intentas hacer un pedido al agregar una cantidad larga de platillos. | APROBADO | N/A |

---

## Entorno de Prueba
Las pruebas se realizaron en un dispositivo Android con las siguientes especificaciones:

| Fabricante y Modelo       | Resolución | Tamaño de Pantalla | S.O.              | Versión           | Build Number          | Procesador                             | USB Debugging | Acceso Root | Capacidad de Almacenamiento | Memoria | Conexión WIFI | Conexión LTE |
|---------------------------|------------|--------------------|-------------------|-------------------|-----------------------|----------------------------------------|---------------|-------------|-----------------------------|---------|---------------|-------------|
| Motorola Moto G34 5G      | 720x1600   | 6.52"             | Android 14       | Upside Down Cake API34 | U1UG34.23-28-2     | Qualcomm SM6375 Snapdragon 695 5G (6 nm) | Sí            | No          | 128 GB                      | 8 GB    | Sí            | Sí          |

Logs extraídos a través de **Android Studio**.

---

## Conclusiones y Observaciones
**Zonas Grises:**
- No está claro si el “punto de recogida” debe seleccionarse de la lista de restaurantes o si permite una selección libre por el usuario. Sería recomendable especificar que los puntos de recogida son otros restaurantes de la lista.
- La descripción de los requisitos y la lógica en el documento y en Figma son confusas; el video del proyecto ofrece una comprensión más amplia, que difiere de los requisitos escritos y los diseños.

---

Este README documenta el enfoque de prueba, las configuraciones del entorno, los resultados obtenidos, y las conclusiones sobre los requisitos, brindando una visión detallada del Sprint 5.
