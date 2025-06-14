<p align="center">
  <img src="Vidéo sans titre ‐ Réalisée avec Clipchamp.gif" width="800" height="200" />
</p>

<h1 align="center">Salut 👋, je suis Ilyass Moussa</h1>

<div align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Hack&size=30&duration=2000&pause=3000&color=FF0000&center=true&vCenter=true&width=1050&lines=🎓+CYBERSÉCURITÉ+%7C+ÉTUDIANT+ORIENTÉ+OFFENSIF+%26+RED+TEAM" alt="Cybersécurité Red Team" />
</div>

---

<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com/?font=Consolas&size=30&duration=3000&pause=1000&color=00FF00&background=000000&center=true&vCenter=true&width=1050&lines=🎓+CYBERSÉCURITÉ+%7C+ÉTUDIANT+ORIENTÉ+OFFENSIF+%26+RED+TEAM" alt="Cybersécurité Red Team" />
</p>

---

## 🛠️ Arsenal Technique

### 🖥️ Systèmes & Environnements
<div align="center">
  <a href="https://archlinux.org/" target="_blank"><img src="https://img.shields.io/badge/Arch_Linux-1793D1?style=for-the-badge&logo=arch-linux&logoColor=white" alt="Arch Linux"/></a>
  <a href="https://www.kali.org/" target="_blank"><img src="https://img.shields.io/badge/Kali_Linux-557C94?style=for-the-badge&logo=kali-linux&logoColor=white" alt="Kali Linux"/></a>
  <a href="https://ubuntu.com/" target="_blank"><img src="https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white" alt="Ubuntu"/></a>
  <a href="https://www.microsoft.com/windows/server" target="_blank"><img src="https://img.shields.io/badge/Windows_Server-0078D6?style=for-the-badge&logo=windows&logoColor=white" alt="Windows Server"/></a>
</div>

### 🔍 Outils Offensifs
<div align="center">
  <a href="https://www.metasploit.com/" target="_blank"><img src="https://img.shields.io/badge/Metasploit-FF0000?style=for-the-badge&logo=metasploit&logoColor=white" alt="Metasploit"/></a>
  <a href="https://portswigger.net/burp" target="_blank"><img src="https://img.shields.io/badge/Burp_Suite-F47C20?style=for-the-badge&logo=burp-suite&logoColor=white" alt="Burp Suite"/></a>
  <a href="https://nmap.org/" target="_blank"><img src="https://img.shields.io/badge/Nmap-4F5D95?style=for-the-badge&logo=nmap&logoColor=white" alt="Nmap"/></a>
  <a href="https://www.wireshark.org/" target="_blank"><img src="https://img.shields.io/badge/Wireshark-1679A7?style=for-the-badge&logo=wireshark&logoColor=white" alt="Wireshark"/></a>
</div>

### 💻 Langages & Scripting
<div align="center">
  <a href="https://www.python.org/" target="_blank"><img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/></a>
  <a href="https://www.gnu.org/software/bash/" target="_blank"><img src="https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnu-bash&logoColor=white" alt="Bash"/></a>
  <a href="https://www.mysql.com/" target="_blank"><img src="https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" alt="SQL"/></a>
  <a href="https://docs.microsoft.com/powershell/" target="_blank"><img src="https://img.shields.io/badge/PowerShell-5391FE?style=for-the-badge&logo=powershell&logoColor=white" alt="PowerShell"/></a>
</div>

### ☁️ Plateformes
<div align="center">
  <a href="https://github.com/" target="_blank"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white&labelColor=000000&color=00FF00" alt="GitHub"/></a>
  <a href="https://github.com/features/packages" target="_blank"><img src="https://img.shields.io/badge/GitHub_Packages-181717?style=for-the-badge&logo=github&logoColor=white&labelColor=000000&color=FFD700" alt="GitHub Packages"/></a>
</div>

---

## 💥 Projets Phares

### 1. 🚨 **Advanced Port Scanner** [![Python](https://img.shields.io/badge/Python-3.8+-yellow?logo=python)](https://python.org)
> Scanner de ports multithread avec détection de services et analyse de vulnérabilités
```python
def scan_port(host, port):
    try:
        with socket.socket() as s:
            s.settimeout(1)
            s.connect((host, port))
            return True
    except:
        return False
