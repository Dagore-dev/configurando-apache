---
theme: default
paginate: true
marp: true
---

# Configurando Apache

David Gómez Redondo

---

# Evitar funcionamiento con `https`

Para ello, en el fichero `httpd-ssl.conf` se debe comentar la orden `Listen 443`.

![](/assets/images/disable-ssl.png)

---

# Evitar funcionamiento sin `https`

Para ello, en el fichero `httpd.conf` se debe comentar la orden `Listen 80`. El resto de configuraciones se hacen en este fichero.

![](/assets/images/disable-http.png)

---

# Acceso al servidor por el puerto 98

Se modifica con la orden `Listen`.

![](/assets/images/listen-98.png)

---

# Cambiar `htdocs` de lugar

Se modifica `DocumentRoot` y se agregan los permisos de acceso con un bloque `Directory`.

![](/assets/images/document-root.png)

---

# Aplicación de arranque `patata.php`

Con el `dir_module` habilitado se modifica el `DirectoryIndex`.

![](/assets/images/directory-index.png)

---

# Impedir accesos al servidor

Los accesos al servidor están habilitados con la orden `Require all granted` dentro del bloque `Directory específico`. Basta con comentarlo.

![](/assets/images/deny-access.png)

---

# Acceder al "Hola mundo cruel" de un compañero de mesa

Para esto solo hay que acceder a la dirección `IP` del equipo del compañero puesto que compartimos la misma red.

![](/assets/images/hola-mundo-cruel-santi.png)

---

# Tema libre: Cambiar el correo del administrador del servidor

El administrador del servidor se define con la orden `ServerAdmin`.

![](/assets/images/server-admin.png)

---

# Tema libre: Impedir el acceso a los fichero `.env`

Se utiliza un bloque `Files` donde se especifica el patrón y la orden `Require all denied`.

![](/assets/images/deny-env-files.png)

---

# Tema libre: 

---

# Gracias por su atención
