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
4.  **Extrae todo el contenido** de este archivo comprimido directamente dentro de `C:\php`. Una vez extraído, puedes eliminar el archivo comprimido original.

<<<<<<< HEAD
### Paso 4: Añadir PHP al PATH del Sistema
=======
### Paso 4: Renombrar el archivo php.ini-development
1.  Entre los archivos que se te generaron en la extracción deberás localizar un archivo de nombre **php.ini-development**
2.  Una vez localizado lo vamos a renombrar a **php.ini**.
3.  Listo, continuar al siguiente paso.

### Paso 5: Añadir PHP al PATH del Sistema
>>>>>>> a9333083acf4aa6b2c0275f191accf8b08ce85ca

Este es un paso fundamental que permitirá a Windows reconocer el comando `php` desde cualquier ubicación en la línea de comandos.

1.  **Copiar la Ruta de la Carpeta PHP:**
    * Vamos a copiar la ruta en la que nos localizamos que debería ser `C:\php`.
    * En la **barra de direcciones** superior del Explorador de Archivos (donde se muestra la ruta actual, por ejemplo, `Este equipo > Disco local (C:) > php`), haz clic para que la ruta completa se seleccione, todo el texto se pondrá azul señal que está seleccionado.
    * Cópiala (puedes usar `Ctrl + C`).

2.  **Abrir las Variables de Entorno del Sistema:**
    * Presiona la tecla `Windows` en tu teclado.
    * Escribe "variables de entorno" y selecciona la opción **"Editar las variables de entorno del sistema"** que aparecerá.

3.  **Editar la Variable `Path`:**
    * En la ventana "Propiedades del sistema", haz clic en el botón **"Variables de entorno..."**.
    * En la sección "Variables del sistema" (la caja inferior), busca y da clic en la variable con el nombre **`Path`**.
    * Ahora localiza el botón **"Editar..."** que se encuentra a su lado derecho y da clic.

4.  **Añadir la Ruta de PHP:**
    * En la nueva ventana que se abre, haz clic en el botón **"Nuevo"**.
    * En el campo de texto que aparece, **pega la ruta** que copiaste anteriormente (`C:\php`).
    * Haz clic en **"Aceptar"** para cerrar esta ventana.

5.  **Guardar y Cerrar Todas las Ventanas:**
    * Haz clic en **"Aceptar"** en la ventana de "Variables de entorno".
    * Finalmente, haz clic en **"Aceptar"** en la ventana de "Propiedades del sistema".

### Paso 6: Verificar la Instalación

1.  **Abrir una Nueva Terminal:**
    * **¡Importante!** Cierra todas las ventanas de Símbolo del sistema (CMD) o PowerShell que tengas abiertas actualmente. Los cambios en las variables de entorno solo se aplican a las nuevas sesiones.
    * Presiona la tecla `Windows` y escribe `cmd`. Presiona `Enter` para abrir una nueva ventana del Símbolo del sistema.

2.  **Ejecutar el Comando de Verificación:**
    * Dentro de la nueva ventana de CMD, escribe el siguiente comando y presiona `Enter`:

    ```bash
    php -v
    ```

3.  **Interpretar el Resultado:**
    * **Si ves la versión de PHP** (por ejemplo, "PHP 8.3.21 (cli) (built: May 7 2024 00:00:00)..."), ¡felicitaciones! PHP ha sido instalado y configurado correctamente en tu PC.
    * **Si recibes el mensaje:** `"php" no se reconoce como un comando interno o externo, programa o archivo por lotes ejecutable.`, significa que ha ocurrido un error en el proceso. Por favor, revisa cuidadosamente todos los pasos, prestando especial atención al "Paso 4: Añadir PHP al PATH del Sistema" y asegurándote de que `php.exe` esté directamente en `C:\php`.

---

Una vez que PHP esté correctamente instalado, ya podrás ejecutar los scripts y proyectos PHP contenidos en este repositorio. ¡Disfruta!
