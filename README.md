# Gestión y Seguimiento de Préstamos 💼

## Descripción del Negocio 📝

Este negocio se centra en la gestión y seguimiento de préstamos. La base de datos proporciona una visión clara y detallada del estado actual de cada préstamo, desde información básica del cliente hasta detalles financieros y fechas importantes. El propósito principal es facilitar a los usuarios entender rápidamente si un préstamo está al día, tiene atrasos o ha sido completado. Esto permite un seguimiento efectivo de los pagos, identificando aquellos que pueden requerir acciones adicionales, evaluando el riesgo financiero asociado a los préstamos y apoyando la toma de decisiones estratégicas dentro de la institución. En resumen, el negocio se enfoca en proporcionar herramientas para la gestión eficiente de préstamos y la toma de decisiones informadas.

## Vista de la Base de Datos 🗄️

La vista `Vista_Prestamos_Estados_narrativa_1_Nuevos_Estado` se crea con el propósito de proporcionar una visión detallada y estructurada del estado actual de los préstamos. Incluye los siguientes campos:

- **ID_Prestamo, ID_Cliente, Nombre_Cliente, Apellido_Cliente, Lugar_Trabajo:** Información básica del cliente asociado al préstamo.
- **Ciudad, Región:** Datos geográficos del cliente obtenidos de la tabla CiudadesRD.
- **Monto_Prestamo, Tasa_Interes_Anual, Garantia, Valor_Garantia:** Detalles financieros y de garantía del préstamo.
- **Fecha_Inicio, Fecha_Termino:** Fechas importantes del préstamo, como el inicio y la fecha estimada de término.
- **Monto_Pagado, Saldo_Pendiente:** Información financiera sobre los pagos realizados y el saldo pendiente.
- **Estado_Pago:** Indica si el préstamo está pagado, pendiente o atrasado según la comparación de fechas y saldos.
- **Tiempo_del_Prestamo:** Presenta el tiempo transcurrido desde el inicio del préstamo en formato narrativo (años, meses, días).
- **Tiene_Atrasos:** Informa si el préstamo tiene atrasos, basado en la comparación entre la fecha de término estimada y la fecha actual.
- **Estado:** Clasifica el estado actual del préstamo en función de si tiene atrasos, y si los tiene, especifica si está "En Legal" (más de 3 meses de atraso) o "En Acuerdo de Pago" (menos de 3 meses de atraso); de lo contrario, indica "Normal (OK)".

## Propósito y Beneficios 🎯

- **Claridad en el Estado del Préstamo:** Facilita a los usuarios entender rápidamente si un préstamo está al día, tiene atrasos o ha sido completado.
- **Seguimiento de Pagos:** Permite gestionar y monitorear los préstamos de manera efectiva, identificando aquellos que pueden requerir acciones adicionales.
- **Análisis de Riesgos:** Ayuda a evaluar el riesgo financiero asociado a los préstamos, especialmente aquellos que están en situación de atraso prolongado ("En Legal").
- **Reportes y Decisiones Estratégicas:** Sirve de base para generar reportes y análisis que apoyen la toma de decisiones financieras y estratégicas dentro de la institución.

## Uso 🔧

Para utilizar esta base de datos, se debe tener acceso al sistema de gestión de base de datos correspondiente y ejecutar las consultas necesarias para acceder a la vista `Vista_Prestamos_Estados_narrativa_1_Nuevos_Estado`.

## Contribución 🤝

Las contribuciones son bienvenidas. Si desea contribuir a este proyecto, por favor envíe una solicitud de extracción detallando los cambios propuestos.

## Licencia ⚖️

Este proyecto está bajo la licencia [MIT](LICENSE).
