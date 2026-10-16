# aap-poc-net-automation

Playbooks **simulados e inofensivos** para una PoC de gobernanza RBAC en
Red Hat Ansible Automation Platform 2.7.

- No se conectan a dispositivos de red reales: los hosts del inventario usan
  `ansible_connection: local` y solo existen como nombres simulados.
- `assign_ip_simulation.yml` **no** contacta ningún IPAM; solo calcula y muestra
  una IP ficticia.
- Este repositorio no contiene secretos.

| Playbook | Propósito |
|---|---|
| `check_connectivity.yml` | Simula una prueba de alcance (ping local) |
| `backup_config.yml` | Genera un respaldo de configuración ficticio dentro del contenedor de ejecución |
| `assign_ip_simulation.yml` | Simula la asignación de una IP desde un pool |

Versionado: `main` = desarrollo; tags `prod-vX.Y.Z` = versiones aprobadas para producción.
