# Docker based images for dbsmartbackup

- Docker integration for [dbsmartbackup](https://github.com/kiorky/db_smart_backup)

## Support development
- Ethereum: ``0xa287d95530ba6dcb6cd59ee7f571c7ebd532814e``
- Bitcoin: ``3GH1S8j68gBceTeEG5r8EJovS3BdUBP2jR``
- [paypal](https://paypal.me/kiorky)


## corpusops/dbsmartbackup
### Description
- This repo produces all those docker images except pg10, master, 1, 2 , 3.
    - [corpusops/dbsmartbackup](https://hub.docker.com/r/corpusops/dbsmartbackup/)
- Another [older repository](https://github.com/corpusops/setups.dbsmartbackup) produces all those docker images:
    - [corpusops/dbsmartbackup-legacy](https://hub.docker.com/r/corpusops/dbsmartbackup-legacy/)
    - but also the latest, 1, 3, 3 & pg10 tags [corpusops/dbsmartbackup](https://hub.docker.com/r/corpusops/dbsmartbackup/)

### Volumes
- a volume mapped to ``/srv/backups`` to store backups

### Configuring the app
- if NO_AUTO_PASSWORD is set, PGPASSWORD and PGUSER wont be set with the valmues of PGUSER or PASSWORD if set, see [rootfs/entry.sh](./rootfs/entry.sh)
- [docker-compose example usage](./docker-compose.sample.yml)
