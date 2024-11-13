---
description: Herramienta para realizar ataques de fuerza bruta en diversos protocolos.
---

# Hydra

## PARAMETROS

\-L -> Se indica el list users.&#x20;

\-P -> Se indica el listado de contraseña.

## COMANDOS

hydra -L \[list users] -P \[list pass] \[IP] ftp -> Ataque de fuerza bruta para el protocolo FTP.

hydra -L \[list users] -P \[list pass] \[IP] ssh -> Ataque de fuerza bruta para el protocolo SSH.

hydra -L \[list users] -P \[list pass] rdp://\[IP] \[-s\[puerto]] -> Ataque de fuerza bruta para el protocolo RDP.

hydra -l \[user] -P \[list pass] \[IP] mysql -> Ataque de fuerza bruta para el usuario de mysql.

hydra -l \[user] -P \[list pass] \[IP] http-get /webdav/ -> Ataque de fuerza bruta para el usuario de webdav.
