# Pinterest Media Analyzer (Analizador de Contenido Multimedia de Pinterest)

> 🔍 Herramienta frontend ligera con fines educativos y de investigación, que permite extraer metadatos de contenido público en Pinterest

🌐 Demostración en línea: [https://twittervideodownloaderx.com/pinterest_downloader_sp](https://twittervideodownloaderx.com/pinterest_downloader_sp)

---

## 📋 Descripción del Proyecto

Este proyecto ha sido desarrollado con fines educativos y de investigación técnica. Se trata de una utilidad frontend ligera diseñada para ayudar a desarrolladores y estudiantes a comprender cómo extraer metadatos estructurados (como etiquetas Schema.org y Open Graph) de páginas públicas de Pinterest, utilizando APIs web estándar como OEmbed.

> 🎯 Casos de uso recomendados:
> - Organización de materiales de estudio personales y recopilación de ideas
> - Práctica de desarrollo frontend e investigación sobre extracción de datos web
> - Aprendizaje sobre estructuras de metadatos multimedia
> - Archivado de contenido con permiso explícito de los titulares de derechos de autor

⚠️ **Aviso importante**: Esta herramienta solo funciona con **contenido accesible públicamente**. No está diseñada ni habilitada para acceder a contenido de Pinterest que requiera inicio de sesión, sea de pago o esté configurado como privado.

---

## �?Características Principales

- 🔗 **Reconocimiento Inteligente de Enlaces**: Detecta automáticamente URLs estándar de Pins de Pinterest, enlaces cortos y formatos móviles
- 🎬 **Soporte Multi-formato**: Extrae metadatos para videos MP4, animaciones WebM, imágenes JPG/PNG y otros formatos multimedia comunes
- 📐 **Visualización de Información de Resolución**: Muestra las opciones de resolución y formatos de archivo disponibles para una selección informada
- 📱 **Diseño Totalmente Responsivo**: Experiencia de usuario optimizada para escritorio, tablet y dispositivos móviles
- �?**Arquitectura Priorizando el Lado del Cliente**: La lógica principal de análisis se ejecuta en el navegador, reduciendo la dependencia del servidor y mejorando la velocidad de respuesta
- 🔐 **Diseño Respetuoso con la Privacidad**: No registra las URLs enviadas, no almacena resultados de análisis ni recopila datos personales de usuarios

---

## 🚀 Guía de Inicio Rápido

1. Abra la aplicación o sitio web de Pinterest y localice el **contenido público** que desea consultar
2. Copie la URL de la página desde la barra de direcciones de su navegador (ejemplo: `https://www.pinterest.com/pin/1234567890/`)
3. Pegue el enlace en el campo de entrada de esta herramienta y haga clic en el botón "Analizar"
4. El sistema extraerá los metadatos públicamente disponibles y mostrará la información de recursos accesibles
5. Seleccione el formato/resolución preferido, luego haga clic derecho en el enlace y elija "Guardar enlace como..." para descargar localmente

> 💡 Consejos de uso:
> - Verifique siempre que el contenido objetivo esté configurado con visibilidad "Pública"
> - Si el análisis falla, intente actualizar la página o verificar su conexión de red
> - Con fines de aprendizaje, considere usar las Herramientas para Desarrolladores del navegador (F12 �?Network �?Fetch/XHR) junto con esta herramienta

---

## ⚠️ Cumplimiento Normativo y Descargo de Responsabilidad (Lea Detenidamente)

Este proyecto opera bajo los principios de "neutralidad técnica" y "cumplimiento legal". Por favor, revise y acepte lo siguiente antes de usar:

### �?Prácticas Recomendadas
- Analice únicamente **contenido público** al que tenga acceso legítimo
- Utilice los recursos extraídos estrictamente para **aprendizaje personal, investigación o referencia privada**
- Obtenga permiso explícito por escrito de los titulares de derechos de autor antes de redistribuir, crear obras derivadas o usar con fines comerciales
- Siempre acredite a los creadores originales e indique claramente la atribución de fuentes en sus proyectos

### �?Actividades Prohibidas
- Intentar acceder o analizar contenido que requiera inicio de sesión, sea de pago o esté configurado como privado
- Usar esta herramienta para scraping comercial, servicios de agregación de datos o generación de ingresos publicitarios
- Enviar solicitudes automatizadas de alta frecuencia, tráfico de bots o cualquier actividad que pueda interrumpir los servicios de Pinterest
- Eliminar, alterar u ocultar marcas de agua, avisos de derechos de autor o metadatos incrustados

> 📜 Aviso Legal:
> El uso de esta herramienta debe cumplir con las leyes de derechos de autor aplicables (incluyendo pero no limitado a la DMCA, la Directiva de Derechos de Autor de la UE y regulaciones locales), así como con las [Directrices de la Comunidad](https://policy.pinterest.com/community-guidelines) y la [Política para Desarrolladores](https://developers.pinterest.com/docs/api/policy/) de Pinterest.
> Los desarrolladores no asumen responsabilidad alguna por problemas legales, daños o pérdidas que surjan del uso indebido de esta herramienta por parte de los usuarios finales.

---

## 🛠 Notas de Implementación Técnica (Para Desarrolladores)

> Los usuarios generales pueden omitir esta sección

### Visión General de la Arquitectura
```
Navegador del Usuario �?Módulo de Análisis en Cliente �?Endpoints Públicos de Pinterest / OEmbed �?Extracción de Datos Estructurados �?Renderizado de Resultados
```

### Enfoques Técnicos Clave
- Utiliza la API `fetch` con configuración apropiada de proxy CORS para recuperar metadatos de páginas públicas
- Analiza datos estructurados Schema.org desde etiquetas `<script type="application/ld+json">`
- Aprovecha metadatos Open Graph (`og:video`, `og:image`, `og:title`, etc.) para el descubrimiento de recursos
- Implementa validación dual mediante patrones regex + análisis DOM para un reconocimiento robusto de enlaces

### Guía de Auto-alojamiento (Referencia)
```bash
# 1. Clonar el repositorio (ejemplo)
git clone https://github.com/yourname/pinterest-downloader-sp.git

# 2. Desplegar archivos estáticos (se recomienda HTTPS)
#    - Vercel / Netlify / Cloudflare Pages (configuración sencilla, recomendado)
#    - Nginx + certificado Let's Encrypt (opción auto-alojada)

# 3. Ejemplo de configuración de encabezados de seguridad (Nginx)
add_header Content-Security-Policy "default-src 'self'; script-src 'self' 'unsafe-inline';";
add_header X-Content-Type-Options "nosniff";
add_header Referrer-Policy "strict-origin-when-cross-origin";
add_header X-Frame-Options "DENY";
```

> 🔐 Mejores Prácticas para Implementación en Producción:
> - Habilite siempre HTTPS para prevenir ataques de tipo man-in-the-middle
> - Implemente limitación de tasa (rate limiting) para prevenir abusos y solicitudes excesivas
> - Evite exponer lógica de análisis sensible que pueda ser mal utilizada
> - Revise y actualice regularmente las dependencias para aplicar parches de seguridad

---

## 🤝 Cómo Contribuir

¡Damos la bienvenida a contribuciones de la comunidad para ayudar a mejorar este proyecto educativo!

| Tipo de Contribución | Ejemplos |
|---------------------|----------|
| 🐛 Reporte de Errores | Envíe Issues con pasos detallados: URL + información del navegador + pasos de reproducción |
| 💡 Sugerencias de Funcionalidades | Comparta ideas constructivas para mejoras de UX, accesibilidad o nuevas características educativas |
| 🌍 Ayuda con Traducciones | Asista con la traducción de texto de la interfaz a idiomas adicionales |
| 📚 Documentación | Agregue ejemplos de uso, diagramas técnicos o guías de cumplimiento normativo |

> Este proyecto se publica bajo la [Licencia MIT](./LICENSE). Fomentamos el uso libre y la modificación con fines educativos y de investigación. Para consultas sobre personalización comercial, por favor contáctenos a través de canales separados.

---

## �?Preguntas Frecuentes (FAQ)

**P: ¿Por qué aparece el mensaje "No se pudo obtener el contenido"?**  
R: Posibles razones: �?El enlace apunta a contenido privado/eliminado �?Pinterest cambió temporalmente la estructura de la página �?Restricciones de red o problemas de CORS. Solución: Verifique el estado público �?Pruebe con otra red �?Espere e intente nuevamente.

**P: ¿El video descargado contiene marcas de agua?**  
R: Esta herramienta devuelve las URLs de recursos originales proporcionadas por la infraestructura oficial de Pinterest. La presencia de marcas de agua depende completamente de la configuración del usuario que subió el contenido. Esta herramienta no añade, elimina ni modifica ninguna marca de agua o marca incrustada.

**P: ¿Se admite el procesamiento por lotes para Álbumes o Tableros?**  
R: La versión actual se enfoca en el análisis de Pins individuales para priorizar la estabilidad y el cumplimiento normativo. Para operaciones por lotes, por favor asegúrese primero de que su caso de uso se alinee con la [Política para Desarrolladores](https://developers.pinterest.com/docs/api/policy/) de Pinterest en cuanto a límites de tasa y uso de datos.

**P: ¿Esta herramienta recopila mis datos de uso o información personal?**  
R: No. Este es un proyecto frontend estático puro sin registro en backend, scripts de análisis ni seguimiento basado en cookies. Todo el procesamiento ocurre localmente dentro de su sesión de navegador.

---

## 🌱 Nuestra Filosofía

> La tecnología en sí misma es neutral. Lo que importa es la *intención* y la *responsabilidad* de quienes la utilizan.

Animamos a desarrolladores y usuarios a adoptar estos valores:

- 🔬 Buscar una comprensión más profunda de las tecnologías web a través de la curiosidad y el aprendizaje ético
- 🤲 Respetar los derechos de los creadores atribuyendo adecuadamente las fuentes y solicitando permisos
- 🌍 Contribuir a un ecosistema digital saludable que equilibre la innovación con la preservación cultural

Juntos, fomentemos un ciclo positivo de creación, intercambio y uso responsable de la tecnología �?

---

## 📄 Licencia

Este proyecto se distribuye bajo la [Licencia MIT](./LICENSE).

```


Se concede permiso, de forma gratuita, a cualquier persona que obtenga una copia
de este software y los archivos de documentación asociados (el "Software"), para usar,
copiar, modificar, fusionar, publicar, distribuir, sublicenciar y/o vender
copias del Software, y permitir a las personas a quienes se les proporcione el
Software hacerlo, sujeto a las siguientes condiciones:

El aviso de derechos de autor anterior y este aviso de permiso se incluirán en todas
las copias o partes sustanciales del Software.

EL SOFTWARE SE PROPORCIONA "TAL CUAL", SIN GARANTÍA DE NINGÚN TIPO, EXPRESA O
IMPLÍCITA, INCLUYENDO PERO NO LIMITADO A LAS GARANTÍAS DE COMERCIABILIDAD,
IDONEIDAD PARA UN PROPÓSITO PARTICULAR Y NO INFRACCIÓN. EN NINGÚN CASO LOS
AUTORES O TITULARES DE LOS DERECHOS DE AUTOR SERÁN RESPONSABLES DE NINGUNA
RECLAMACIÓN, DAÑOS U OTRA RESPONSABILIDAD, YA SEA EN UNA ACCIÓN DE CONTRATO,
AGRAVIO O DE OTRO TIPO, QUE SURJA DE, FUERA DE O EN CONEXIÓN CON EL SOFTWARE
O EL USO U OTROS TRATOS EN EL SOFTWARE.
```

---


*🔖 Versión: v1.2.0-es (Optimización frontend / Soporte i18n mejorado / Documentación de cumplimiento reforzada)*