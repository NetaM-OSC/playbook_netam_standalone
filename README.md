#  playbook_netam_standalone


## Tags:

* `install` - Tag to use on first netam installation

## Variables:

### Netam_postgresql:
* `d_netam_db_backup_base_dir`: `'/usr/local/exploit'` - Netam database backup path
### Netam_redis:
* `d_redis_version`: `6.0.9` - Redis version to install
* `d_redis_package`: `redis-{{ d_redis_version }}.tar.gz` - Redis artifact name
* `d_redis_url`: `https://download.redis.io/releases/{{ d_redis_package }}` - Redis download URL
### Netam_core:
* `d_ruby_version`: `'2.7.2'` - Ruby version to use for netam environment
* `d_node_version`: `'14.15.4'` - Node version to user for netam environment
* `d_node_artifact`: `'node-v{{ d_node_version }}-linux-x64'` - Node artifact name
## TODO:

#### Improvement:
* Update variables coherence between roles -  (Playbook)
* Update roles to could be deployed on Debian hosts -  (Playbook)
* Update firewalls configuration to configure with hosts IP to restrict opening -  (Playbook)
* Rework configurations to work with variables from group/host/inv variables to get full coherence with all roles -  (netam_postgresql)
* Remove all tasks dedicated for NetAM-Core -  (netam_postgresql)
#### Feature:
* Add role for nginx deployment -  (Playbook)
* Move DB creation into NetAM-Core role -  (netam_postgresql)
* Add configuration management in role -  (netam_core)
* Add nginx configuration -  (netam_core)
* Perform DB migration for install / update tags -  (netam_core)
* Add tags in role (install, configure, update) -  (netam_core)
* Write all role -  (netam_worker)


Documentation generated using: [Ansible-autodoc](https://github.com/AndresBott/ansible-autodoc)

