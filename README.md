# MeshCom Firmware (Beta v1.0)

Meshtastic Source-Code angepasst für MeshCom Projekt:

* Bluetooth PIN wurde fix auf "000000" gesetzt, erleichtert Verbindung mit dem Smartphone\
filename: nimble/BluetoothUtil.cpp, line 242\
filename: src/coniguration.h, line 592
* HOP_Limit für Nachrichten wurde auf 5 erhöht, damit Nachrichten im Mesh-Netzwerk 5 mal von anderen Nodes weitergesendet werden.\
filename: mesh/MeshTypes.h, line 37
* MeshCom logo und ÖVSV link\
filename: src/graphics/img/icon.xbm\
filename: src/graphics/Screen.cpp, line 127
* Beide sleep modi (light sleep, deep sleep) sind deaktiviert\
filename: src/sleep.cpp
* Wifi Refresh für Gateway reduziert auf 5sec\
filename: mesh/http/WifiAPClient.cpp, line 66
* Fixe Voreinstellung von:\
PSK Encryption NONE\
Channel: Very Long Range Very Slow (BW125kHz)\
Region: EU433\
filename: src/configuration.h, line 594-597



[Firmware fuer den TTGO TBeam (langes Board)](https://isemann.at/files/tbeam_meshcom_1.2.49_v1.0.bin)

[Firmware fuer den TLora (kleines Board)](https://isemann.at/files/tlora-v2_meshcom_1.2.49_v1.0.bin)

[Firmware fuer den Heltec](https://isemann.at/files/heltec-v2_meshcom_1.2.49_v1.0.bin)


ToDo:
* ShortName = Suffix ( MZC) oder CALL (OE3MZC/p)
* Reconnect to MeshCom server after reboot
