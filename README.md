# Holberton — System Engineering & DevOps (Advanced)

Continuation of the Holberton School System Engineering & DevOps curriculum, focused on Linux internals, networking, web infrastructure, configuration management, and APIs. Picks up where the [shell-fundamentals repo](https://github.com/TeoVH/holberton-system_engineering-devops) left off.

## Modules

### Linux & Scripting

| Module | Topic |
|--------|-------|
| [0x05-processes_and_signals](./0x05-processes_and_signals) | Processes, signals (`kill`, `trap`), PIDs |
| [0x06-regular_expressions](./0x06-regular_expressions) | Regular expressions (Oniguruma in Ruby scripts) |

### Networking

| Module | Topic |
|--------|-------|
| [0x07-networking_basics](./0x07-networking_basics) | OSI model, IPv4/IPv6, TCP/UDP, ports |
| [0x08-networking_basics_2](./0x08-networking_basics_2) | `localhost`, `0.0.0.0`, hosts file, `netcat` |

### Web Infrastructure

| Module | Topic |
|--------|-------|
| [0x09-web_infrastructure_design](./0x09-web_infrastructure_design) | Designing simple-to-complex web stacks (load balancers, caching, redundancy) |
| [0x0C-web_server](./0x0C-web_server) | Nginx — virtual hosts, redirects, custom 404 |
| [0x0F-load_balancer](./0x0F-load_balancer) | HAProxy — round-robin load balancing |
| [0x10-https_ssl](./0x10-https_ssl) | TLS/SSL termination, HTTPS via HAProxy + Let's Encrypt |
| [0x13-firewall](./0x13-firewall) | `ufw` firewall configuration |

### Configuration Management & Remote Access

| Module | Topic |
|--------|-------|
| [0x0A-configuration_management](./0x0A-configuration_management) | Puppet — manifests, resources, idempotency |
| [0x0B-ssh](./0x0B-ssh) | SSH keys, configuration, authentication |

### Databases

| Module | Topic |
|--------|-------|
| [0x14-mysql](./0x14-mysql) | MySQL — backups, replication (primary/replica) |

### APIs

| Module | Topic |
|--------|-------|
| [0x15-api](./0x15-api) | Consuming REST APIs in Python (`requests`), exporting to JSON/CSV |

Each module folder contains the relevant scripts, manifests or configuration files for the tasks.

## Tech Stack

- **OS:** Ubuntu 14.04 / 20.04
- **Web:** Nginx, HAProxy
- **Config management:** Puppet
- **DB:** MySQL
- **Languages:** Bash, Ruby (regex tasks), Python (API tasks)
- **Tooling:** `ufw`, `netcat`, `dig`, `ssh`, `curl`

## Running the Scripts

Most tasks are Bash, Puppet manifests or Python scripts that target a specific Linux server configuration. Example:

```bash
git clone https://github.com/TeoVH/holbertonschool-system_engineering-devops.git
cd holbertonschool-system_engineering-devops/0x0C-web_server

# Run a Bash setup script (typically as root on a fresh Ubuntu host)
sudo ./<task-script>
```

For Puppet manifests:

```bash
sudo puppet apply <manifest>.pp
```

For Python API tasks:

```bash
cd 0x15-api
python3 <script>.py <args>
```

## Author

- **Mateo Villada** — [@TeoVH](https://github.com/TeoVH)

## Acknowledgments

Projects completed as part of the [Holberton School](https://www.holbertonschool.com/) System Engineering & DevOps curriculum.
