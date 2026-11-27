# Documentación del proyecto Limpia-Mar

| Archivo | Contenido |
|---|---|
| [SRS.md](SRS.md) | Especificación de requerimientos (SRS v1.0). |
| [investigacion-srs.md](investigacion-srs.md) | Investigación sobre el SRS con referencias APA 7. |
| [casos-de-uso.md](casos-de-uso.md) | Diagrama de casos de uso general del sistema. |
| [clases-modulo.md](clases-modulo.md) | Diagrama de clases del módulo del equipo. |

## Modelado UML

**Herramienta:** Mermaid. La elegimos porque GitHub dibuja los diagramas directamente dentro de los archivos `.md`, sin exportar imágenes, y porque cada cambio queda registrado en el historial de commits.

### Diagrama de casos de uso general
Muestra todo lo que el **Jugador** puede hacer en Limpia-Mar: ver el menú, leer cómo jugar, elegir nivel, jugar, pausar, ver resultados y consultar récords. El **Sistema de récords** es un actor secundario que guarda los puntajes.
- El rectángulo marca el **límite del sistema**: lo que está adentro es lo que el juego hace.
- «include»: jugar un nivel siempre incluye mover a Aspi y recoger basura.
- «extend»: la penalización por pez y la pausa solo pasan en ciertas condiciones.

### Diagrama de clases del módulo: Jugabilidad del laberinto
Nuestro equipo modela el **módulo de jugabilidad**, que es el corazón del juego: el laberinto, los personajes que se mueven en él (Aspi y los peces), la basura y el marcador.
- **Herencia:** `Aspi` y `Pez` heredan de la clase abstracta `Personaje`, porque los dos tienen posición y se mueven por el laberinto.
- **Composición:** un `Nivel` tiene su `Laberinto`; sin el nivel, el laberinto no existe.
- **Agregación:** el nivel tiene peces y basura que aparecen y desaparecen durante la partida.
- Las clases se programarán en **Python con pygame**; las que se dibujan heredan de `pygame.sprite.Sprite`.

**Equipo:** Álvaro Getzemani Hernández Sánchez (Getze) y Gonzalo David Martínez Medina (David).
