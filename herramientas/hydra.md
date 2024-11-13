---
description: Herramienta para realizar ataques de fuerza bruta en diversos protocolos.
---

# Hydra

## Parámetros de Hydra

* **-L**: Indica el archivo con la lista de usuarios.
* **-P**: Indica el archivo con la lista de contraseñas.
* **-l**: Especifica un usuario individual en lugar de una lista.

## Comandos de Hydra para Ataques de Fuerza Bruta

#### 1. FTP (File Transfer Protocol)

```bash
hydra -L [lista_usuarios] -P [lista_contraseñas] [IP] ftp
```

Realiza un ataque de fuerza bruta contra el protocolo FTP en la dirección IP especificada.

#### 2. SSH (Secure Shell)

```bash
hydra -L [lista_usuarios] -P [lista_contraseñas] [IP] ssh
```

Ejecuta un ataque de fuerza bruta contra el protocolo SSH en la IP indicada.

#### 3. RDP (Remote Desktop Protocol)

```bash
hydra -L [lista_usuarios] -P [lista_contraseñas] rdp://[IP] -s [puerto]
```

Lanza un ataque de fuerza bruta para el acceso remoto a través de RDP en la IP y puerto (opcional) especificados.

#### 4. MySQL

```bash
hydra -l [usuario] -P [lista_contraseñas] [IP] mysql
```

Ataque de fuerza bruta contra un usuario específico de MySQL en la dirección IP dada.

#### 5. WebDAV (HTTP GET)

```bash
hydra -l [usuario] -P [lista_contraseñas] [IP] http-get /webdav/
```

Realiza un ataque de fuerza bruta contra un usuario en un recurso web protegido por WebDAV, utilizando el método HTTP GET en la ruta indicada.
