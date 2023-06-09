# Virsh : KVM – Outil de virtualisation
KVM (Kernel-based Virtual Machine) est une virtualisation matérielle open source offrant performances élevées et facilité d'utilisation. Optimisé pour la virtualisation de serveur, KVM accélère les systèmes d'exploitation avec une utilisation optimale des ressources processeur et une compatibilité étendue. Solution performante et compatible pour la virtualisation de serveur.

## Documentation de KVM - Commandes Utiles

### virsh nodeinfo

La commande virsh nodeinfo affiche des informations sur l'hôte KVM, y compris le modèle de processeur, le nombre de sockets et de cœurs disponibles.

Exemple d'utilisation :

``$ virsh nodeinfo``

<p align="left">
  <img src="/img2/Vrish1.png" alt="Picture" >
</p>


### virsh dominfo <nom-de-la-machine-virtuelle>
La commande virsh dominfo affiche des informations d’une machine virtuelle, y compris la mémoire allouée, le nombre de processeurs, etc
 
Exemple d'utilisation :
  
``$ virsh dominfo nom-vm``
  
  <p align="left">
  <img src="/img2/vrish2.png" alt="Picture" >
</p>
  

### virsh list --all
  
La commande virsh list --all affiche la liste de toutes les machines virtuelles présentes sur l'hôte KVM.
  
Exemple d'utilisation :
  
``$ virsh list --all``
  
  <p align="left">
  <img src="/img2/vrish4.png" alt="Picture" >
</p>
  
  
### virsh domblklist <nom-de-la-machine-virtuelle>  
  
Voici une explication simplifiée des commandes pour afficher les informations sur le stockage d'une machine virtuelle KVM :
  
La commande virsh domblklist <nom-de-la-machine-virtuelle> pour afficher les périphériques de stockage et leurs sources de données. Cela nous permet de voir les périphériques utilisés, tels que "vda" et "hdc" et de connaître les chemins vers les fichiers d'image.
 
 Exemple d'utilisation :
  
 ``$ virsh domblklist <nom-de-la-machine-virtuelle>``
  
  <p align="left">
  <img src="/img2/vrish5.png" alt="Picture" >
</p>  
  
### virsh domblkinfo  
   
La commande virsh domblkinfo permet d'obtenir des informations détaillées sur un périphérique de stockage spécifique d'une machine virtuelle KVM.

Pour l'utiliser, remplacez <nom-de-la-machine-virtuelle> par le nom réel de votre machine virtuelle et <nom-du-périphérique> par le nom du périphérique de stockage dont vous souhaitez obtenir les informations. Par exemple, vous pouvez utiliser VDA comme nom du périphérique.
  
 Exemple d'utilisation :  
  
``$ virsh domblkinfo <nom-de-la-machine-virtuelle> <nom-du-périphérique> ``
  
  
  <p align="left">
  <img src="/img2/vrish6.png" alt="Picture" >
</p>  
  
 
  ### qemu-img info 
  
La commande qemu-img info affiche des informations détaillées sur un fichier d'image disque spécifique et connaître la taille réelle.
  
  Exemple d'utilisation :  
  
``$ qemu-img info <chemins-vers-les-fichiers-image> ``
  
   <p align="left">
  <img src="/img2/vrish8.png" alt="Picture" >
</p>  
  
  
Pour calculer 10G en octets, vous pouvez utiliser la formule suivante :
 ###### 10 gigaoctets = '10 * 1024 * 1024 * 1024 octets'
Ce calcul donne une taille de ``10 737 418 240 octets`` .
  
________________________________________________________________________________________________________________________________________________________
  
  ## References
  
  https://manpages.ubuntu.com/manpages/trusty/man1/qemu-img.1.html
  
  https://en.wikiversity.org/wiki/KVM/qemu-img/qemu-img_info
  
  https://www.redhat.com/en/topics/virtualization/what-is-KVM
  
  https://www.cyberithub.com/virsh-commands-examples-virt-df-virt-top-kvm/
  
  https://computingforgeeks.com/virsh-commands-cheatsheet/
  
  https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/7/html/virtualization_deployment_and_administration_guide/sect-statlists
  
  https://bugzilla.redhat.com/show_bug.cgi?id=1330940
  
  https://docs.oracle.com/en/operating-systems/oracle-linux/kvm-user/kvm-KVMUsage.html#section_xwd_hnd_c5b
  
  https://qemu.readthedocs.io/en/latest/tools/qemu-img.html
  
  
  
