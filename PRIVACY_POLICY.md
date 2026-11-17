# Política de privacidad de CAM DOCS

**CAM DOCS — EVERY DOCUMENT. SMARTER.**
Desarrollado por ASTRIM · Sitio web oficial: https://astrim-web.web.app/

Versión 1.0 · En vigor desde el 16 de noviembre de 2026 · Aplicable a CAM DOCS 0.1.0 y posteriores.

Esta política describe cómo funciona realmente la aplicación CAM DOCS con la información que procesa. Se ha redactado a partir de una revisión del código fuente de la aplicación.

## 1. Responsable

ASTRIM, desarrolladora de CAM DOCS. Sitio web oficial: https://astrim-web.web.app/

Datos de identificación y contacto adicionales: [PENDIENTE DE COMPLETAR POR ASTRIM: denominación legal completa, domicilio y correo electrónico de contacto para privacidad].

## 2. Resumen

- CAM DOCS no requiere cuenta ni registro y no muestra publicidad.
- ASTRIM no recibe tus documentos, fotografías ni textos: CAM DOCS no tiene servidores propios a los que los envíe.
- Escanear, filtrar, reconocer texto (OCR), buscar, organizar y exportar se hace en tu dispositivo.
- Hay dos casos en los que la aplicación se comunica con servicios de terceros, explicados en los apartados 6 y 7: las métricas técnicas que envía Google ML Kit (Android) y la inteligencia artificial en la nube, que es opcional y solo funciona con tu autorización en cada envío.

## 3. Información que procesa la aplicación

- **Documentos e imágenes** que capturas con la cámara o importas: la imagen original de cada página, su versión procesada y una miniatura.
- **Texto reconocido (OCR)** de cada página, con la posición de cada palabra.
- **Datos de organización** que creas: títulos, carpetas, etiquetas, favoritos, anotaciones y orden de páginas.
- **Ajustes** de la aplicación: tema, idioma, calidad, opciones de seguridad y de OCR.
- **Datos de seguridad**: si configuras un PIN, se guarda únicamente un valor derivado (PBKDF2-HMAC-SHA256 con sal aleatoria), nunca el PIN. Si guardas una clave de API de inteligencia artificial, se guarda en el almacén seguro del sistema.

CAM DOCS no solicita tu nombre, correo electrónico, teléfono, ubicación ni contactos, y no utiliza identificadores publicitarios.

## 4. Documentos y fotografías del usuario

Los documentos, fotografías y archivos que escaneas, importas o generas con CAM DOCS te pertenecen. Se procesan para prestarte las funciones de la aplicación y no se utilizan para ningún otro fin.

## 5. Permisos que solicita la aplicación

- **Cámara**: para escanear documentos. Solo se usa mientras estás en la pantalla de escaneo. No se graba vídeo ni audio.
- **Biometría** (huella o rostro): solo si activas el desbloqueo biométrico. CAM DOCS no recibe tus datos biométricos; la verificación la hace el sistema operativo y solo comunica si fue correcta.
- **Internet** (Android): necesario para la inteligencia artificial en la nube opcional (apartado 7) y lo utilizan también los componentes de Google ML Kit (apartado 6).
- **Galería y archivos**: CAM DOCS no solicita acceso general a tus fotos ni a tu almacenamiento. Para importar imágenes se usa el selector del sistema, que solo entrega a la aplicación las imágenes que eliges. En iOS se declara el uso de la fototeca para ese selector y el micrófono porque lo exige el componente de cámara; CAM DOCS no graba audio.

Los permisos de leer y escribir el almacenamiento externo y de grabar audio que declaran algunos componentes se eliminan del paquete Android final.

## 6. Reconocimiento de texto (OCR)

- **Android**: se utiliza Google ML Kit Text Recognition con el modelo incluido en la aplicación. Según la documentación de Google, las imágenes y el texto reconocido se procesan en el dispositivo y **no se envían a Google**. Sin embargo, los componentes de ML Kit pueden contactar con servidores de Google para recibir correcciones o información de compatibilidad y **envían a Google métricas técnicas de uso y rendimiento**: información del dispositivo (fabricante, modelo, versión del sistema), información de la aplicación (nombre del paquete y versión), un identificador por instalación que según Google no pretende identificar al usuario ni al dispositivo, métricas de rendimiento, configuración de la API (por ejemplo, formato y resolución de la imagen), tamaño de entrada y salida, tipo de evento y códigos de error. Google indica que usa estos datos para diagnóstico y análisis de uso, que los cifra en tránsito y que no los transfiere a terceros. Este tratamiento lo realiza Google conforme a sus propias condiciones: https://developers.google.com/ml-kit/terms y https://policies.google.com/privacy
- **iOS**: se utiliza el framework Vision de Apple, que forma parte del sistema operativo y procesa el texto en el dispositivo.
- El OCR puede no reconocer el texto o hacerlo con errores. CAM DOCS no inventa el texto que no reconoce.
- **Traducción en el dispositivo (Android)**: la función Traducir usa Google ML Kit Translation y Language Identification. La primera vez que traduces a o desde un idioma, y solo después de que lo confirmes, la aplicación descarga desde servidores de Google el paquete de ese idioma (unos 30 MB). La descarga revela a Google la dirección IP de tu conexión y qué paquete se solicita, pero **no incluye el texto de tus documentos**: la detección del idioma y la traducción se hacen en el teléfono. Estos componentes envían las mismas métricas técnicas descritas arriba. Puedes eliminar los paquetes descargados en Ajustes › Inteligencia › Paquetes de idioma.

## 7. Inteligencia artificial (ASTRIM Intelligence)

- **Análisis local**: resúmenes, datos clave, lectura de facturas y contratos, clasificación, preguntas, comparaciones y búsquedas se calculan en el dispositivo con el texto OCR, sin conexión.
- **IA en la nube (opcional)**: solo está disponible si tú introduces tu propia clave de API de Anthropic (Claude). Está desactivada por defecto.
- **Autorización en cada envío**: antes de cada consulta en la nube la aplicación te muestra qué documentos y cuántos fragmentos de texto se enviarán, y no envía nada si no lo autorizas.
- **Qué se envía**: fragmentos del texto reconocido de los documentos seleccionados (para las preguntas, solo los más relevantes), el título del documento y el número de página de cada fragmento, tu pregunta y, en su caso, el idioma de destino de una traducción. **No se envían imágenes.** La solicitud se envía por HTTPS directamente desde tu dispositivo a la API de Anthropic (https://api.anthropic.com), identificada con tu clave; como en cualquier conexión a internet, el servidor recibe además la dirección IP de tu conexión.
- **Quién lo trata**: Anthropic trata esa información conforme a sus condiciones y su política de privacidad (https://www.anthropic.com/legal/privacy), vinculadas a la cuenta asociada a tu clave. ASTRIM no recibe ni almacena esas solicitudes ni sus respuestas.
- Los documentos **protegidos** no se incluyen en el análisis mientras están bloqueados.

## 8. Servicios externos

Aparte de lo descrito en los apartados 6 y 7, CAM DOCS no integra servicios de analítica, publicidad, redes sociales, informes de errores ni sistemas de seguimiento, y no transmite información a ASTRIM.

Cuando abres el sitio web oficial desde la sección "Acerca de", se abre en tu navegador, que se rige por sus propias condiciones.

## 9. Almacenamiento local

- Los documentos, el texto reconocido y la base de datos se guardan en el **almacenamiento privado** de la aplicación, al que otras aplicaciones no pueden acceder.
- Las **copias de seguridad automáticas en la nube del sistema están desactivadas** para la aplicación (Android), de modo que los documentos no se copian a otros servicios por esa vía.
- Los ajustes se guardan en las preferencias de la aplicación; el valor derivado del PIN, la clave de API opcional y la clave de cifrado de documentos protegidos se guardan en el almacén seguro del sistema (Android Keystore / iOS Keychain).

## 10. Cifrado y seguridad

- **Cifrado del sistema**: los archivos privados de la aplicación están protegidos por el cifrado de almacenamiento del sistema operativo (cifrado por archivo en Android; en iOS la aplicación solicita la protección de datos completa, que impide el acceso con el dispositivo bloqueado).
- **Documentos protegidos (opcional)**: puedes marcar un documento como protegido. Sus imágenes, su texto OCR y sus anotaciones se cifran además con AES-256-GCM usando una clave aleatoria guardada en el almacén seguro del sistema; abrirlo exige tu PIN o biometría. Mientras lo tienes abierto se descifra a una caché temporal privada que se borra al salir del documento o de la aplicación. El título y las etiquetas de un documento protegido no se cifran.
- **Bloqueo de la aplicación**: PIN opcional con bloqueo temporal tras intentos fallidos, desbloqueo biométrico opcional y pantalla protegida (en Android impide capturas de pantalla).
- Ningún sistema es infalible: estas medidas reducen riesgos, pero no pueden garantizar una seguridad absoluta frente a un dispositivo comprometido o desbloqueado por terceros.

## 11. Compartir y exportar archivos

CAM DOCS solo comparte un documento cuando tú lo exportas y eliges el destino con la hoja de compartir o el diálogo de guardado del sistema. Desde ese momento, el archivo exportado queda sujeto a la aplicación o servicio que elijas. Los PDF pueden protegerse con contraseña al exportarlos. Los archivos temporales de exportación se borran al iniciar la aplicación.

## 12. Conservación de datos

- Los documentos se conservan en tu dispositivo hasta que los eliminas.
- Los documentos enviados a la **papelera** se eliminan definitivamente a los 30 días, o antes si vacías la papelera.
- Las sesiones de escaneo interrumpidas se eliminan a las 24 horas; las exportaciones temporales, al iniciar la aplicación.

## 13. Eliminación de información

- Puedes eliminar documentos (pasan a la papelera), restaurarlos o borrarlos definitivamente desde la papelera.
- Puedes borrar la clave de API y el PIN desde Ajustes.
- Desinstalar la aplicación elimina su almacenamiento privado, incluidos todos los documentos, del dispositivo.
- La eliminación usa los mecanismos normales del sistema de archivos. CAM DOCS no realiza un borrado forense (sobrescritura) de los datos; en los documentos protegidos, lo que queda en el almacenamiento está cifrado.
- Las métricas técnicas enviadas por Google ML Kit y las solicitudes enviadas a Anthropic no están bajo el control de ASTRIM; para ellas aplica la política del proveedor correspondiente.

## 14. Derechos de los usuarios

Como CAM DOCS no envía tus documentos a ASTRIM, la información que la aplicación procesa está en tu dispositivo y bajo tu control: puedes consultarla, exportarla, modificarla y eliminarla en cualquier momento desde la propia aplicación.

Según la legislación aplicable, puedes tener derechos de acceso, rectificación, supresión, oposición, limitación del tratamiento y portabilidad, y a presentar una reclamación ante la autoridad de protección de datos competente. Para ejercer tus derechos ante ASTRIM puedes dirigirte a través de su sitio web oficial (https://astrim-web.web.app/) [PENDIENTE DE COMPLETAR POR ASTRIM: correo electrónico o canal de contacto específico para privacidad]. Para los datos tratados por Google o Anthropic, dirígete a esos proveedores.

## 15. Menores

CAM DOCS es una herramienta de propósito general para la gestión de documentos y no está dirigida específicamente a menores. [PENDIENTE DE COMPLETAR POR ASTRIM: edad mínima de uso conforme a la legislación aplicable y a las políticas de las tiendas de aplicaciones].

## 16. Actualizaciones de esta política

Si cambia el funcionamiento de la aplicación en lo que afecta a la información que procesa, esta política se actualizará y se indicará su nueva versión y fecha. La versión vigente está disponible dentro de la aplicación (Ajustes › Acerca de CAM DOCS) y en el sitio web oficial.

## 17. Contacto

ASTRIM · Sitio web oficial: https://astrim-web.web.app/

© 2026 ASTRIM. TODOS LOS DERECHOS RESERVADOS.
