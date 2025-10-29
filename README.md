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
azureuser@VM1:~$ ssh-keygen -t ed25519 -f ~/.ssh/cloud_tp
Generating public/private ed25519 key pair.
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Passphrases do not match.  Try again.
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /home/azureuser/.ssh/cloud_tp
Your public key has been saved in /home/azureuser/.ssh/cloud_tp.pub
The key fingerprint is:
SHA256:SSggBacCs9EKNssnmyWRBVyEdt5yW7W796elr53lz4s azureuser@VM1
The key's randomart image is:
+--[ED25519 256]--+
|B=@+             |
|o/.o   . .       |
|O.* o . o .      |
|o= = + o o       |
|  B o o S .      |
| o   .   .       |
|          .    ..|
|         . .  =+o|
|          . .E==*|
+----[SHA256]-----+
```




