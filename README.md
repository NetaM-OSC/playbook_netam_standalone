# README

## TODO

### Global

- Update variables coherence between roles
- Update roles to could be deployed on Debian hosts
- Update firewalls configuration to configure with hosts IP to restrict opening
- Add role for nginx deployment

### NetAM-DB

- Move DB creation into NetAM-Core role
- Rework configurations to work with variables from group/host/inv variables to get full coherence with all roles
- Remove all tasks dedicated for NetAM-Core

### NetAM-Core

- Add configuration management in role
- Add nginx configuration
- Perform DB migration for install / update tags
- Add tags in role
  - Install
  - Configure
  - Update

### NetAM-Worker

- Do all tasks
