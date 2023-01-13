# Generalità
Usa punto interrogativo per vedere comandi available

per esempio 
**switch>e?
enable exit 
switch>**

Primo comando 
sw1>enable

"entri in modalita attiva"

----
Da modalita attiva passi a modalita configurazione


Switch>enable
Switch#conf t
Enter configuration commands, one per line.  End with CNTL/Z.
Switch(config)#enable password CCNA
Switch(config)#exit
Switch#
%SYS-5-CONFIG_I: Configured from console by console

Switch#exit

Switch>enable
Password: 
Switch#show running-conf
Building configuration...

Current configuration : 1103 bytes
!
version 15.0
no service timestamps log datetime msec
no service timestamps debug datetime msec
no service password-encryption
!
hostname Switch
!
enable password CCNA


come vedi è leggibile in chiaro

THERE ARE TWO CONFIGURATION FILE
Running-config = file configurazione in esecuzione
Startup-config = File configurazione eseguito al reboot
PER SALVARE LE CONFIGURAZIONI FATTE USA 

Switch#write
Building configuration...
[OK]
Switch#copy running-config startup-config
Destination filename [startup-config]? 
Building configuration...
[OK]
Switch#

CONTROLLA SE HA SALVATO NEL FILE GIUSTO

Switch#show startup-config 
Using 1103 bytes
!
version 15.0
no service timestamps log datetime msec
no service timestamps debug datetime msec
no service password-encryption
!
hostname Switch
!
enable password CCNA
!
!
PER TOGLIERE LA PASSWORD IN CHIARO
Switch#conf ter
Enter configuration commands, one per line.  End with CNTL/Z.
Switch(config)#service password-en
Switch(config)#service password-encryption 
Switch(config)#show runn
Switch(config)#show running-
Switch(config)#do show runni
Switch(config)#do show running-config
Building configuration...

Current configuration : 1108 bytes
!
version 15.0
no service timestamps log datetime msec
no service timestamps debug datetime msec
service password-encryption
!
hostname Switch
!
enable password 7 08026F6028
!
!
!
!
!
!
spanning-tree mode pvst
spanning-tree extend system-id
!
interface FastEthernet0/1

OSSERVA CHE ALGORITMO 7 è FACILMENTE CRACCABILE MEGLIO USARE ALLORA

Switch(config)#enable secret Cisco
Switch(config)#do show running-conf
Building configuration...

Current configuration : 1155 bytes
!
version 15.0
no service timestamps log datetime msec
no service timestamps debug datetime msec
service password-encryption
!
hostname Switch
!
enable secret 5 $1$mERr$YlCkLMcTYWwkF1Ccndtll.
enable password 7 08026F6028
!
VEDI CHE IN QUESTO MODO NON VIENE USATO ALGORITMO 7 MA IL 5 CHE E' MD5

Router>          = user EXEC mode
Router#          = privileged EXEC mode
Router(config)#  = global configuration mode
Router>enable ##used to enter privileged EXEC mode
Router#configure terminal  ##used to enter global configuration mode
Router(config)#enable password password  ##configures a password to protect privileged exec mode
Router(config)#service password-encryption ##encrypts the enable password (and other passwords)
Router(config)#enable secret password ##configures a more secure, always-encrypted enable password
Router(config)#do privileged-exec-level-command ##executes a privileged-exec level command from global configuration mode


Router(config)#no command##removes the command
Router#show running-config##displays the current, active configurtion file
Router#show startup-config##displays the saved configuration file which will be loaded if the device is restarted
Router#write ##saves the configuration
Router#write memory##saves the configuration
Router#copy running-config startup-config##saves the configuration