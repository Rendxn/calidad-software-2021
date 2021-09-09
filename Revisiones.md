# Revisiones

Las revisiones hacen una parte importante dentro del ciclo de vida de desarrollo de software, pues permiten encontrar defectos en una etapa temprana y reducen costos.
En conformidad con el estándar IEEE 1028-2008, el plan de revisión consta de los siguientes items.

## Responsabilidades

* Tomador de decisiones: Juan Carlos Jaramillo Gómez
* Líder de revisión: Santiago Espinosa Arteaga
* Registrador: Sebastián Rendón Giraldo
* Personal administrativo: Salomé Aristizábal Giraldo
* Personal técnico: Juan Carlos Jaramillo Gómez
* Representante del cliente: Edward

## Revisión de los requisitos de software (SRR)

### Producto de software

Especificación de requisitos de software (SRS).

### Objetivos

* Evaluar conformidad del documento de especificación de requisitos de software a las especificaciones.
* Encontrar anomalías en las especificaciones de requisitos de software.
* Elaborar una lista de acciones correctivas.
* Reportar resultados de la revisión.

### Evaluación de entrada

Se realizará la evaluación del producto mediante una [lista de verificación y validación de especificación de requisitos](https://www.cs.toronto.edu/~sme/CSC340F/2005/assignments/inspections/reqts_checklist.pdf). Este consiste en evaluar el producto de software utilizando una lista de verificación dividida en diferentes criterios, asegurándose de que el producto cumpla con las especificaciones.

La lista de verificación es la siguiente.

1. Organización y completitud

   * ¿Son correctas todas las referencias cruzadas a otros requisitos?
   * ¿Están todos los requisitos escritos a un nivel consistente y apropiado de detalle?
   * ¿Proveen los requisitos una base adecuada para el diseño?
   * ¿Está incluida la prioridad de implementación para cada requisito?
   * ¿Están definidas todas las interfaces de comunicación, software y hardware externo?
   * ¿Se han definido algoritmos intrínsecos a los requisitos funcionales?
   * ¿La especificación incluye todas las necesidades conocidas del cliente o del sistema?
   * ¿Se documenta el comportamiento esperado para todas las condiciones de error anticipadas?

2. Correctitud

   * ¿Hay requisitos duplicados o conflictos entre los requisitos?
   * ¿Está cada requisito escrito en un lenguaje claro, conciso y sin ambigüedad?
   * ¿Es cada requisito verificable mediante pruebas, demostración, revisión o análisis?
   * ¿Está cada requisito dentro del alcance del proyecto?
   * ¿Tienen los requisitos errores de redacción?
   * ¿Falta información para algún requisito (no contemplada)?
   * ¿Se pueden implementar todos los requisitos dentro de las limitaciones conocidas?
   * ¿Los mensajes de error especificados son únicos y significativos?

3. Atributos de Calidad

   * ¿Están todos los objetivos de rendimiento debidamente especificados?
   * ¿Están todas las consideraciones de seguridad y protección debidamente especificadas?
   * ¿Se documentan y cuantifican otros objetivos de atributos de calidad pertinentes?

4. Trazabilidad

   * ¿Se identifica cada requisito de forma única y correcta?
   * ¿Se puede rastrear cada requisito funcional de software a un requisito de nivel superior (por ejemplo, requisito del sistema, caso de uso)?

## Revisión de diseño preliminar (PDR)

### Productos de software

Descripción de diseño de software (SDD).
Documento de diseño de interfaces (IDD).

### Objetivos

* Evaluar la adecuación técnica del diseño preliminar de software representados en el SDD y el IDD.
* Encontrar anomalías en el diseño preliminar de software.
* Elaborar una lista de acciones correctivas.
* Reportar resultados de la revisión.

### Evaluación de entrada

Se evaluará la correctitud, completitud, legibilidad y testabilidad de los elementos de diseño de software (SDD; IDD) siguiendo los criterios establecidos en el estándar IEEE 1012-2016.

1. Correctitud:

    * ¿Están correctamente relacionados los elementos de diseño con los respectivos requisitos de software?
    * ¿El diseño de software satisface los requisitos de software?
    * ¿El diseño de software cumple con las reglas de negocio, estándares, referencias, regulaciones y políticas?
    * ¿Las secuencias de diseño representan correctamente los estados, cambios de estado y el flujo de la aplicación en general?
    * ¿La interacción entre elementos de diseño no presenta efectos secundarios?
    * ¿El flujo de datos y control satisfacen los requisitos de funcionalidad y rendimiento?

2. Consistencia

    * ¿Todos los términos y conceptos de diseño están documentados correctamente?
    * ¿Hay consistencia entre los elementos de diseño y el diseño de la arquitectura?

3. Completitud

    * ¿Están presentes en el SDD los elementos de funcionalidad (algoritmos, estados, validaciones, manejo de excepciones)?
    * ¿Están presentes en el SDD las descripciones de hardware, software e interfaz de usuario?
    * ¿Se especifican en el SDD métricas de rendimiento?
    * ¿Están presentes en el SDD los elementos de control de software, hardware y del sistema?
    * ¿Tanto el SDD como el IDD satisfacen procedimientos de gestión de configuración especificados?

4. Legibilidad

    * ¿La documentación es legible, entendible y sin ambigüedad?
    * ¿La documentación define acrónimos, términos, lenguaje de diseño, entre otros?

5. Testabilidad

    * ¿Hay criterios de aceptación objetivos para cada elemento de diseño?
    * ¿Se puede probar cada elemento de diseño según los criterios de aceptación?

## Revisión de diseño crítico (CDR)

### Productos de software

Descripción de diseño de software (SDD).
Documento de diseño de interfaces (IDD).

### Objetivos

* Determinar si el diseño detallado completo cumple con los requisitos especificados (funcional/rendimiento).
* Determinar si el diseño está completo y listo para ser implementado.
* Reasignar requisitos y ajustar diseños en los casos necesarios para preservar la consistencia.

### Evaluación de entrada

Se evaluará la correctitud, consistencia, completitud y legibilidad de los elementos de diseño utilizando la siguiente lista de verificación y validación.

1. Correctitud:

    * ¿Los elementos de diseño cumplen con los respectivos requisitos de software referentes a la funcionalidad y al rendimiento?
    * ¿Las interfaces internas cumplen con los respectivos requisitos de software referentes a la funcionalidad y al rendimiento?
    * ¿Las interfaces externas cumplen con los respectivos requisitos de software referentes a la funcionalidad y al rendimiento?

2. Consistencia:

   * ¿Hay consistencia entre los elementos de diseño y los requisitos especificados?
   * ¿Hay consistencia entre los elementos de diseño y el diseño de la arquitectura?

3. Completitud:

   * ¿Todos los elementos de diseño están completos?
   * ¿Todos los elementos de diseño fueron probados y cumplieron con sus criterios de aceptación?
   * ¿Tanto el SDD como el IDD satisfacen procedimientos de gestión de configuración especificados?

4. Legibilidad

    * ¿La documentación es legible, entendible y sin ambigüedad?
    * ¿La documentación define acrónimos, términos, lenguaje de diseño, entre otros?

---

Para cada producto de software se deberán incluir los objetivos de la revisión y la evaluación de entrada, además de una planeación de la revisión; preparación; examen y salida. Estas últimas se explican a continuación.

### Preparación administrativa

Previo a la examinación, el personal administrativo se encargará de que la revisión del producto de software contenga todos los recursos necesarios para seguir adelante con la revisión. Se tendrán en cuenta.

* Personal
* Tiempo
* Materiales (artefactos, documentos).
* Herramientas (listas de verificación).

## Planeación de la revisión

Basado en estos objetivos, el líder de revisión será el encargado de realizar las siguientes actividades.

1. Identificar el equipo de revisión.
2. Asignar las responsabilidades a los miembros del equipo de revisión.
3. Agendar y anunciar el lugar de la reunión.
4. Distribuir los materiales con tiempo previo.
5. Establecer un calendario para la distribución de material y la devolución y envío de comentarios.

## Preparación

Cada miembro del equipo es responsable de preparar la tarea de revisión de la que fue encargado.

## Examen

Utilizando las herramientas seleccionadas para la revisión, se determinará si.

 1. El producto de software está completo.
 2. El producto de software se conforma con los estándares, regulaciones y especificaciones.
 3. Es necesario aplicar cambios al producto de software en caso de ser necesario.
 4. El producto de software es adecuado.
 5. Los descubrimientos requieren modificar el calendario del proyecto.

Seguido de esto, se identificarán las anomalías y su prioridad y se realizará una lista de acciones a tomar.

Toda esta información debe ser documentada para la salida de la revisión y entregada una vez se considere que las actividades fueron hechas.

## Salida

La salida de la revisión técnica consistirá de la siguiente información.

1. Información general de la entrada (nombre del proyecto, miembros del equipo, producto, completitud de los objetivos).
2. Documentación de la revisión.
3. Lista de anomalías del producto de software.
4. Lista de problemas de gerencia.
5. Lista de acciones y su estado actual (abierta, resuelta).
6. Recomendaciones adicionales del equipo de revisión.

## Plan de Revisión de la Validación y Verificación de Software
