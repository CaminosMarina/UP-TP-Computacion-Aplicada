# Cómo reconstruir

Cada directorio está comprimido por separado en un archivo .tar.gz:
- root.tar.gz
- etc.tar.gz
- opt.tar.gz
- www_dir.tar.gz
- backup_dir.tar.gz

/var está dividido en 3 partes (split -n 3 -d). Para unirlas y descomprimirlas:
- cat var.tar.gz.part_* | tar -xzvf -
