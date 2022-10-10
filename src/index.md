---
theme: default
paginate: true
marp: true
---

# Configurando Apache

David Gómez Redondo

---

# Evitar funcionamiento con `https`

---

# Evitar funcionamiento sin `https`

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

# Gracias por su atención
