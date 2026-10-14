# VirologIA

Aprende virología molecular practicando: clasifica virus, ordena sus ciclos, calcula como en el laboratorio, ensaya el examen y resuelve casos. Aplicación web de un solo fichero para la asignatura de **Virología (1394) del Grado en Biotecnología de la Universidad Miguel Hernández de Elche**.

**Usar la app:** https://fborrasumh.github.io/virologia/

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23361886.svg)](https://doi.org/10.5281/zenodo.23361886)

**Idiomas:** español (por defecto), inglés y portugués; selector en la barra superior (o `?lang=en` / `?lang=pt` en la URL).

## Qué hace

Sigue las unidades U1–U6 de la guía docente 2026-2027.

- **Clasifica y repasa (U1, U2, U4).** 24 virus para situar en los 8 grupos de genoma de la guía (con su grupo de Baltimore), con envuelta o sin ella y con replicación en núcleo o citoplasma. El código corrige al momento y explica las excepciones (gripe en el núcleo, poxvirus en el citoplasma). Incluye 37 tarjetas de repaso del temario con repetición espaciada (cajas de Leitner).
- **Ordena los ciclos (U3, U4).** Seis ciclos para reconstruir paso a paso: ciclo lítico general, poliovirus, gripe A, VIH-1, hepatitis B y fago T4. El código cuenta las etapas bien colocadas y señala el primer error.
- **Laboratorio numérico (U1–U4).** Siete tipos de problema ligados a las prácticas: título por placas, MOI y Poisson, volumen para una MOI, número de triangulación T, DNA por A260 (fago λ), eficiencia de transformación y tamaño de explosión. Los datos salen del nombre o código del estudiante, así que el mismo código da siempre los mismos ejercicios. **La solución la calcula el código**, que muestra el desarrollo paso a paso y reconoce errores típicos (olvidar el volumen sembrado, contar una placa no fiable, confundir infectadas con no infectadas, el factor de RNA frente al de dsDNA, ng frente a µg…).
- **Simulacro de examen (U1–U5).** 16 preguntas de desarrollo con el formato de la guía: respuesta de una página, y una de ellas dividida en cinco minipreguntas. Hay temporizador opcional. La revisión **sin IA** indica qué conceptos clave aparecen. Con IA, se ve el estado de cada concepto (bien, incompleto, con error o ausente) y los errores conceptuales, con la frase exacta de la respuesta. **No hay nota**, como pidieron los autores de la idea.
- **Casos y tutor (U5, U6).** Cinco casos inspirados en las prácticas de aula: coronavirus emergente (PA1), filovirus (PA2), gripe pandémica (PA4), viruela y su erradicación (PA5) y el diseño de un vector viral para la retina. Cada caso tiene pistas progresivas, preguntas guía y un diagnóstico que corrige el código. Con IA, hay además un **tutor socrático**.
- **Mis apuntes (con IA).** Puedes subir apuntes, diapositivas o el manual (Word, PDF, PowerPoint o texto) y hacerles preguntas, o crear tarjetas de repaso.
- **Progreso.** Muestra los aciertos recientes por unidad y recomienda qué practicar después. Se exporta e importa en JSON (para cambiar de ordenador), en Word, y el historial del laboratorio en CSV.

## Cómo se usa la IA (opcional)

Todo lo anterior funciona sin clave, salvo el feedback con IA del simulacro, el tutor y "Mis apuntes". Para esas funciones cada persona usa su propia clave de OpenAI, Google Gemini o Anthropic Claude, que se guarda solo en su navegador. No hace falta servidor.

La regla es **la IA propone y el código comprueba**:

- Cada comentario de la IA sobre una respuesta lleva una cita literal de esa respuesta. Si la cita no aparece, el concepto se marca como "sin cita verificada" y el error se descarta.
- Si la IA escribe una nota o una puntuación, se le pide de nuevo el feedback. Si la nota persiste, el código la borra y lo avisa.
- El tutor **no recibe la solución del caso**. Además, el código borra cualquier frase suya que nombre la solución o diga cuál es la opción correcta.
- En "Mis apuntes", las citas se comprueban contra el material, se avisa de las cifras que no están en él y solo se guardan las tarjetas con una cita verificada.

## Privacidad

Respuestas, progreso, apuntes y clave se guardan solo en el navegador (IndexedDB y localStorage). Solo al usar una función con IA salen hacia el proveedor elegido las respuestas del simulacro, los mensajes al tutor o los apuntes, con los correos, DNI/NIE y teléfonos enmascarados. Antes del primer envío de cada sesión se muestra lo que va a salir y hay que confirmarlo. El nombre o código del laboratorio no sale del navegador.

## Límites

- El contenido base (virus, tarjetas, ciclos, preguntas y casos) es material de repaso redactado a partir del temario de la guía. **Puede contener errores u omisiones** y debe revisarlo el profesorado de la asignatura antes de recomendarlo. Ante cualquier duda, manda lo que digan el profesorado y la guía docente.
- La revisión sin IA solo busca palabras clave: no sabe si la explicación es correcta.
- La IA puede equivocarse al valorar un concepto. La comprobación de citas solo garantiza que la frase citada existe, no que el comentario sea acertado.
- El progreso es una orientación calculada con lo practicado, no una calificación.
- En los PDF no se leen las imágenes, y un PDF escaneado sin texto no sirve para "Mis apuntes".
- Se ha probado con una IA simulada (OpenAI, en español, inglés y portugués), no con claves reales.

## Autoría

Luis Pérez García-Estañ (Universidad Miguel Hernández de Elche), María del Mar Ortega-Villaizán (Universidad Miguel Hernández de Elche) y Fernando Borrás Rocher (Universidad Miguel Hernández de Elche).

**Origen de la idea:** idea y criterio docente de Luis Pérez García-Estañ y María del Mar Ortega-Villaizán, profesorado de Virología (asignatura 1394, Grado en Biotecnología, UMH). La app sigue el temario, las prácticas de aula y el formato de examen de su guía docente 2026-2027.

ORCID: Luis Pérez García-Estañ [0000-0003-4078-8763](https://orcid.org/0000-0003-4078-8763) · María del Mar Ortega-Villaizán [0000-0003-2065-0601](https://orcid.org/0000-0003-2065-0601) · Fernando Borrás Rocher [0000-0002-5519-4573](https://orcid.org/0000-0002-5519-4573)

## Cómo citar

Pérez García-Estañ, L., Ortega-Villaizán, M. M. y Borrás Rocher, F. (2026). *VirologIA* (v1.0.0) [Software]. DOI: [10.5281/zenodo.23361886](https://doi.org/10.5281/zenodo.23361886)

## Licencia

MIT. Véase [LICENSE](LICENSE).
