# Arch Install Scripts

#
# /etc/abs.conf
#

# el directorio de nivel superior de todos sus PKGBUILD
[ "$ABSROOT" = "" ] && ABSROOT="/var/abs/"

#
# Servidor desde el que sincronizar
#
SYNCSERVER="rsync.archlinux.org"

#
# La arquitectura para obtener abs para
# Ya sea i686 o x86_64
#
ARCH="i686"

#
# Lista de espejos de Pacman utilizada para la sincronización mediante archivo tar
#
LISTA DE ESPEJOS="/etc/pacman.d/listadeespejos"

#
# REPOS que serán analizados por abs (en este orden)
# (anteponga un ! al repositorio para deshabilitarlo)
#
# Nota: Si se elimina un repositorio, ¡aún se recupera!
# Los repositorios deben ir precedidos de un ! para evitar su recuperación
#
REPOS=(núcleo extra comunidad multilib !prueba !prueba-comunidad !prueba-multilib
       !puesta en escena !puesta en escena comunitaria !gnome-inestable !kde-inestable)