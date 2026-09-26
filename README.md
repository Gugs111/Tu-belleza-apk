# Tu Belleza — proyecto APK para tablet Android 8.1

Proyecto Android nativo que empaqueta la versión web de Tu Belleza dentro de un WebView local.
Está preparado para la tablet Occicel con Android 8.1 (API 27).

## Características
- Pantalla completa e interfaz horizontal.
- WebView con JavaScript y almacenamiento local habilitados.
- El HTML está incluido dentro del APK: no depende de GitHub Pages para abrir la app.
- Servicios, inventario, ventas, clientes, citas, galería y configuración.
- Los datos se guardan localmente en la tablet.
- Las imágenes remotas de servicios/galería requieren Internet.

## Compilar con Android Studio
1. Abre esta carpeta en Android Studio.
2. Espera a que termine la sincronización de Gradle.
3. Ve a Build > Generate App Bundles or APKs > Generate APKs.
4. El APK release queda en:
   app/build/outputs/apk/release/app-release.apk

## Compilar desde GitHub Actions
El proyecto incluye `.github/workflows/build-apk.yml`.
Sube el proyecto a un repositorio GitHub y ejecuta:
Actions > Compilar Tu Belleza APK > Run workflow.
Al terminar, descarga el artefacto `Tu-Belleza-APK`.

## Requisitos
- Android Studio reciente / JDK 17 para compilación local.
- Para instalar el APK: Android 8.1 o superior.
