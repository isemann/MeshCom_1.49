# MeshCom Firmware (Beta)

Meshtastic Source-Code angepasst für MeshCom Projekt:

/*
* Bluetooth PIN wurde fix auf "000000" gesetzt, erleichtert Verbindung mit dem Smartphone
filename: nimble/BluetoothUtil.cpp, line 242
filename: src/coniguration.h, line 592
* HOP_Limit für Nachrichten wurde auf 5 erhöht, damit Nachrichten im Mesh-Netzwerk 5 mal von anderen Nodes weitergesendet werden.
filename: mesh/MeshTypes.h, line 37
* MeshCom logo
filename: src/graphics/img/icon.xbm
* Beide sleep modi (light sleep, deep sleep) sind deaktiviert

* Wifi Refresh für Gatway reduziert auf 5sec
*filename: src/sleep.cpp

Zum Source-Code auf Github geht es [hier.](https://github.com/isemann/MeshCom)

[Firmware fuer den TTGO TBeam (langes Board)](https://isemann.at/files/tbeam_meshcom_1.2.48_v0.9.bin)

[Firmware fuer den TLora (kleines Board)](https://isemann.at/files/tlora-v2_meshcom_1.2.48_v0.9.bin)

[Firmware fuer den Heltec](https://isemann.at/files/heltec-v2_meshcom_1.2.48_v0.9.bin)


Ein weiteres Update der Firmware ist in Arbeit das folgende Aenderungen beinhaltet:

fixe Voreinstellung von:
PSK Encryption NONE,
Channel: Very Long Range Very Slow (BW125kHz)
Region: EU433
ShortName = Suffix ( MZC) oder CALL (OE3MZC/p)
