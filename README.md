# Mikrotik-Script-Monitoring LOG

## Link Script
[Monitoring Log](https://linktodocumentation)


## Server
```bash
 :local myserver ([/system identity get name]) 
 ```
 Fungsi yang akan menampilkan Nama Mikrotik Kita.
 ## Schedule
```bash
:local scheduleName "LogFilter"
```
Schedule di Mikrotik sebagai tanda/looping interval,silahkan sesuaikan dengan nama yang kalian buat interval jika Mikrotik Low spec bisa disetting 30-60sec,agar tidak memberatkan CPU dan proses RouterBoard Anda.
 ## BOT ID
 ```bash
:local bot "PASTE ID BOT"
:local ChatID "PASTE ID GRUP BOT"
```
Pastekan ID BOT Anda baik.
 ## Check Log Message
 ```bash
:local startBuf [:toarray [/log find message~"login failure"|| message~"logged in"]]
```
Script diatas akan mencari pesan yang ada login failure dan logged in
 ## Check Log via
 ```bash
 :local removeThese {"ftp"}
```
Silahkan bisa disesuaikan mana yang tidak akan dikirim ke bot anda..jika contoh diatas login via FTP tidak akan dikirim.
