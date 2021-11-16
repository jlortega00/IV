# Documentacion para añadir una clave pública a GitHub

Primero generaremos una nueva clave SSH.

```console
ssh-keygen -t ed25519 -C "your_email@example.com"
```

Esto crea una llave SSH utilizando el correo electrónico proporcionado como etiqueta.
Agrega tu llave privada SSH al ssh-agent. 
```console
ssh-add ~/.ssh/id_ed25519
```
Copiamos en el clickboard 
```console
clip < ~/.ssh/id_ed25519.pub
```
Finalmente nos vamos a SSH setting en GitHub y añadimos la nueva clave creada.
