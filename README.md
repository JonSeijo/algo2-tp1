# algo2-tp1
TP 1 - Algoritmos y Estructuras de Datos 2

## Inicio

Para empezar hacer "git clone" del repositorio. Esto les descarga una copia de todo listo para empezar a usar, ya deberian estar agregados como colaboradores.


## Hacer andar paquete de latex

*Asumiendo que estan en LINUX*

- Descarguen el paquete de latex de algo2

[http://www.dc.uba.ar/materias/aed2/2016/1c/descargas/otros](http://www.dc.uba.ar/materias/aed2/2016/1c/descargas/otros)

- Bajar lo que dice "LaTex en Algo2. Paquete oficial de LaTex de Algo2"
- Esto les descarga un .zip
- Dentro de este .zip, tiene que haber una carpeta "texmf"
- La descomprimen en su home ( /home/MiUsuario  )
- Parados ahi en la consola escriben

```
sudo texhash texmf
```

- Ya deberian poder usar las macros y cosas copadas de latex lo mas bien. Prueben compilar el apunte de tads basicos que esta subido a este repo. Este es un archivo de latex que usa todas estas macros locas, asi que si lo compilan bien es porque pudieron instalar todo.


## Sobre gitignore

Por defecto puse que se ignoren todos los archivos .pdf del directorio. Esto quiere decir que directamente no se suben pdfs al repo automaticamente. Esto es para evitar conflictos con el tp compilado, no tiene sentido porque con el .tex nos basta.

Puede haber casos que si querramos subir un pdf, por ejemplo una update del enunciado, o algun apunte o lo que sea. Para esto hay que abrir el archivo .gitignore de este mismo repositorio (Abrirlo con cualquier editor de texto) y agregar una excepcion de archivo

Una excepcion se hace agregando ! al inicio de un path. Por ejemplo, si quiero agregar como excepcion a *pepito.pdf*, dentro del .gitignore tengo que agregar una linea que diga

```
!pepito.pdf
```