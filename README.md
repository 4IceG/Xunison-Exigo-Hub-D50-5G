# Xunison-Exigo-Hub-D50-5G
My OpenWrt SNAPSHOT / LuCI Main build for the Xunison Exigo Hub D50 5G router [Build: XX.XX.2026]. Coming soon...

<p align="center">
<img src="https://github.com/4IceG/Personal_data/blob/master/xunisondevelop.png?raw=true" />
</p>

![GitHub release (latest by date)](https://img.shields.io/github/v/release/4IceG/Xunison-Exigo-Hub-D50-5G?style=flat-square)
![GitHub stars](https://img.shields.io/github/stars/4IceG/Xunison-Exigo-Hub-D50-5G?style=flat-square)
![GitHub forks](https://img.shields.io/github/forks/4IceG/Xunison-Exigo-Hub-D50-5G?style=flat-square)
![GitHub All Releases](https://img.shields.io/github/downloads/4IceG/Xunison-Exigo-Hub-D50-5G/total)

### <img src="https://raw.githubusercontent.com/4IceG/Personal_data/master/dooffy_design_icons_EU_flags_United_Kingdom.png" height="24"> OpenWrt installation procedure / <img src="https://raw.githubusercontent.com/4IceG/Personal_data/master/dooffy_design_icons_EU_flags_Poland.png" height="24"> Procedura instalacji OpenWrt

<details>
   <summary>Pokaż | Show me</summary>

![](https://forum.openwrt.org/uploads/default/original/3X/d/9/d92a1660e463e3b93a9c53158456a9fa1b3599ce.png)

Installing firmware / Recovery steps
1. Turn off the power
2. Press and hold the reset button
3. Turn on the power (reset cannot be released, the internet light will stay on after 10s)
4. Set the computer IP address to 192.168.1.2
subnet mask 255.255.255.0
gateway 192.168.1.1
5. Open the computer browser and enter 192.168.1.254
6. Select the firmware file (factory)
7. Click the update button once and wait for the router to restart
  
</details>

### <img src="https://raw.githubusercontent.com/4IceG/Personal_data/master/dooffy_design_icons_EU_flags_United_Kingdom.png" height="24"> What You Should Know / <img src="https://raw.githubusercontent.com/4IceG/Personal_data/master/dooffy_design_icons_EU_flags_Poland.png" height="24"> Co powinieneś wiedzieć

+ #### Installation of additional packages / Instalacja dodatkowych pakietów
> Snapshots are built daily, and that sets time limits to installing new packages with opkg. Due to kernel version checksums, you can only install “kmod” kernel modules and other kernel version dependent modules from the exactly same snapshot build. So, a few hours after flashing the firmware you may not be able to install new modules with opkg any more (as the next snapshot has been built into the download repo and has different checksums).   
> Obrazy snapshots budowane są codziennie, a to ustawia limity czasowe na instalację nowych pakietów za pomocą opkg. Z powodu sum kontrolnych wersji jądra, możesz zainstalować tylko moduły "kmod" i inne moduły zależne od wersji jądra z dokładnie tego samego snapshotu. Tak więc, kilka godzin po flashowaniu firmware możesz nie być w stanie zainstalować nowych modułów za pomocą opkg (ponieważ następny snapshot został wbudowany w repo i ma inne sumy kontrolne).

### <img src="https://raw.githubusercontent.com/4IceG/Personal_data/master/dooffy_design_icons_EU_flags_United_Kingdom.png" height="24"> Work is in progress on the final, functional image  / <img src="https://raw.githubusercontent.com/4IceG/Personal_data/master/dooffy_design_icons_EU_flags_Poland.png" height="24"> Trwają prace nad finalnym, działającym obrazem
