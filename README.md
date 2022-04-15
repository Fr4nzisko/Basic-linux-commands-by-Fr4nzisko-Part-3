# Basic linux commands by Fr4nzisko Part 3





## Directorio raiz del sistema*



````bash
/
````

*Archivos de configuración del sistema. (donde se almacenan las credenciales*
````bash
/etc
````

*Aloja programas en un sistemas. (comandos*
````bash
/usr
````

*Aloja programas instalados a posterior*
````bash
/opt
````

*Contiene a los usuarios*
````bash
/home
````

*Es el home del usuario root*
````bash
/root
````


*Archivo temporales, después se borrar automáticamente por el sistema*


````bash
/tmp
````

*Donde se guardar registro del sistema (registro de errores*
````bash
/var
````

*Archivo para envíar la información para que sea descartada*
````bash
/dev/null
````

# Directorio importante

*uso de grep :*
````bash
ls bin | grep nano
````

````bash
ls /usr/bin | grep ping
````

````bash
cat /etc/passwd 
````

````bash
which ping
````

````bash
grep fr4nzisko /etc/passwd
````

````bash
cat /etc/passwd | grep "kali"*kali:x:1000:1000:Kali,,,:/home/kali:/usr/bin/zsh
````


*nombre de usuario*
````bash
kali
````

*contraseña encriptada*
````bash
x
````


*id de usuario asignado (uid*
````bash
1000
````

*id de grupo (gid*
````bash
1000
````

*Nombre completo del usuario*
````bash
Kali,,,
````

*la ruta principal del usuario*
````bash
/home/kali/
````

*la shell que ocupa el usuario echo $SHELL*
````bash
/usr/bin/zsh
````

*ruta donde se almacena las contraseña de los usuarios*
````bash
/etc/shadow
````
![Captura de Pantalla 2022-04-15 a la(s) 16 30 02](https://user-images.githubusercontent.com/59784204/163629455-dfd330d9-edad-4ac9-bef8-ce51cc967aa4.png)

*Nombre de usuario*
````bash
kali
````

*Contraseña cifrada*
````bash
$y$
````

*Días transcurrido del cambio de credenciales*
````bash
17854
````

*Es modificable*
````bash
0
````

*Contraseña nunca caduca*
````bash
9999
````


*MD5*
````bash
$1$
````

*Blowfish*
````bash
$2$
````

*Blowfish*
````bash
$2y$
````

*SHA-256*
````bash
$5$
````

*SHA-512*
````bash
$6$
````

# Permisos de usuario 

````bash
chmod (+) (-) (rwx) (421) (pgp) 
````

*lectura*valor (4*
````bash
r
````

*escritura*valor (2*
````bash
w
````

*ejecucion*valor (1*
````bash
x
````

*ninguno*
````bash
0
````



*propietario (kali*
````bash
p
````

*grupos (otros usuario o grupos*
````bash
g
````

*otro*
````bash
o
````

*Referimos a todos los usuarios*
````bash
a
````

*Referimos al propietario*
````bash
u
````

*Referimos al grupo*
````bash
g
````

*Referimos a otros.*
````bash
o
````

# Saber a que tipo de dato nos enfrentamos al listar (ls -l )

*Directorio*
````bash
d
````

*Archivo de bloque.*
````bash
b
````

*Archivo especial de caracteres*
````bash
c
````

*Canal*
````bash
p
````

*Socket*
````bash
s
````

*Archivo normal*
````bash
-
````



*Es lo mismo que chmod ugo+rw fr4nzisko.txt da permiso a todos los usuarios*
````bash
chmod a+r fr4nzisko.txt
````

*Como arriba si no se indica a, u, g o o por defecto se toma a*
````bash
chmod +r fr4nzisko.txt
````

*rw-r-----*
````bash
chmod 640 fr4nzisko.txt
````

*rwxrwxrwx*
````bash
chmod 777 fr4nzisko.txt
````

*rwxrw--w-*
````bash
chmod 762 fr4nzisko.txt
````

````bash
sudo -l 
````

````bash
id
````

````bash
sudo su ($#)
````

````bash
su
````

````bash
passwd usuario 
````


# tmp

````bash
mktemp -d 
````

# Reiniciar el sistema

````bash
reboot 
````
