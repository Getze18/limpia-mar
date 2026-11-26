# Investigación: el SRS (Especificación de Requerimientos de Software)

**Proyecto:** Limpia-Mar
**Equipo:** Álvaro Getzemani Hernández Sánchez y Gonzalo David Martínez Medina

| Pregunta | Investigó |
|---|---|
| 1. ¿Qué es un SRS/ERS y qué problemas evita? | Álvaro |
| 2. ¿Qué secciones propone IEEE 830? | Álvaro |
| 3. ¿Qué hace bueno a un requerimiento? | Gonzalo |
| 4. ¿Qué plantillas y herramientas existen? | Gonzalo |

---

## Resumen de hallazgos

**1. Qué es un SRS y qué problemas evita.** El SRS (en español ERS, Especificación de Requerimientos de Software) es el documento que describe qué debe hacer un sistema y bajo qué condiciones, sin decir cómo se programa (IEEE, 1998). Funciona como acuerdo entre el cliente y el equipo de desarrollo. Evita malentendidos sobre lo que se pidió, cambios tardíos que salen caros, funciones que nadie pidió y discusiones sobre si el producto está "terminado", porque da una base para probar (Sommerville, 2011; Wiegers & Beatty, 2013).

**2. Secciones de IEEE 830.** El estándar propone tres partes (IEEE, 1998):
1. *Introducción:* propósito, alcance, definiciones y glosario, referencias y visión general del documento.
2. *Descripción general:* perspectiva del producto, funciones principales, características de los usuarios, restricciones, supuestos y dependencias.
3. *Requerimientos específicos:* funcionales, de interfaz, de rendimiento, de diseño y atributos de calidad.

IEEE 830 fue reemplazado por ISO/IEC/IEEE 29148 (2018), que conserva la misma idea, pero sigue siendo la estructura más usada en cursos por ser sencilla.

**3. Características de un buen requerimiento.** Debe ser correcto, no ambiguo (una sola interpretación), completo, consistente (no contradice a otro), priorizado, verificable (se puede probar) y rastreable (IEEE, 1998; ISO/IEC/IEEE, 2018).
- ❌ *Malo:* "Los peces deben ser difíciles de esquivar." (¿Qué tan difíciles? No se puede probar.)
- ✅ *Bueno:* "Si Aspi toca un pez, el sistema resta 100 puntos y muestra el aviso '¡Cuidado con los peces!'." (Se prueba tocando un pez y revisando el marcador.)

**4. Plantillas y herramientas.**
- *Plantillas:* IEEE 830, ISO/IEC/IEEE 29148, Volere (Robertson & Robertson, 2012) e historias de usuario con criterios de aceptación en métodos ágiles (Pressman & Maxim, 2020).
- *Herramientas para escribir y versionar:* Markdown en GitHub (versiones con commits y seguimiento con Issues), Google Docs o Word (historial de cambios) y herramientas especializadas como Jira o IBM DOORS para proyectos grandes.

## Plantilla elegida

Usaremos **IEEE 830 adaptada a Markdown**, con cada requerimiento en una ficha (ID, título, descripción, prioridad y criterio de aceptación).

**Justificación:** tiene las secciones 1 a 3 que pide la actividad, es corta para un equipo de dos personas, y al estar en Markdown vive en GitHub junto al código: cada cambio queda en un commit y cada requerimiento funcional se liga a un Issue del tablero.

## Declaración de uso de IA generativa

Usamos un asistente de IA generativa (Claude, de Anthropic) para **organizar el resumen y proponer un primer borrador** de los ejemplos de requerimientos. Revisamos las definiciones, las secciones de IEEE 830 y las características de un buen requerimiento contra las fuentes de abajo, y adaptamos el texto a nuestro proyecto.

## Referencias (APA 7)

IEEE. (1998). *IEEE recommended practice for software requirements specifications* (IEEE Std 830-1998). https://doi.org/10.1109/IEEESTD.1998.88286

ISO/IEC/IEEE. (2018). *Systems and software engineering — Life cycle processes — Requirements engineering* (ISO/IEC/IEEE 29148:2018). https://doi.org/10.1109/IEEESTD.2018.8559686

Pressman, R. S., & Maxim, B. R. (2020). *Software engineering: A practitioner's approach* (9th ed.). McGraw-Hill Education.

Robertson, S., & Robertson, J. (2012). *Mastering the requirements process: Getting requirements right* (3rd ed.). Addison-Wesley.

Sommerville, I. (2011). *Ingeniería de software* (9.ª ed.). Pearson Educación.

Wiegers, K., & Beatty, J. (2013). *Software requirements* (3rd ed.). Microsoft Press.
