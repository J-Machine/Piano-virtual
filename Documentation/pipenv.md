Install:  pip3 install pipenv
- --
En el project
* Especificando la version a usar: pipenv --python 2.7.18
* Instalación de pkg: pipenv install [package names]
** El usuario puede proporcionar estos parámetros adicionales:

--two - Realiza la instalación en un virtualenv usando el enlace del sistema python2.
--three - Realiza la instalación en un virtualenv usando el enlace del sistema python3.
--python: realiza la instalación en un virtualenv utilizando el intérprete de Python proporcionado.

* Especificar version de pkg: Se prefiere el uso de ~ = sobre el identificador == ya que este último evita que pipenv actualice los paquetes
    $ pipenv install "requests~=2.2"  # locks the major version of the package (this is equivalent to using ==2.*)
* Desinstalar pkg: pipenv uninstall [package]
- --
* PIP.LOCK
$ pipenv lock se usa para crear un Pipfile.lock, que declara todas las dependencias (y subdependencias) de su proyecto, sus últimas versiones disponibles y los hashes actuales para los archivos descargados. Esto asegura compilaciones repetibles y, lo que es más importante, deterministas.
  
- --
* Activar el env: pipenv shell
* Desactivar: exit


- --

Source: https://pipenv-es.readthedocs.io/es/latest/
https://www.adictosaltrabajo.com/2018/11/06/gestion-de-versiones-de-python-con-pipenv/