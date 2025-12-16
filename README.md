📧 Generador Automático de Borradores de Correo desde Google Sheets
Un script de Google Apps Script diseñado para automatizar la creación de borradores de correo electrónico en Gmail directamente desde Google Sheets al cambiar una celda de estado.

✨ Características Principales
Activación por Evento: El borrador de correo se crea automáticamente al seleccionar un valor específico ("Enviar") en una celda de estado.

Personalización de Destinatarios: Permite definir destinatarios principales (TO) y en copia (CC) fijos, además de tomar un correo de la propia fila.

Plantillas HTML: Carga y utiliza una plantilla de correo electrónico HTML almacenada en Google Drive, permitiendo diseños ricos y profesionales.

Datos Dinámicos: Reemplaza etiquetas dentro de la plantilla HTML (ej. {{name}}) con datos específicos de la fila de la hoja de cálculo.

Notificaciones: Muestra una alerta de éxito o error en la interfaz de Google Sheets.

⚙️ Configuración y Uso
Sigue estos pasos para implementar el script en tu Google Sheet:

1. Preparación de Google Sheets
Asegúrate de que tu hoja de cálculo esté configurada de la siguiente manera:

Nombre de la Hoja: El script opera en una hoja llamada Hoja 1.

Columna del Email (A): Debe contener la dirección de correo electrónico del destinatario principal de la fila.

Columna del Desplegable (B): Es la columna de activación. Al seleccionar el valor Enviar en esta columna, se dispara el script.

Columna de Datos (Ej. AD / Columna 30): La columna que contiene el dato que deseas usar en la plantilla (ej. el nombre, name).

2. Creación y Configuración del Archivo HTML
El cuerpo del correo se carga desde un archivo HTML alojado en Google Drive.

Crea un archivo de texto simple (puedes usar el Bloc de Notas o cualquier editor de código) con el contenido de tu correo electrónico en formato HTML.

Importante: Incluye las etiquetas dinámicas que deseas reemplazar, como {{name}}.

Sube este archivo .html a tu Google Drive.

Haz clic derecho sobre el archivo en Drive, selecciona Obtener enlace y copia el ID del archivo. El ID es la cadena de caracteres entre /d/ y /view en el enlace.

Ejemplo de URL: https://drive.google.com/file/d/TU_ID_AQUI/view?usp=sharing
