🐶 Clasificador de Imágenes: Perros y Gatos

Este proyecto fue desarrollado como práctica personal para crear un clasificador de imágenes capaz de reconocer perros y gatos usando Python, TensorFlow y TensorFlow.js.

La idea es que el modelo, una vez entrenado, pueda ejecutarse directamente en el navegador — incluso desde un celular — sin necesidad de instalar nada adicional. Solo apuntas la cámara a un perro o gato (real o en foto) y el modelo hace la predicción al instante.

🚀 ¿Qué hace este proyecto?

El sitio web carga un modelo previamente entrenado en Python con TensorFlow.
Ese modelo se exporta a los archivos model.json y .bin, los cuales son utilizados por TensorFlow.js para funcionar directamente en el navegador.

Puede reconocer si la imagen corresponde a un perro o un gato, mostrando el resultado en tiempo real.

⚙️ Cómo usarlo
1. Descargar el repositorio

Descarga o clona este repositorio en tu computadora:

git clone https://github.com/TU_USUARIO/clasificador-perros-gatos.git

2. Iniciar el servidor local

TensorFlow.js necesita ejecutarse desde un servidor local, así que puedes usar el que viene con Python:

python -m http.server 8000


Luego abre tu navegador y entra a:
👉 http://localhost:8000

📱 Uso desde el celular

Para probarlo en el celular, necesitas acceder mediante un enlace HTTPS, ya que la cámara solo funciona bajo conexiones seguras.
Puedes usar Ngrok para eso:

Descarga y descomprime Ngrok.

Abre una terminal en la carpeta donde lo tengas.

Ejecuta:

ngrok http 8000


Mantén activo tanto el servidor Python como el túnel de Ngrok.

Copia el enlace HTTPS que aparece en la terminal y ábrelo desde el navegador de tu celular.

🔁 El túnel de Ngrok expira cada 2 horas, pero puedes reiniciarlo fácilmente.

🎥 Uso general

Una vez abierto el sitio:

Da clic en “Cambiar cámara” para usar la frontal o trasera.

Apunta la cámara hacia un perro o gato (puede ser una imagen o uno real).

En la parte inferior aparecerá la predicción.

Nota: El modelo no es perfecto, fue entrenado con fines educativos, así que puede fallar en algunas imágenes.

🧩 Problemas o errores

Si algo no funciona:

Revisa la consola del navegador (F12 → pestaña “Console”) para ver si hay errores.

Asegúrate de tener tanto Python como Ngrok ejecutándose.

También puedes dejar un comentario o reporte de error en este repositorio.




🧠 Autor

Proyecto realizado por [Tu nombre o usuario de GitHub] como práctica de inteligencia artificial con TensorFlow.
