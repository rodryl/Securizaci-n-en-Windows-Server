# Securización en Windows Server

## Vectores de ataques

OS - Parcheo de sistemas operativos - Protección de Virtual Patching para protección hasta conseguir una ventana de trabajo para aplicar os parches oficiales

Aplicaciones - Parcheo de aplicaciones - Protección de Virtual Patching para protección hasta conseguir una ventana de trabajo para aplicar os parches oficiales

Virtualización/Cloud - Protección de los hosts

Malware - Protección Antimalware en tiempo real y escaneos programados, Protección de Predictive Machine Learning vs Zero Day y Ransomware

Phishing - Protección de AntiSpam perimetral- Protección de AntiSpam interno

Ingeniería Social - 

Configuraciones Erróneas - Mala configuración de un servicio, etc

Certificados - Nivel de seguridad de certificados, Cuales? Renovarlos

## Prioridad 

Active Directory Domain Services - Control de las cuentas - Permisos que se pueden dar - Muchas apps usan autenticación con AD

Servidor de Email - Ataques de SPAM - 

Virtualización - Secuestro de máquinas virtuales dentro de los hosts

Servidores de ficheros - Robo de información 

Servidores de bases de datos - Robo o destrucción de información

Servidores Web - Alterar la información de la web - 

Servidores de AV - Desactivar los antivirus 

MECM - Desplegar software/malware a todos los equipos

## Generar estrategias de respuestas a incidentes

## Cumplimiento normativo 

Auditorías

Requerimientos de accesos y privilegios

Protección de datos

Encriptación

Copias de seguridad

## Brechas de seguridad - Métodos de detección

Alerta por el usuario del equipo

Herramientas nativas - Visor de eventos - Administrador de tareas - Sysinternals - Antivirus

Dispositivos de seguridad - logs y alertas de IDS, IPS y Firewalls

Comprobación de configuraciones

## LOGS

Mejorar el nivel de auditoria de los logs - Customizar los logs por defectos de Windows para que escriba logs más detallados - Cambiar todos los niveles de logeo modificando las configuraciones de auditoría a través de directivas de grupo

Monitoreo de logs - Implementación de Alertas mediante un SIEM ya que son demasiados logs. En cada servidor tenemos logs de aplicación, logs de seguridad, logs de sistema operativo

Los logs se deben guardar y no sobreescribir

Generar Scripts que generen alertas por mail cada 24hrs o más que nos alerten is hay algún cambio

## Sysinternals

Descarga: : https://docs.microsoft.com/en-us/sysinternals/downloads/sysinternals-suite

Listado de herramientas: : https://docs.microsoft.com/es-es/sysinternals/downloads/security-utilities

Utilidades de:

Archivos y discos

Red

Procesos

Seguridad

Información de sistemas

Otras

## Sysmon

Sirve para mejorar el nivel de logeo de un sistema:

Se instala

Ofrece información de: 

Creación de procesos

Conexiones de red

Cambios a las fechas de creación de archivos

Link: : https://docs.microsoft.com/en-us/sysinternals/downloads/sysmon

Comandos: 

## Accesschk 

Permite comprobar los accesos de usuarios y grupos a recursos como:

Ficheros

Directorios

Claves de registro

Objetos globales

Servicios

Link: : https://docs.microsoft.com/es-es/sysinternals/downloads/accesschk

Comandos:

## Logonsessions

Lista sesiones activas y procesos por sesión. Se pueden exportar a un CSV.

Comandos:

Link: : https://docs.microsoft.com/en-us/sysinternals/downloads/logonsessions

## Process Explorer

Muestra archivos y directorios abiertos por proceso

Cuando se ha lanzado un proceso

Si el proceso tiene comunicación por red

Uso de CPU

Uso de memoria

Link: : https://docs.microsoft.com/en-us/sysinternals/downloads/process-explorer

## Process Monitor

información en tiempo real de:

Registros

Sistema de archivos

Captura de información de los procesos

Captura de información de los servicios

Determina que claves de registros de aplicaciones guardan datos

Logea datos acerca de los eventos

Logeea todas las operaciones durante el arranque

Link: : https://docs.microsoft.com/en-us/sysinternals/downloads/procmon

## Sigcheck

Nos permite comprobar si un archivo fué comprometido.

Muestra información de:

Número de versión del fichero

Timestamp

Firma digital

Cadena de certificados

Estado del fichero en Virus Total

Link: : https://docs.microsoft.com/en-us/sysinternals/downloads/sigcheck

## Autoruns

Revisar Autoruns

Directorio Startup

Claves de registro

