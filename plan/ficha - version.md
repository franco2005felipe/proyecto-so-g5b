| Pregunta | Respuesta | Enlace |
|---|---|---|
| Versión y fecha | Lubuntu 26.04.1, ISO publicada el 26/08/2026 | https://cdimage.ubuntu.com/lubuntu/releases/resolute/release/ |
| Archivo descargado | lubuntu-26.04.1-escritorio-amd64.iso (3,7 GB, escritorio, 64 bits) | https://cdimage.ubuntu.com/lubuntu/releases/resolute/release/ |
| Hipervisor | VirtualBox 7.2.22 | https://www.virtualbox.org/wiki/Downloads |

## Zorin OS (VM gráfica)

| Pregunta | Respuesta | Enlace donde lo comprobamos |
|---|---|---|
| Versión elegida y fecha de lanzamiento | Zorin OS 18.1 (lanzada el 15 de abril de 2026; la versión mayor Zorin OS 18 salió el 14 de octubre de 2025). | https://zorin.com/os/details/ |
| Hasta cuando recibe actualizaciones de seguridad | Hasta el 1 de junio de 2029. | https://zorin.com/os/details/ |
| Requisitos de hardware y si funciona en VirtualBox | Mínimos: procesador Dual-Core 1 GHz (64-bit), 2 GB de RAM y 15 GB de disco (recomendado 4 GB RAM y 32 GB disco). Sí funciona en VirtualBox (ej. con 4 GB de RAM y 2 CPU). | https://zorin.com |
| ¿El instalador permite particionar manualmente? | Sí. El instalador (Ubiquity) ofrece la opción «Más opciones» (Something else) para crear, redimensionar y asignar particiones manualmente. | https://zorin.com |
| Guía oficial para instalar Docker Engine en esa familia | Docker no tiene una página dedicada a Zorin OS. Como está basado en Ubuntu 24.04 LTS, se usa la guía oficial de Ubuntu y lo dejamos documentado. | https://docker.com |
| Imagen base del Dockerfile para esa versión | No existe imagen oficial de Zorin OS en Docker Hub. Para replicar su base se utiliza la imagen oficial `ubuntu:24.04` (o la asignada al grupo). | https://docker.com |

## Fedora Server (VM de consola)

| Pregunta | Respuesta | Enlace donde lo comprobamos |
|---|---|---|
| Versión elegida y fecha de lanzamiento | Fedora Server 45 (lanzada el 3 de noviembre de 2026). | https://docs.fedoraproject.org/en-US/releases/ |
| Hasta cuando recibe actualizaciones de seguridad | Aproximadamente 13 meses tras su lanzamiento (hasta el 8 de diciembre de 2027, 4 semanas después de salir Fedora 47). | https://docs.fedoraproject.org/en-US/releases/ |
| Requisitos de hardware y si funciona en VirtualBox | Mínimos: procesador de 2 GHz (2 núcleos), 2 GB de RAM y 15 GB de disco. Sí funciona en VirtualBox (ej. con 2 GB de RAM y 2 CPU). | https://fedoraproject.org |
| ¿El instalador permite particionar manualmente? | Sí. El instalador (Anaconda) cuenta con la opción de almacenamiento «Personalizada» (Custom) para configurar particiones y volúmenes LVM manualmente. | https://fedoraproject.org |
| Guía oficial para instalar Docker Engine en esa familia | Sí, Docker cuenta con documentación oficial específica para Fedora. | https://docker.com |
| Imagen base del Dockerfile para esa versión | La imagen oficial existe en Docker Hub como `fedora` con la etiqueta `45` (`fedora:45`). | https://docker.com |

## Ubuntu (Imagen base de Docker)

| Pregunta | Respuesta | Enlace donde lo comprobamos |
|---|---|---|
| Versión elegida y fecha de lanzamiento | Ubuntu 26.04.1 LTS *Resolute Raccoon* (lanzada el 27 de agosto de 2026; la versión 26.04 LTS inicial salió el 23 de abril de 2026). | https://ubuntu.com/project/docs/release-team/list-of-releases/ |
| Hasta cuando recibe actualizaciones de seguridad | Soporte estándar hasta mayo de 2031 (5 años) y soporte extendido (ESM con Ubuntu Pro) hasta abril de 2036. | https://ubuntu.com/about/release-cycle |
| Requisitos de hardware y si funciona en VirtualBox | Mínimos (Server): procesador de 1 GHz, 1 GB de RAM y 2.5 GB de disco (Desktop: 2 GHz dual-core, 4 GB RAM, 25 GB disco). Sí funciona en VirtualBox; como contenedor Docker usa directamente el kernel del host. | https://ubuntu.com |
| ¿El instalador permite particionar manualmente? | Sí. Tanto el instalador de Server (Subiquity) como el de Desktop permiten elegir «Custom storage layout» / «Manual partitioning». (En Docker no aplica instalador, ya que se despliega desde imagen). | https://ubuntu.com |
| Guía oficial para instalar Docker Engine en esa familia | Sí, Docker dispone de una guía oficial exclusiva para Ubuntu mediante su repositorio `apt`. | https://docker.com |
| Imagen base del Dockerfile para esa versión | La imagen oficial existe en Docker Hub con la etiqueta `ubuntu:26.04` (o `ubuntu:noble` / `ubuntu:24.04` si el proyecto requiere la LTS anterior). | https://docker.com |
