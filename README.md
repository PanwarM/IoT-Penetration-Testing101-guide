![image](https://github.com/V33RU/IoT-Penetration-Testing101-guide/blob/master/git.PNG)


# IoT-Penetration-Testing101-Guide

How to step into IoT penetration testing  
----------------------------------------------------------------------------------------------------------------------
 ## Software tools and hardware requirements:
 
|__IoT Penetration testing Framework__  |
| --------------------------------------|
| 1.[IoTSecFuzz](https://gitlab.com/invuls/iot-projects/iotsecfuzz)			        |
| 2.Expliot Framework                   |
| 3.Routersploit			|


| __Firmware Reverse engineering:__     |
| --------------------------------------|
| 1. binwalk                            |
| 2. firmwalker                         |
| 3. FACT-core                          |
| 4. radare2                            |
| 5. capstone                           |
| 6. angr                               |
| 7. flawfinder                         |
| 8. firmware modkit                    |
| 9. r2ghidra-dec                       |
 

| __Firmware emulating:__	|
| ------------------------------|
| 1. FAT tool                   |
| 2. Qemu             		|	
| 3. Qiling         		|
| 4. Firmadyne        		|



| __BluetoothTool__ | __Hardware Requirements__ | 
| -------------------|---------------------------|
| Gattacker         | CSR 4.0                   | 
| Bluez             | CSR 4.0                   | 
| bettercap         | CSR 4.0                   |
| btlejuice         | CSR 4.0                   |
| nrfconnect        | NRF52840                  |
| sniffle           | TI CC1352R                |


	
|__Hardware:__	    |
| ------------------|
| 1.flashrom        |
| 2.openocd         |
	
|__Apk Analyzers:__ |
| ------------------|
| 1.MobSF           |
| 2.QARK            | 
| 3.Objection       |

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
