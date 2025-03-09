Para descargar un repositorio de GitHub y abrirlo en Visual Studio Code:
1. Copiar la URL del repositorio
2. Clonar el repositorio en VS Code:
   Abre Visual Studio Code.
  Presiona Ctrl + Shift + P (o Cmd + Shift + P en macOS) para abrir la Paleta de Comandos.
  Escribe "Git: Clone" y selecciona la opción Git: Clone.
  Pega la URL copiada y presiona Enter.
  Elige una carpeta donde se descargará el repositorio.
3. Abrir el repositorio en VS Code
  Cuando termine la clonación, VS Code preguntará si quieres abrir el repositorio. Haz clic en "Abrir".
4. Verificar conexión con GitHub
    Abre una terminal en VS Code: git remote -v
    Si ves la URL de GitHub, la clonación fue exitosa.
5. (Opcional) Configurar credenciales de GitHub
    Si es la primera vez que usas Git en tu PC, configura tu usuario y correo con:
       git config --global user.name "TuNombre"
       git config --global user.email "TuEmail"

Para cargar los cambios de tu repositorio en Visual Studio Code a tu página de GitHub, sigue estos pasos:
1. Asegúrate de que tu repositorio está vinculado a GitHub
    Si clonaste tu repositorio desde GitHub, ya está vinculado. Si no, verifica con: git remote -v
    Si no ves la URL de tu repositorio, agrégala con: git remote add origin https://github.com/TU_USUARIO/TU_REPOSITORIO.git
2. Guarda los cambios en Git
   git add .
3. Añade todos los archivos modificados: git commit -m "Descripción de los cambios"
4. Sube los cambios a GitHub: git push origin master
Si Git te pide autenticación, inicia sesión en GitHub con tu cuenta

Si tu página no se actualiza en GitHub Pages
Revisa la rama de publicación en Settings > Pages.
Si usas una rama diferente (gh-pages): git push origin gh-pages

