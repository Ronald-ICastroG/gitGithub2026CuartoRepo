En Git, siempre es recomendable trabajar en ramas diferentes al main para evitar conflictos y mantener el código base seguro. Crea una nueva rama para cada característica o tarea que estés desarrollando.

    Crear una nueva rama:
        Siempre asegúrate de estar fuera de la rama principal cuando desarrolles nuevas características.
        Usa un nombre descriptivo para la rama que refleje la tarea que estás realizando.

git checkout -b mi-nueva-rama

    Realizar commits: Asegúrate de que cada commit describa claramente los cambios realizados.

git add .
git commit -m "Implementación de nueva API"

¿Cómo desarrollar y probar una API en Python?

Hemos hablado sobre la configuración del entorno de desarrollo; ahora, toca desarrollar una simple API en Python.

    Configurar la estructura del proyecto:
        Crea una carpeta dedicada para tu API, por ejemplo, api.
        Añade un archivo app.py y requirements.txt en la raíz de tu carpeta de API.

    Instalar las dependencias necesarias:
        Asegúrate de que requirements.txt contenga todos los paquetes necesarios.

pip3 install -r requirements.txt

    Desplegar la API:
        Usa herramientas como uvicorn para lanzar tu servidor y verificar que todo funcione correctamente.

uvicorn app:app --reload

¿Cómo efectuar un pull request en GitHub?

Al finalizar tus cambios y haberlos probado adecuadamente, es hora de subirlos a GitHub y abrir un pull request. Esto no solo integra tus cambios al repositorio principal, sino que también permite revisiones de tus compañeros de equipo.

    Subir cambios a GitHub:
        Asegúrate de estar en la rama correcta y empuja tus cambios.

git push -u origin mi-nueva-rama

    Crear un pull request:
        Utiliza el archivo pull-request-template.md para seguir una guía estructurada en el momento de realizar el pull request.

Compartir una base común, usando las plantillas y el flujo de trabajo explicados, asegura que todos los miembros del equipo estén alineados y que el proyecto avance sin contratiempos.
Consejos adicionales

    Nunca trabajes directamente en main: Esto protege la integridad del proyecto principal y permite un flujo de desarrollo más organizado.
    Utiliza plantillas: Tanto para issues como para pull requests, asegurando que toda la comunicación sea clara y relevante.
    Revisión de código colaborativo: Anima a tus compañeros a revisar el código antes de fusionarlo en el main, esto ayuda a detectar errores más temprano y aprender de los diferentes enfoques en el equipo.

Este proceso asegura no solo una correcta integración de herramientas, sino que también fomenta un ambiente de trabajo colaborativo y organizado, esencial en todo proyecto de software.
