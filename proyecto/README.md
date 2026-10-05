# Proyecto: Brechas en Saber 11 entre colegios oficiales y privados

## Pregunta de análisis
¿Existen diferencias en los resultados de las pruebas Saber 11 entre estudiantes de colegios oficiales y privados en Colombia, y cómo varían esas brechas por territorio y periodo?

El análisis busca identificar diferencias de desempeño que puedan servir como insumo para priorizar intervenciones educativas y orientar decisiones sobre apoyo académico y asignación de recursos.
 
## Fuente de datos
• Conjunto: Resultados únicos Saber 11.
• Enlace: https://www.datos.gov.co/Educaci-n/Resultados-nicos-Saber-11/kgxf-xxbe
• Entidad: Instituto Colombiano para la Evaluación de la Educación (ICFES).
• Portal: Datos Abiertos Colombia.
• Licencia: la ficha web consultada no muestra una licencia específica; se verificará en los metadatos del conjunto antes de la entrega final del proyecto.
• Actualización: la vista pública consultada reporta datos actualizados al 23 de agosto de 2023 y metadatos actualizados el 18 de mayo de 2026.
 
## Variables previstas
• PERIODO: periodo de presentación de la prueba.
• COLE_NATURALEZA: naturaleza del establecimiento educativo, variable principal para distinguir colegios oficiales y privados.
• COLE_DEPTO_UBICACION: departamento donde está ubicado el establecimiento.
• COLE_MCPIO_UBICACION: municipio donde está ubicado el establecimiento.
• Puntajes de Saber 11: puntajes disponibles por componente, como Matemáticas, Inglés y Sociales y Ciudadanas, además del indicador global cuando esté disponible en el conjunto.

Con estas variables se calcularán promedios y diferencias de puntaje entre colegios oficiales y privados, con comparaciones por periodo y territorio.
 
## Herramientas del curso
Se utilizará pandas para cargar, limpiar, filtrar, agrupar y resumir los datos. Su estructura tabular permite comparar los resultados por naturaleza del colegio, periodo y ubicación geográfica mediante operaciones reproducibles de agrupación y agregación.

Docker se utilizará para fijar el entorno de ejecución y las versiones de las dependencias, de manera que el análisis pueda reproducirse en distintas máquinas con la misma configuración.
 
## Cómo reproducir
docker build --tag proyecto:0.1 proyecto/
docker run --rm proyecto:0.1



