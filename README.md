GPSMapApp

Descripción:
SimpleGPSMapApp es una aplicación Android que permite al usuario visualizar su ubicación actual en un mapa, añadir marcadores en distintas ubicaciones y capturar imágenes. Utiliza la API de Google Maps y los servicios de localización de Android para gestionar la ubicación del usuario y proporcionar una interfaz interactiva y dinámica.

Características:

Muestra la ubicación actual del usuario en un mapa.
Permite añadir marcadores en cualquier ubicación dentro del mapa.
Incluye una opción para capturar y mostrar imágenes relacionadas con una ubicación.
Implementa subprocesos (threads) para mejorar el rendimiento de la aplicación.

Requisitos del proyecto:

Android Studio
Conexión a Internet para acceder a la API de Google Maps.
Dispositivo o emulador con servicios de Google Play.
Permisos de ubicación habilitados en el dispositivo.

Configuración del Proyecto:

Obtener la API Key de Google Maps:

Para poder utilizar Google Maps en la aplicación, necesitas obtener una clave API de Google. Puedes seguir las instrucciones en la página oficial de Google Maps API.

Añadir la API Key:

Una vez obtengas tu clave API, debes agregarla al archivo res/values/google_maps_api.xml.

Configurar permisos:

Asegúrate de que los siguientes permisos estén configurados en el archivo AndroidManifest.xml:

Copiar código
<uses-permission android:name="android.permission.ACCESS_FINE_LOCATION" />
<uses-permission android:name="android.permission.ACCESS_COARSE_LOCATION" />

Ejecutar el Proyecto:

Abre el proyecto en Android Studio, sincroniza las dependencias del archivo build.gradle, conecta tu dispositivo o emulador, y ejecuta la aplicación.

Uso de la Aplicación:

Al abrir la aplicación, se mostrará la ubicación actual del usuario en un mapa.
Puedes añadir marcadores en cualquier lugar del mapa tocando sobre la ubicación deseada.
La app también incluye la opción de capturar imágenes relacionadas con las ubicaciones seleccionadas.

Estructura del Proyecto:

MainActivity.java: Contiene la lógica principal de la aplicación, gestionando la interacción con el mapa y la obtención de la ubicación del usuario.

activity_main.xml: Archivo que define el diseño de la interfaz gráfica de la aplicación, incluyendo el MapView.

AndroidManifest.xml: Archivo que define los permisos y otras configuraciones necesarias para el funcionamiento correcto de la aplicación.

Tecnologías utilizadas:

Java: Lenguaje de programación utilizado en la app.

Google Maps API: Para la visualización y manipulación de mapas dentro de la app.

Android Location Services: Para obtener y gestionar la ubicación del usuario.

