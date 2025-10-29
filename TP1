# TP-PANORAMA-DU-CLOUD

## A. Choix de l'algorithme de chiffrement

🌞 Déterminer quel algorithme de chiffrement utiliser pour vos clés

Pour chiffrer mes clés j'ai utilisé ed25519


- Pourquoi éviter RSA comme algorithme de chiffrement pour nos clés
[https://devblogs.microsoft.com/devops/ssh-rsa-deprecation]

-Pourquoi utiliser ED25519 comme algorithme de chiffrement pour mes clés.
[https://www.brandonchecketts.com/archives/ssh-ed25519-key-best-practices-for-2025#:~:text=Although%20the%20256-bit%20ed25519,a%20similar%20level%20of%20security.]



## B. Génération de votre paire de clés¶

🌞 Générer une paire de clés pour ce TP

```sh
PS C:\Users\gusta> ssh-keygen -t ed25519 -f "$HOME\.ssh\cloud_tp"
Generating public/private ed25519 key pair.
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in C:\Users\gusta\.ssh\cloud_tp
Your public key has been saved in C:\Users\gusta\.ssh\cloud_tp.pub
The key fingerprint is:
SHA256:D9uLaPg0i+2GBTpMuiDTRrb5qUICRm/8t9g55fMwra0 gusta@NATHANHO_AMB
The key's randomart image is:
+--[ED25519 256]--+
|                 |
| .               |
|. o              |
|..++.            |
|oB.+..  S        |
|*.O  ... *.      |
|=+ o =* *oo.     |
|o   ==oO +=.     |
| ....=* oE=o     |
+----[SHA256]-----+
```


## C. Agent SSH

🌞 Configurer un agent SSH sur votre poste

- Démarrage et activation de l'agent ssh
```sh
PS C:\Users\gusta> Start-Service "ssh-agent"
PS C:\Users\gusta> Get-Service "ssh-agent"

Status   Name               DisplayName
------   ----               -----------
Running  ssh-agent          OpenSSH Authentication Agent
```
- Ajout de la clé à l'agent et vérification
  ```sh
PS C:\Users\gusta> ssh-add "$HOME\.ssh\cloud_tp"
Enter passphrase for C:\Users\gusta\.ssh\cloud_tp:
Identity added: C:\Users\gusta\.ssh\cloud_tp (gusta@NATHANHO_AMB)
PS C:\Users\gusta> ssh-add -l
256 SHA256:D9uLaPg0i+2GBTpMuiDTRrb5qUICRm/8t9g55fMwra0 gusta@NATHANHO_AMB (ED25519)
```


  










