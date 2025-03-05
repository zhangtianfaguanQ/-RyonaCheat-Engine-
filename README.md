[enable]
aobscanmodule(CALL_CHARABASE,DOA6.exe,48 8B C4 88 48 08 57 48 81 EC 80 00 00 00 48 C7 40 98 FE FF FF FF)
registersymbol(CALL_CHARABASE)
registersymbol(BryanyoraMem)
registersymbol(CameraPos_PN)
alloc(BryanyoraMem,4096,"DOA6.exe")
label(CameraPos_PN)

BryanyoraMem+0C:
db 00

BryanyoraMem+180:
CameraPos_PN:
db 00 01 08 09 0A 0B 02 00 00 00 00 00 00 00 00 00
BryanyoraMem+190:
db 0B 0A 09 08 01 00 02 00 00 00 00 00 00 00 00 00
BryanyoraMem+1A0:
db 07 07 00 00 00 00 00 00 00 00 00 00 00 00 00 00
BryanyoraMem+1B0:
dq 0000000000000000 0000000000000000
BryanyoraMem+1C0:
dq 0000000000000000 0000000000000000

[disable]
unregistersymbol(CALL_CHARABASE)
unregistersymbol(BryanyoraMem)
unregistersymbol(CameraPos_PN)
