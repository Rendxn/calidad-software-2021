# Revisiones

Las revisiones hacen una parte importante dentro del ciclo de vida de desarrollo de software, pues permiten encontrar defectos en una etapa temprana y reducen costos.
En conformidad con el estándar IEEE 1028-2008, el plan de revisión consta de los siguientes items:

## Responsabilidades

* Tomador de decisiones: Juan Carlos Jaramillo Gómez
* Líder de revisión: Santiago Espinosa Arteaga
* Registrador: Sebastián Rendón Giraldo
* Personal administrativo: Salomé Aristizábal Giraldo
* Personal técnico: Juan Carlos Jaramillo Gómez
* Representante del cliente: Edward

## Revisión de los requisitos de software (SRR)

### Objetivos

* Evaluar conformidad del documento de requisitos de Software (SRD) a las especificaciones.

### Producto de software

Documento de requisitos de software.

### Procedmientos de revisión

Se realizará la evaluación del producto mediante una [lista de verificación de especificación de requisitos](https://www.cs.toronto.edu/~sme/CSC340F/2005/assignments/inspections/reqts_checklist.pdf). Este consiste en evaluar el producto de software utilizando una lista de verificación dividida en diferentes criterios, asegurándose de que el producto cumpla con las especificaciones.

La lista de verificación es la siguiente:

#### Organización y completitud

* ¿Son correctas todas las referencias cruzadas a otros requisitos?
* ¿Están todos los requisitos escritos a un nivel consistente y apropiado de detalle?
* ¿Proveen los requisitos una base adecuada para el diseño?
* ¿Está incluida la prioridad de implementación para cada requisito?
* ¿Están definidas todas las interfaces de comunicación, software y hardware externo?
* ¿Se han definido algoritmos intrínsecos a los requisitos funcionales?
* ¿La especificación incluye todas las necesidades conocidas del cliente o del sistema?
* ¿Se documenta el comportamiento esperado para todas las condiciones de error anticipadas?

#### Correctitud

* ¿Hay requisitos duplicados o conflictos entre los requisitos?
* ¿Está cada requisito escrito en un lenguaje claro, conciso y sin ambigüedad?
* ¿Es cada requisito verificable mediante pruebas, demostración, revisión o análisis?
* ¿Está cada requisito dentro del alcance del proyecto?
* ¿Tienen los requisitos errores de redacción?
* ¿Falta información para algún requisito (no contemplada)?
* ¿Se pueden implementar todos los requisitos dentro de las limitaciones conocidas?
* ¿Los mensajes de error especificados son únicos y significativos?

#### Atributos de Calidad

* ¿Están todos los objetivos de rendimiento debidamente especificados?
* ¿Están todas las consideraciones de seguridad y protección debidamente especificadas?
* ¿Se documentan y cuantifican otros objetivos de atributos de calidad pertinentes?

#### Trazabilidad

* ¿Se identifica cada requisito de forma única y correcta?
* ¿Se puede rastrear cada requisito funcional de software a un requisito de nivel superior (por ejemplo, requisito del sistema, caso de uso)?
