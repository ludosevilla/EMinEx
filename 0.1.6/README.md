| [🇬🇧 English version](#eng) | [🇪🇸 Versión en español](#esp) |
|----------------------------|-----------------------------|

# Version 0.1.5

- **emx-0.1.6.com** : Version MSX-DOS "autonome", ne nécessite aucun pilote, compatible avec l’UART 16C550  
- **emx-F0.1.6.com** : Version MSX-DOS pour pilote Fossil, nécessite un pilote Fossil  
- **emx-C0.1.6.cas** et **emx-C0.1.6.wav** : Version cassette (sans lecteur de disquette installé)

## Utilisation (valable uniquement pour les versions MSX-DOS) :

`progname [vitesse [protocole]]`

- Sans aucun paramètre, **EMinEx** tentera de détecter automatiquement la vitesse du modem, en utilisant le protocole 8N1.

- Avec le paramètre **vitesse**, **EMinEx** communiquera à la vitesse spécifiée, en utilisant le protocole 8N1. Aucune détection automatique.  
  Vitesses disponibles pour la version autonome : 57600, 38400, 19200, 14400, 9600, 4800, 2400, 1200  
  Vitesses disponibles pour la version Fossil : 57600, 9600, 4800, 2400, 1200

- Avec le paramètre **protocole**, **EMinEx** utilisera le protocole spécifié :  
  - **XYZ** :  
    - **X** = nombre de bits (5, 6, 7 ou 8)  
    - **Y** = parité (O, E ou N)  
    - **Z** = bits de stop (1 ou 2)

La version cassette effectue toujours une détection automatique et ne prend en charge que l’UART 16C550.

## Exemples :

- `emx`  
- `emx 9600`  
- `emx 9600 7N1`

## Divers :
- **drv140.com** : Pilote Fossil 1.40 par Erik Maas.  

Après exécution, vous devrez taper `_system` pour revenir à MSX-DOS.

---
<a id="eng"></a>
# Version 0.1.6

- **emx-0.1.6.com** : "Standalone" MSX-DOS version, no need any driver, support UART 16C550  
- **emx-F0.1.6.com** : Fossil driver MSX-DOS version, needs Fossil driver
- **emx-C0.1.6.cas** and **emx-C0.1.6.wav** : Cassette version (without floppy installed)

## Usage (only for MSX-DOS versions):

`progname [speed [protocol]]`

- Without any parameter, **EMinEx** will try to detect the modem speed, using 8N1 protocol.

- With the **speed** parameter, **EMinEx** will communicate at the specified speed using the 8N1 protocol. No auto-detection.  
  Available speeds for standalone version: 57600, 38400, 19200, 14400, 9600, 4800, 2400, 1200  
  Available speeds for Fossil version: 57600, 9600, 4800, 2400, 1200

- With the **protocol** parameter, **EMinEx** will use the indicated protocol:  
  - **XYZ**:  
    - **X** = number of bits (5, 6, 7, or 8)  
    - **Y** = parity (O, E, or N)  
    - **Z** = Stop bits (1 or 2)

Cassette version will always perform auto-detection and only support UART 16C550

## Examples:

- `emx`  
- `emx 9600`  
- `emx 9600 7N1`

## Misc:
- **drv140.com** : Fossil driver 1.40 by Erik Maas.
  
After loading, you will need to type `_system` to return to MSX-DOS.

---
<a id="esp"></a>
# Versión 0.1.6

- **emx-0.1.6.com** : Versión MSX-DOS "independiente", no requiere ningún controlador, compatible con UART 16C550  
- **emx-F0.1.6.com** : Versión MSX-DOS con controlador Fossil, necesita un controlador Fossil  
- **emx-C0.1.6.cas** y **emx-C0.1.6.wav** : Versión en cassette (sin disquetera instalada)

## Uso (solo para versiones MSX-DOS):

`progname [velocidad [protocolo]]`

- Sin parámetros, **EMinEx** intentará detectar automáticamente la velocidad del módem, usando el protocolo 8N1.

- Con el parámetro **velocidad**, **EMinEx** comunicará a la velocidad indicada, usando el protocolo 8N1. Sin autodetección.  
  Velocidades disponibles para la versión independiente: 57600, 38400, 19200, 14400, 9600, 4800, 2400, 1200  
  Velocidades disponibles para la versión Fossil: 57600, 9600, 4800, 2400, 1200

- Con el parámetro **protocolo**, **EMinEx** usará el protocolo indicado:  
  - **XYZ**:  
    - **X** = número de bits (5, 6, 7 o 8)  
    - **Y** = paridad (O, E o N)  
    - **Z** = bits de parada (1 o 2)

La versión en cassette siempre realizará detección automática y solo admite UART 16C550.

## Ejemplos:

- `emx`  
- `emx 9600`  
- `emx 9600 7N1`

## Varios:
- **drv140.com** : Controlador Fossil 1.40 por Erik Maas.

Después de ejecutar, tendrás que escribir `_system` para volver a MSX-DOS.
