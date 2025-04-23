# TryHackMe-Journal
# TryHackMe Learning Journal 🚀

Bienvenue ! Ceci est un suivi de mon apprentissage en cybersécurité via [TryHackMe](https://www.tryhackme.com).  
Je documente ici mes progrès, mes découvertes importantes et les compétences acquises.

## 📋 Objectifs
1. Développer mes compétences en cybersécurité (pentesting, réseaux, Linux, etc.)
2. Expérimenter avec des scénarios réels.
3. Travailler vers des certifications reconnues.

---

## 💡 Apprentissage en cours
### 🌱 **Current Path**: Cybersecurity 101 learning path
🤖 **Progrès :** 1%  

Jour 1 :

# 🕵️‍♂️ Recherche des pages d'administration via Gobuster

Ce dossier documente l'usage de l'outil gobuster pour trouver une page d'administration dans un site web.  
Gobuster est un outil de **bruteforce** qui permet d’explorer des répertoires et des fichiers cachés sur un serveur.

---

## 🔧 **Pré-requis**
1. Avoir **Gobuster** installé :
   - Installation avec apt sur Kali Linux :  
     ```bash
     sudo apt install gobuster
     ```
2. Avoir un dictionnaire de mots (wordlist) :  
   - Par exemple, les wordlists par défaut de Kali Linux :  
     `/usr/share/wordlists/dirb/common.txt`

3. Le site cible : Une URL valide d’un site web à tester.

---

## 🔍 **Commande utilisée**
Voici la commande pour rechercher des pages potentiellement sensibles dans un site web :

```bash
gobuster dir -u http://example.com -w /usr/share/wordlists/dirb/common.txt

