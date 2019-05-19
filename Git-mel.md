## Git

### 1: Comandos básicos - terminal normal

Crear un archivo
``` console
	touch <archivo_con_extensión>
```

Borrar un fichero y sus sub-ficheros (cuidado con este comando)
``` console
	rm -rf <archivo_o_carpeta>
```

Imprimir algo y mandar su contenido a un fichero
``` console
	echo "texto_ejemplo" >> <archivo_destino>
```

Listar todos los archivos (incluyendo ocultos)
``` console
	ls -la <ruta_a_lo_que_quieras_listar (parámetro opcional)>
```

Saber en dónde te encuentras actualmente
``` console
	pwd
```

### 2 : Iteración básica de Git

Inicializa repositorio (decirle a Git que escuche por cambios en una carpeta)
``` console
	git init
```

Selecciona archivos que vas a añadir
``` console
	git add -A  // Para añadir todos los archivos
	git add <file1> <file2> <file_n> //  Para añadir archivos o carpetas específicos
```

Para saber el status del repo y sus archivos
``` console
	git status
```

hacer el commit
``` console
	git commit -m "mensaje_del_commit"
```

### 3 : Rastreo de los cambios, retirando cambios de los archivos 

Muestra todos los commits realizados hasta el momento, con toda su información
``` console
	git log
```

Muestra todos los commits realizados hasta el momento, en formato corto y mostrando las ramas
``` console
	git log --all --oneline --graph
```

Descarta los cambios de un archivo que hayas añadido para el próximo commit (con git add)
``` console
	git checkout -- <archivo(s)>
```

*Nota: Para NO subir cambios a un archivo, basta con no añadirlo ni commitearlo*

### Opcional : Llave SSH para conectar con el repo remoto y trabajar más rápido

Comunicar con cuenta de github, generar ssh key
``` console
	ssh-keygen -t rsa -b 4096 -C <email_de_github>
	cat ~/.ssh/id_rsa.pub
```
Pegar lo que haya salido del comando anterior en github/settings/ssh & gpg keys

### 4 : Repositorios remotos

Asociar a repo de github a un repo local
``` console
	git remote add origin <direccion_url_o_ssh_al_repo_remoto>

```

Subir todos los commits nuevos al repo remoto
``` console
	git push origin <nombre_de_la_rama>
```

bajar cambios del repo remoto
``` console
	git pull origin <nombre_de_la_rama>
```

Bajar todo un repositorio de github, tuyo o de otros
``` console
	git clone <direccion_url_del_repo_remoto>
```

### 5 : Branching, trabajando con Ramas

Saber en qué rama estás
``` console
	git branch
```

Crear una rama nueva, y moverte a ella
``` console
	git checkout -b <nombre_de_la_nueva_rama>
```

Moverte a una rama existente
``` console
	git checkout <nombre_de_la_rama>
```

Moverte a un commit ("bolita en el tiempo"), de cualquier rama
``` console
	git checkout <commit_id(se obtiene con un git log c: )>
```

**Y aun falta más (unir ramas, comparar cambios, hacer deploy a GH pages) c: Espera la siguiente clase. En clasesnacho.com xDD**