---
description: Herramienta para realizar ataques de fuerza bruta en diversos protocolos.
---

# Hydra

## Parámetros de Hydra

* **-L**: Indica el archivo con la lista de usuarios.
* **-P**: Indica el archivo con la lista de contraseñas.
* **-l**: Especifica un usuario individual en lugar de una lista.

## Comandos de Hydra

### FTP (File Transfer Protocol)

```bash
hydra -L [lista_usuarios] -P [lista_contraseñas] [IP] ftp
```

Realiza un ataque de fuerza bruta contra el protocolo FTP en la dirección IP especificada.

### SSH (Secure Shell)

```bash
hydra -L [lista_usuarios] -P [lista_contraseñas] [IP] ssh
```

Ejecuta un ataque de fuerza bruta contra el protocolo SSH en la IP indicada.

### RDP (Remote Desktop Protocol)

```bash
hydra -L [lista_usuarios] -P [lista_contraseñas] rdp://[IP] -s [puerto]
```

Lanza un ataque de fuerza bruta para el acceso remoto a través de RDP en la IP y puerto (opcional) especificados.

### MySQL

```bash
hydra -l [usuario] -P [lista_contraseñas] [IP] mysql
```

Ataque de fuerza bruta contra un usuario específico de MySQL en la dirección IP dada.

### WebDAV (HTTP GET)

```bash
hydra -l [usuario] -P [lista_contraseñas] [IP] http-get /webdav/
```

Realiza un ataque de fuerza bruta contra un usuario en un recurso web protegido por WebDAV, utilizando el método HTTP GET en la ruta indicada.

## Notas Adicionales

* **\[lista\_usuarios]**: archivo de texto que contiene una lista de nombres de usuarios, uno por línea.
* **\[lista\_contraseñas]**: archivo de texto con las posibles contraseñas, también una por línea.
* **\[IP]**: la dirección IP del objetivo.
* **-s \[puerto]**: (opcional) especifica un puerto si no es el puerto estándar del protocolo.
