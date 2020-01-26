![image](https://github.com/V33RU/IoT-Penetration-Testing101-guide/blob/master/git.png)


# IoT-Penetration-Testing101-Guide

How to step into IoT penetration testing  
----------------------------------------------------------------------------------------------------------------------
 ## Software tools and hardware requirements:
 
|__IoT Penetration testing Framework__  |
| --------------------------------------|
| 1.[IoTSecFuzz](https://gitlab.com/invuls/iot-projects/iotsecfuzz)			        |
| 2.[Expliot Framework](https://gitlab.com/expliot_framework/expliot)                   |
| 3.[Routersploit](https://github.com/threat9/routersploit)			|


| __Firmware Reverse engineering:__     |
| --------------------------------------|
| 1. [binwalk](https://github.com/ReFirmLabs/binwalk)                            |
| 2. [firmwalker](https://github.com/craigz28/firmwalker)                         |
| 3. [FACT-core](https://github.com/fkie-cad/FACT_core)                          |
| 4. [radare2](https://github.com/radareorg/radare2)                            |
| 5. [capstone](http://www.capstone-engine.org/)                           |
| 6. [angr](https://github.com/angr/angr)                               |
| 7. [flawfinder](https://github.com/david-a-wheeler/flawfinder)                         |
| 8. [firmware modkit](https://github.com/rampageX/firmware-mod-kit)                    |
| 9. [r2ghidra-dec](https://github.com/radareorg/r2ghidra-dec)                       |
 

| __Firmware emulating:__	|
| ------------------------------|
| 1. [FAT tool](https://github.com/attify/firmware-analysis-toolkit)                   |
| 2. [Qemu](https://github.com/qemu/qemu)             		|	
| 3. [Qiling](https://github.com/qilingframework/qiling)         		|
| 4. [Firmadyne](https://github.com/firmadyne/firmadyne)        		|



| __BluetoothTool__ | __Hardware Requirements__ | 
| -------------------|---------------------------|
| [Gattacker](https://github.com/securing/gattacker)         | CSR 4.0                   | 
| [Bluez](http://www.bluez.org/)             | CSR 4.0                   | 
| [bettercap](https://www.bettercap.org/)         | CSR 4.0                   |
| [btlejuice](https://github.com/DigitalSecurity/btlejuice)         | CSR 4.0                   |
| [nrfconnect](https://www.nordicsemi.com/Software-and-tools/Development-Tools/nRF-Connect-for-desktop)        | NRF52840                  |
| [sniffle](https://github.com/nccgroup/Sniffle)           | TI CC1352R                |


	
|__Hardware:__	    |
| ------------------|
| 1.[flashrom](https://flashrom.org/Flashrom)        |
| 2.[openocd](https://github.com/ntfreak/openocd)         |
	
|__Apk Analyzers:__ |
| ------------------|
| 1.[MobSF](https://github.com/MobSF/Mobile-Security-Framework-MobSF)           |
| 2.[QARK](https://github.com/linkedin/qark)            | 
| 3.[Objection](https://github.com/sensepost/objection)       |

## Setup the Lab -- Download the OVA file from the below link 

- username : iotpentest
- password : iot
- <https://drive.google.com/open?id=1JQvY8TppPc7hz3V9fJU0PvWSIiNvX5YX>

## *write your own way approach to pentest device
--------------------------------------------------------------------------------------------------------------------------

### 1. Network pentesting on devices

### Embedded application
   
   <https://owasp.org/www-project-embedded-application-security/migrated_content>
    
### 2. Bluetooth pentesting
   
  - Gattacker
  
  - ___Running Gattacker___
    ![image](https://github.com/V33RU/Null-Bangalore-IoT-Security-101-workshop/blob/master/null/gattacker/gattacker1.JPG)
    
  - ___Running Gattacker___
    ![image](https://github.com/V33RU/Null-Bangalore-IoT-Security-101-workshop/blob/master/null/gattacker/gattacker2.JPG)
    
   - ___btlejuice___
   
   "BtleJuice is a complete framework to perform Man-in-the-Middle attacks on Bluetooth Smart devices (also known as Bluetooth Low Energy)"
   "BtleJuice is composed of two main components: an interception proxy and a core. These two components are required to run on independent machines in order to operate simultaneously two bluetooth 4.0+ adapters.
        - Running btlejuice
        - btlejuice-proxy (in vm)
        - btlejuice -u (ip address) -w (host linux)
        - localhost:8080 (in any webb browser)
     ![image](https://github.com/V33RU/Null-Bangalore-IoT-Security-101-workshop/blob/master/null/btlejuice/BTLE-JUICE.png)
    
   - ___bettercap___
        - #bettercap
        - ble.recon on (recon the devices)
        - ble.recon off (stopr the recon)
        - ble.show (to see all scanned devices surrounded by us)
        - ble enum (bd addr)
      ![image](https://github.com/V33RU/Null-Bangalore-IoT-Security-101-workshop/blob/master/null/bettercap/bettercap.png)
           
        
   - ___sudo bettercap -caplet https-ui (for web ui)___
      ![image](https://github.com/V33RU/Null-Bangalore-IoT-Security-101-workshop/blob/master/null/bettercap/Selection_003.png)
  
  
### 3. Firmware Revere engineering
    
   - ___FACT Tool (Firmware analysis comparison toolkti)___
      ![image](https://github.com/V33RU/Null-Bangalore-IoT-Security-101-workshop/blob/master/null/firmware/Selection_003.png)
     
   - ___FACT UI (after running script ui will load at https://127.0.0.1:5000)___
      ![image](https://github.com/V33RU/Null-Bangalore-IoT-Security-101-workshop/blob/master/null/firmware/FACT-UI.png)
         
      
### 4. Hardware Exploitation


### 5. Exploit Frameworks 
	
   ___expliot framework___
    ![image](https://github.com/V33RU/Null-Bangalore-IoT-Security-101-workshop/blob/master/null/exploit%20framework/expliot.JPG)
   
   ___IoTSecFuzz___
    ![image](https://github.com/V33RU/Null-Bangalore-IoT-Security-101-workshop/blob/master/null/exploit%20framework/iotsecfuzz.JPG)
   
   ___Routersploit___
    ![image](https://github.com/V33RU/Null-Bangalore-IoT-Security-101-workshop/blob/master/null/exploit%20framework/routersploit.JPG)
