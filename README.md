# SonicScope

A free hi-res audio player for Windows and Linux, with tools for your music collection.

![SonicScope](image/SonicScope.jpg "SonicScope")

**[⬇ Download the latest version](../../releases/latest)**

*Deutsch und Русский: see below.*

Up to version 1.2.5, SonicScope was called AudioCluster.

## What it does

- **Player**: PCM up to 768 kHz and native DSD (DoP), gapless, bit-perfect output through WASAPI Exclusive. Also plays audio CDs straight from the drive.
- **Parametric EQ**: 16 bands, applied live, with presets.
- **Radio**: internet radio (MP3, Ogg, AAC, FLAC) with a catalog of stations, recording and scheduled recordings.
- **Converter**: converts to WAV, FLAC, WavPack, DSD or MP3, without changing the sound.
- **Disc Ripper**: rips audio CDs to WAV or FLAC.
- **Playlist Editor**: creates cue sheets, splits recordings into tracks, writes tags.
- **Library**: a searchable database of your music folders.
- **File Manager**: two panes, with audio tools.
- **Viewer**: Markdown, HTML and JSON.
- **Quality & Lineage**: checks whether a file was ever an MP3 and whether its hi-res rate is real.

The interface is in English, German and Russian (**View ▸ Language**). **Help ▸ Guide** (F1) explains every tab.

## Download and start

Pick a file from the [latest release](../../releases/latest):

| System | File | How to start |
|---|---|---|
| Windows 10/11, 64-bit | `SonicScope_x-y-z.zip` | Unpack it anywhere and double-click `SonicScope.exe`. Nothing is installed. |
| Linux x86_64, any distribution | `SonicScope-x.y.z-linux-x86_64.tar.gz` | Unpack it and start `SonicScope` in that folder. |
| Debian / Ubuntu | `sonicscope_x.y.z_amd64.deb` | `sudo apt install ./sonicscope_x.y.z_amd64.deb` |
| Linux, single file | `sonicscope-x.y.z-x86_64.AppImage` | `chmod +x` it, then run it. |

On Linux the system also needs `libportaudio2` (sound output) and `libwavpack1` (WavPack and DSD).

**Windows SmartScreen:** the program is not signed, so on the first start Windows may say "Windows protected your PC". Click **More info → Run anyway**. Each release lists the SHA-256 checksum of every file, so you can check that your download is the original one.

## Licence

SonicScope is free for personal, non-commercial use. You may pass it on free of charge, as long as the copy is complete and unchanged. The full terms are in [LICENSE](LICENSE).

SonicScope contains open-source components, each under its own licence. They are listed in [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md), the licence texts are in [licenses](licenses), and every download includes both. The source code of SonicScope itself is not published.

## Problems and questions

Please open an [issue](../../issues). Say which version and system you use, and what you did before the problem appeared.

---

## Deutsch

SonicScope ist ein kostenloser Hi-Res-Audioplayer für Windows und Linux, mit Werkzeugen für die eigene Musiksammlung: Player (bis 768 kHz, natives DSD, bit-perfekt), parametrischer EQ, Internetradio, Konverter, CD-Ripper, Cue-Sheet-Editor, Bibliothek und Dateimanager. Die Oberfläche gibt es auf Deutsch (**Ansicht ▸ Sprache**).

Bis Version 1.2.5 hieß SonicScope AudioCluster.

**[⬇ Neueste Version herunterladen](../../releases/latest)**

- **Windows:** die `.zip` entpacken und `SonicScope.exe` starten. Es wird nichts installiert. Meldet Windows „Der Computer wurde durch Windows geschützt“, dann auf **Weitere Informationen → Trotzdem ausführen** klicken. Das Programm ist nicht signiert.
- **Linux:** `.tar.gz`, `.deb` oder AppImage, wie in der Tabelle oben. Zusätzlich werden `libportaudio2` und `libwavpack1` gebraucht.

Die Nutzung ist für private, nicht-kommerzielle Zwecke kostenlos. Weitergeben dürfen Sie das Programm kostenlos und nur vollständig und unverändert. Die Bedingungen stehen in [LICENSE](LICENSE).

## Русский

SonicScope — бесплатный Hi-Res аудиоплеер для Windows и Linux с инструментами для музыкальной коллекции: плеер (до 768 кГц, нативный DSD, bit-perfect), параметрический эквалайзер, интернет-радио, конвертер, риппер CD, редактор cue, библиотека и файловый менеджер. Интерфейс есть на русском (**Вид ▸ Язык**).

До версии 1.2.5 SonicScope назывался AudioCluster.

**[⬇ Скачать последнюю версию](../../releases/latest)**

- **Windows:** распакуйте `.zip` и запустите `SonicScope.exe`. Установка не нужна. Если Windows пишет «Система Windows защитила ваш компьютер», нажмите **Подробнее → Выполнить в любом случае**. Программа не подписана.
- **Linux:** `.tar.gz`, `.deb` или AppImage, см. таблицу выше. Также нужны `libportaudio2` и `libwavpack1`.

Программа бесплатна для личного некоммерческого использования. Передавать её другим можно бесплатно, только полностью и без изменений. Условия описаны в [LICENSE](LICENSE).
