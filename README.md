<div align="center">
  <h1>🎓 Étudiant en Cybersécurité | Passionné par l'Offensif & Red Team</h1>
  <p><em>Touche pas, c’est mon lab personnel. Mais si tu veux apprendre, bienvenue.</em></p>
</div>

---

[![Bannière](https://user-images.githubusercontent.com/79813703/224882534-09d61d4f-f019-45af-819c-918c8a1d3b83.gif)](https://github.com/ilyass-moussa) 

---

---
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Hacker Monkey</title>
  <style>
    body {
      background: #000;
      color: #fff;
      font-family: 'Courier New', Courier, monospace;
      overflow: hidden;
    }
    .terminal {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      background: rgba(0, 0, 0, 0.7);
      padding: 20px;
      border-radius: 5px;
      box-shadow: 0 0 10px #0f0;
    }
    .line {
      opacity: 0;
      white-space: pre;
      animation-fill-mode: forwards;
    }
    .glitch {
      position: relative;
      animation: glitch 1s infinite;
    }
    @keyframes glitch {
      0% { transform: translate(0, 0); }
      10% { transform: translate(-2px, 1px); text-shadow: -1px 0 red, 1px 0 cyan; }
      20% { transform: translate(1px, -2px); text-shadow: 1px 0 yellow, -1px 0 magenta; }
      30% { transform: translate(-1px, 0); text-shadow: none; }
      100% { transform: translate(0, 0); }
    }
    .cursor {
      display: inline-block;
      width: 10px;
      background: #0f0;
      animation: blinkCursor 1s infinite;
    }
    @keyframes blinkCursor {
      0%, 50% { opacity: 1; }
      50.01%, 100% { opacity: 0; }
    }
    .monkey {
      position: absolute;
      bottom: 10%;
      left: 10%;
      width: 150px;
    }
  </style>
</head>
<body>

<div class="terminal">
  <div class="line" id="boot1">[✓] LOADING KERNEL...</div>
  <div class="line" id="boot2">[✓] INIT CYBER_ENV...</div>
  <div class="line glitch" id="warning">[!] WARNING: ROOT_ACCESS</div>
  <div class="line" id="prompt1">(base) ┌──(root㉿kali)-[/home/hackerman]</div>
  <div class="line" id="prompt2">└─# █<span class="cursor"></span></div>
</div>

<img src="https://example.com/monkey_hacking.png"  alt="Hacker Monkey" class="monkey">

<script>
  // Fonction d'écriture caractère par caractère avec délai aléatoire
  function typeLine(element, text, delayMin = 50, delayMax = 150) {
    return new Promise(resolve => {
      let index = 0;
      element.textContent = '';
      const interval = setInterval(() => {
        if (index < text.length) {
          element.textContent += text.charAt(index);
          index++;
        } else {
          clearInterval(interval);
          resolve();
        }
      }, Math.random() * (delayMax - delayMin) + delayMin);
    });
  }

  async function runAnimation() {
    await typeLine(document.getElementById("boot1"), "[✓] LOADING KERNEL...");
    await typeLine(document.getElementById("boot2"), "[✓] INIT CYBER_ENV...");
    await typeLine(document.getElementById("warning"), "[!] WARNING: ROOT_ACCESS");

    // Clignotement rouge sur warning
    document.getElementById("warning").style.color = 'red';
    let redBlink = true;
    setInterval(() => {
      document.getElementById("warning").style.color = redBlink ? 'red' : '#0f0';
      redBlink = !redBlink;
    }, 500);

    // Ligne de prompt
    await typeLine(document.getElementById("prompt1"), "(base) ┌──(root㉿kali)-[/home/hackerman]");
    document.getElementById("prompt2").style.opacity = 1;

    // Curseur pulse
    const cursor = document.querySelector('.cursor');
    cursor.style.display = 'inline-block';

    // Attendre un peu avant afficher le nom final
    setTimeout(() => {
      alert("ALERTE : SINGE HACKER DÉTECTÉ !");
    }, 3000); // 3s après commande
  }

  runAnimation();
</script>

</body>
</html>
---


## 🔧 Compétences & Environnements

  ![Linux](https://img.shields.io/badge/-Linux-FCC624?logo=linux&logoColor=black)

<a href="https://www.archlinux.org/"><img alt="Arch Linux" title="Arch Linux" src="https://github.com/cheesits456/cheesits456/raw/master/icons/arch.png" height="42"></a>
![Arch Linux](https://img.shields.io/badge/-Arch_Linux-1793D1?logo=arch-linux&logoColor=white)
<a href="https://www.kali.org/"><img alt="Kali Linux" title="Kali Linux" src="https://upload.wikimedia.org/wikipedia/commons/2/2b/Kali-dragon-icon.svg" height="42"></a>
![Kali Linux](https://img.shields.io/badge/-Kali_Linux-557C94?logo=kali-linux&logoColor=white)
<a href="https://ubuntu.com/"><img alt="Ubuntu" title="Ubuntu" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/ubuntu/ubuntu.png" height="42"></a>
![Ubuntu](https://img.shields.io/badge/-Ubuntu-E95420?logo=ubuntu&logoColor=white)



  ![Windows Server](https://img.shields.io/badge/-Windows_Server-0078D6?logo=windows&logoColor=white)


<a href="https://www.gnu.org/software/bash/"><img alt="Bash" title="Bash" src="https://raw.githubusercontent.com/github/explore/master/topics/bash/bash.png" height="42"></a>
![Bash](https://img.shields.io/badge/-Bash-121011?logo=gnu-bash&logoColor=white)
<a href="https://www.python.org/"><img alt="Python" title="Python" src="https://raw.githubusercontent.com/github/explore/master/topics/python/python.png" height="42"></a>
![Python](https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white)
<a href="https://www.mysql.com/"><img alt="SQL" title="SQL" src="https://raw.githubusercontent.com/github/explore/master/topics/sql/sql.png" height="42"></a>
![SQL](https://img.shields.io/badge/-SQL-4479A1?logo=mysql&logoColor=white)


  <a href="https://github.com/"><img alt="GitHub" title="GitHub" src="https://raw.githubusercontent.com/github/explore/78df643247d429f6cc873026c0622819ad797942/topics/github/github.png" height="42"></a>
<a href="https://github.com/features/packages"><img alt="GitHub Packages" title="GitHub Packages" src="https://github.com/cheesits456/cheesits456/raw/master/icons/packages.png" height="42"></a>
![Wireshark](https://img.shields.io/badge/-Wireshark-1679A7?logo=wireshark&logoColor=white)
![Metasploit](https://img.shields.io/badge/-Metasploit-FF0000?logo=metasploit&logoColor=white)
![Burp Suite](https://img.shields.io/badge/-Burp_Suite-F47C20?logo=burp-suite&logoColor=white)
![Nmap](https://img.shields.io/badge/-Nmap-4F5D95?logo=nmap&logoColor=white)

---

## 🚀 Projets Académiques 

### PortScanner-Python  
Scanner de ports simple écrit en Python avec gestion des threads et détection du service en écoute.  
**Technologies :**  
![Python](https://img.shields.io/badge/Python-3776AB)   
![socket](https://img.shields.io/badge/socket-5C94FB)   
![threading](https://img.shields.io/badge/threading-4B8F75) 
🔗 [Voir le projet](https://github.com/ilyass-moussa/PortScanner-Python)

---

### Scapy-Packet-Analyzer  
Outil d’analyse réseau permettant de capturer et afficher des paquets TCP/UDP/DNS en temps réel.  
**Technologies :**  
![Python](https://img.shields.io/badge/Python-3776AB)   
![Scapy](https://img.shields.io/badge/Scapy-3A8FCD) 
🔗 [Voir le projet](https://github.com/ilyass-moussa/Scapy-Packet-Analyzer)

---

### Nmap-AutoScan  
Script en Bash automatisant les scans Nmap classiques (rapide, complet, vulnérabilités).  
**Technologies :**  
![Bash](https://img.shields.io/badge/Bash-4EAA25)   
![Nmap](https://img.shields.io/badge/Nmap-4F5D95) 
🔗 [Voir le projet](https://github.com/ilyass-moussa/Nmap-AutoScan)

---

## 🧠 Mon État d'Esprit Offensif

> “Pour bien défendre, il faut savoir attaquer.”  
> Je m'entraîne chaque jour à penser comme un attaquant, pour mieux comprendre comment se protéger.

---

## 📊 Statistiques GitHub (en temps réel)

📊 **Activité globale :**  
![Stats](https://github-readme-stats.vercel.app/api?username=ilyass-moussa&show_icons=true&theme=dracula)

🧮 **Langages utilisés :**  
![Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=ilyass-moussa&theme=dracula)

---

## 🔥 Centres d'intérêt 
- Tests d'intrusion réseaux/web  
- Techniques d'évasion  
- Tactiques Red Team  
- Recherche de vulnérabilités  

---



[![Visiteurs](https://visitor-badge.laobi.icu/badge?page_id=ilyass-moussa.ilyass-moussa)](https://github.com/ilyass-moussa)
