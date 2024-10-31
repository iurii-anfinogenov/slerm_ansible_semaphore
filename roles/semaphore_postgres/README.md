Role Name
A brief description of the role goes here.

Requirements an installed Postgresql, though note that this role requires root access:

```yaml
  hosts: servers
  become: true
  roles:
    - role: semaphore_postgres
```      
Role Variables
Defaults are provided but can be overridden:

```yaml
    semaphore_version: "latest"
    db_name: "semaphoredb"
    db_user: "semaphore"
    db_passwd: "semaphorepass"
    semaphore_config_path: "/etc/semaphore/config.json"
    semaphore_service_path: "/etc/systemd/system/semaphore.service"
   ```
Dependencies
An installed PostgreSQL instance with databases and users created (configured in variables).
