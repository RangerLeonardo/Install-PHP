# Guía de Instalación de PHP en Windows

Este documento te guiará paso a paso para descargar, instalar y configurar PHP en tu sistema operativo Windows, lo que te permitirá ejecutar los proyectos de este repositorio.

---

## 🚀 Pasos para la Instalación

Sigue cuidadosamente estas instrucciones para configurar PHP en tu equipo:

### Paso 1: Obtener el Repositorio

1.  **Clonar el Repositorio:**
    Si estás familiarizado con Git, puedes clonar este repositorio usando el siguiente comando en tu terminal:

    ```bash
    git clone https://github.com/RangerLeonardo/BlogCafe.git
    ```

2.  **Descargar el Repositorio (Alternativa):**
    Si prefieres no usar Git, puedes descargar el repositorio completo como un archivo ZIP desde la plataforma donde se aloja (ej. GitHub). Una vez descargado, **descomprímelo**. Esto creará una carpeta con el nombre `Install-PHP`.

### Paso 2: Preparar el Archivo PHP

1.  Navega a la carpeta que se generó en el paso anterior, `Install-PHP`.
2.  Dentro de esta carpeta, encontrarás el archivo comprimido de PHP (probablemente llamado `php.zip` o `php.rar`).
3.  **Copia** este archivo comprimido.

### Paso 3: Descomprimir PHP en la Ubicación Correcta

1.  Dirígete a la raíz de tu **Disco Local (C:)**.
2.  Crea una **nueva carpeta** con el nombre `php` (es decir, la ruta completa será `C:\php`).
3.  **Pega** el archivo comprimido de PHP (que copiaste en el Paso 2) dentro de la carpeta `C:\php`.
4.  **Extrae todo el contenido** de este archivo comprimido directamente dentro de `C:\php`. Es crucial que los archivos principales de PHP, como `php.exe` y `php-cgi.exe`, estén directamente dentro de `C:\php`, y no dentro de una subcarpeta adicional (ej. `C:\php\php-8.x.x`). Una vez extraído, puedes eliminar el archivo comprimido original.

### Paso 4: Añadir PHP al PATH del Sistema

Este es un paso fundamental que permitirá a Windows reconocer el comando `php` desde cualquier ubicación en la línea de comandos.

1.  **Copiar la Ruta de la Carpeta PHP:**
    * Abre el Explorador de Archivos y navega a la carpeta `C:\php`.
    * En la **barra de direcciones** superior del Explorador de Archivos (donde se muestra la ruta actual, por ejemplo, `Este equipo > Disco local (C:) > php`), haz clic para que la ruta completa se seleccione.
    * Cópiala (puedes usar `Ctrl + C`).

2.  **Abrir las Variables de Entorno del Sistema:**
    * Presiona la tecla `Windows` en tu teclado.
    * Escribe "variables de entorno" y selecciona la opción **"Editar las variables de entorno del sistema"** que aparecerá.

3.  **Editar la Variable `Path`:**
    * En la ventana "Propiedades del sistema", haz clic en el botón **"Variables de entorno..."**.
    * En la sección "Variables del sistema" (la caja inferior), busca y selecciona la variable con el nombre **`Path`**.
    * Haz clic en el botón **"Editar..."**.

4.  **Añadir la Ruta de PHP:**
    * En la nueva ventana que se abre, haz clic en el botón **"Nuevo"**.
    * En el campo de texto que aparece, **pega la ruta** que copiaste anteriormente (`C:\php`).
    * Haz clic en **