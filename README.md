# Linux-lab-setup
Documentación de mi laboratorio Linux - Fase 1 del aprendizaje DevSecOps

## ¿Qué es este proyecto?
Documentación de la instalación y configuración de mi laboratorio personal con Linux.
Parte de mi aprendizaje hacia DevSecOps.

## Sistema
- Laptop: Intel Core i3, 8GB RAM
- OS instalado: Ubuntu 22.04 LTS
- Fecha de instalación: [15/03/2026]

## Lo que aprendí
- Cómo crear una USB booteable con Rufus
- Cómo instalar Ubuntu desde cero
- Comandos básicos de terminal: pwd, ls, cd, mkdir, whoami, uname

## Comandos básicos que practico
| Comando | Qué hace |
|---------|----------|
| pwd | Muestra la carpeta actual |
| ls | Lista archivos |
| cd | Navega entre carpetas |
| mkdir | Crea una carpeta |
| whoami | Muestra el usuario |
| uname -a | Info del sistema |

## Próximos pasos
- [ ] Aprender permisos (chmod, chown)
- [ ] Configurar servidor SSH
- [ ] Instalar y usar Nmap
- [ ] Practicar Bash scripting

## Problemas resueltos

### Minecraft en Ubuntu 24.04
El launcher oficial (.deb) no abría por incompatibilidad de librerías.

**Solución — Flatpak:**
sudo apt install flatpak -y
flatpak --user remote-add --if-not-exists flathub https://dl.flathub.org/repo/flathub.flatpakrepo
flatpak install minecraft
flatpak run com.mojang.Minecraft
Seleccionar opción 3 (com.mojang.Minecraft) cuando lo pida.


## Día 1 — 16 marzo 2026
**Tema:** Navegación en Linux

**Lo que practiqué:**
| Comando | Qué hace |
|---------|----------|
| pwd | Muestra en qué carpeta estás |
| ls | Lista archivos y carpetas |
| cd | Navega entre carpetas |
| cd .. | Sube un nivel |
| cd ~/ | Regresa a tu carpeta personal |
| mkdir | Crea una carpeta |
| touch | Crea un archivo vacío |
| rm -r | Borra una carpeta con contenido |

**Problema que resolví:**
Al dar dos veces `cd ..` llegué a la raíz del sistema y vi bin, home, mnt, usr.
Solución: usar `cd home` luego `cd (user)` para regresar a mi carpeta personal.
Atajo aprendido: `cd ~/` regresa siempre a casa sin importar dónde estés.

**Lo que entendí:**
Linux es un árbol de carpetas. La raíz es `/` y todo vive dentro de ella.
Mi carpeta personal siempre es `/home/user` y el símbolo `~` la representa.
