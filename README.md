# Tutorial-de-instalaci-n-de-Docker-2026-link-mega-sin-acortadores
Este es un tutorial simple para instalar Docker.

# Sección 1: Powershell

  1. Buscar Powershell en la barra de búsqueda de Windows y ejecutar cómo administrador.
     <img width="906" height="401" alt="image" src="https://github.com/user-attachments/assets/3d32a371-226c-44a9-9a59-240c0b8be02b" />
     
  2. Con Poweshell abierto, debe ejecutar una serie de comandos a continuación

# Sección 2: Comandos

  1. wsl --install: Habilita WSL 2 en windows
    <img width="335" height="33" alt="image" src="https://github.com/user-attachments/assets/87122362-5724-45fd-9814-213b8fbf63ae" />
    Posteriormente, escriba usuario, contraseña y conformación de contraseña

  2. Invoke-WebRequest -Uri https://desktop.docker.com/win/stable/Docker%20Desktop%20Installer.exe -OutFile DockerDesktopInstaller.exe
     Descarga el installer de Docker en el escritorio

  3. Start-Process -Wait -FilePath .\DockerDesktopInstaller.exe: instala Docker en el escritorio

     <img width="808" height="23" alt="image" src="https://github.com/user-attachments/assets/236dafeb-1848-4c39-9739-f5a637fd7119" />

     
  4. Remove-Item .\DockerDesktopInstaller.exe: Elimina el installer 
     
# Sección 3: Docker

  Después de la instalación, inicia Docker en el escritorio y debemos configurarlo para utilizar      WSL 2 correctamente.
  Puede hacerse de la siguiente manera.

  1. Abrir Docker
  2. Ir a: Ajustes > General
  3. Marca la opción de "Usar el motor WSL 2"

  <img width="1571" height="767" alt="image" src="https://github.com/user-attachments/assets/a4df927c-dbd6-429d-84c7-bdcc1847bf72" />

Después tenemos que verificar la instalación de Docker en Git Bash con docker --version

<img width="340" height="56" alt="image" src="https://github.com/user-attachments/assets/ef2d2140-ec73-4d8b-ae5d-2fca3b93c4d0" />

Este comando debería poner en pantalla la versión de docker que fué instalado

# Docker fué instalado satisfactoriamente




















  


     


