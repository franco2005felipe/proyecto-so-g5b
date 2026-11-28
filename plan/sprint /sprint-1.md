# Sprint 1 Montaje 
## 1. VM gráfica Zorin 18.1
<img width="1137" height="738" alt="image" src="https://github.com/user-attachments/assets/56f72c04-e805-425d-ba0b-5f8ecb2e3ee6" />


## Tabla de como lo distribuimos

| Partición | Tamaño | Por qué |
|---|---|---|
| `/` | 20 GB | El sistema y los programas, con margen para actualizar |
| `swap` | 2 GB | Igual a la RAM de la VM, por si falta memoria |
| `/home` | 4.8 GB | Los archivos de los usuarios, separados del sistema |

## 2. VM de consola (g05b-consola)
Captura 4: se muestra los comandos pedidos (lsblk, df -h y cat /etc/fstab de g07-consola, con prompt y fecha)

<img width="1273" height="818" alt="image" src="https://github.com/user-attachments/assets/f55e7786-12e9-47cc-809c-8c376023b535" />

Captura 5: las cinco herramientas mostrando su versión

<img width="1275" height="828" alt="image" src="https://github.com/user-attachments/assets/0165745f-d1ac-4a81-9968-cc9dd717916a" />

## 3. Red
Captura 6: ip a en las dos VMs, mostrando una dirección en cada interfaz
<img width="1326" height="995" alt="fedora ip" src="https://github.com/user-attachments/assets/c727d966-7864-45e2-a452-9388a698247b" />

Captura 7: ping de la gráfica a la consola y de la consola a la gráfica
<img width="1461" height="1020" alt="evidencia ping fedora" src="https://github.com/user-attachments/assets/b688572b-10e0-4bbb-af6b-09cc765ec486" />

## 4. SSH
Captura 8: la sesión SSH abierta, con el prompt de la consola
<img width="1431" height="1000" alt="sprint1_conexion ssh zorin a fedora" src="https://github.com/user-attachments/assets/736d8af7-4eed-4484-8243-14f90f33177d" />


## 5. Instantáneas
## Captura 9: pestaña de instantáneas de g05b-grafica
<img width="1917" height="1077" alt="Zorin_Instantanea_Instalacion_Limpia(parte 5)" src="https://github.com/user-attachments/assets/7910e259-eb21-42ac-9372-cae3a84b0dcf" />


## Captura 10: pestaña de instantáneas de g05b-consola
<img width="976" height="761" alt="image" src="https://github.com/user-attachments/assets/8ddad52b-eeb7-49c1-abfa-6858dee8b63f" />


## Código del sprint
g05b-grafica


g05b-consola
<img width="1182" height="819" alt="image" src="https://github.com/user-attachments/assets/b01d7c9f-2f86-4976-b566-f05aeb17f7b4" />
