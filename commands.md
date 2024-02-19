# Basic SysAdmin

## Informazioni di Sistema:

- `uname -a`: Mostra le informazioni di sistema.
- `free -m`: Mostra l'utilizzo della memoria.
- `df -ah`: Mostra l'utilizzo dello spazio su disco in formato human-readable.
- `du -sh`: Mostra l'utilizzo dello spazio su disco di un file o una directory in formato human-readable.
- `top`: Mostra una vista dinamica e in tempo reale delle risorse di sistema.
- `htop`: Versione più colorata e interattiva di `top`.

## Operazioni su File e Directory:

- `ls -la`: Elenca file e directory in modo dettagliato (anche nascosti).
- `cat nomeFile`: Mostra il contenuto di un file.
- `grep modello nomeFile`: Cerca un modello in un file.
- `find /percorso -name nomeFile`: Cerca file in una gerarchia di directory.
- `lsof`: Fornisce informazioni dettagliate sui file aperti dai processi.
- `touch nomeFile`: Crea un nuovo file vuoto o aggiorna l'orario di accesso di un file esistente.
- `cp origine destinazione`: Copia file o directory.
- `mv origine destinazione`: Sposta o rinomina file o directory.
- `rm nomeFile`: Rimuove (elimina) un file.
- `mkdir nomeDirectory`: Crea una nuova directory.
- `chmod permessi nomeFile`: Modifica i permessi di accesso di un file.
- `chown utente:gruppo nomeFile`: Cambia il proprietario e il gruppo di un file.

## Configurazione di Sistema:

- `lsmod`: Elenca i moduli del kernel caricati.
- `sysctl -a`: Mostra i parametri del kernel.
- `lspci`: Mostra informazioni dettagliate sui dispositivi PCI.
- `lshw`: Mostra informazioni dettagliate sull'hardware.
- `uname -r`: Mostra la versione del kernel.
- `lsblk`: Elenca le informazioni sui dispositivi di blocco.
- `fdisk -l`: Mostra le informazioni sulle partizioni del disco.
- `chkconfig --list`: Visualizza lo stato di avvio dei servizi.
- `systemctl enable nomeServizio`: Abilita un servizio all'avvio del sistema.
- `systemctl disable nomeServizio`: Disabilita un servizio all'avvio del sistema.

## Sicurezza e Firewall:

- `firewall-cmd --zone=public --add-port=NUMERO/protocollo --permanent`: Apri una porta nel firewall.
- `firewall-cmd --reload`: Ricarica le regole del firewall.
- `firewall-cmd --state`: Mostra lo stato del firewall.
- `firewall-cmd --list-all`: Mostra dettagli sulla configurazione del firewall.
- `sestatus`: Mostra lo stato di SELinux.
- `setenforce 0`: Disabilita temporaneamente SELinux.
- `getenforce`: Mostra lo stato di SELinux (Enforcing, Permissive, Disabled).
- `iptables -L`: Elenca le regole del firewall.

## Risoluzione Problemi di Rete:

- `ip a`: Mostra le interfacce di rete e le loro configurazioni.
- `nslookup`: Effettua interrogazioni DNS.
- `ping nomeHost`: Verifica la connettività a un host.
- `traceroute nomeHost`: Mostra il percorso che i pacchetti seguono per raggiungere un host.
- `ss`: Visualizza le connessioni di rete.
- `ip route show`: Mostra la tabella di routing.
- `ip neigh show`: Visualizza la tabella ARP per le associazioni IP/MAC.
- `ip link show`: Mostra tutte le interfacce, anche quelle non attive.

## Log e Messaggi di Sistema:

- `dmesg`: Mostra i messaggi nel buffer del kernel.
- `journalctl -xe`: Visualizza i log di sistema in modo esteso e direttamente dalla fine del registro.
- `tail -f /var/log/syslog`: Monitora il log di sistema in tempo reale.
- `ls /var/log/`: Visualizza l'elenco dei file di log disponibili.
- `cat /var/log/messages`: Mostra il contenuto del file di log dei messaggi di sistema.

## systemctl

- `systemctl status nomeServizio`: Mostra lo stato di un servizio.
- `systemctl stop nomeServizio`: Arresta un servizio.
- `systemctl start nomeServizio`: Avvia un servizio.
- `systemctl restart nomeServizio`: Riavvia un servizio.
ƒ