# DevSec Linux Hardening Playbook

Ansible playbook for hardening a Linux host(s) to comply with these DevSec baselines:

- [Linux baseline](https://github.com/dev-sec/linux-baseline)
- [SSH baseline](https://github.com/dev-sec/ssh-baseline)

## Run

```shell
# Modify inventory with host address and user. Esure you have already setup SSH
# access on your target host.
nano inventory.yaml

# Install the required Ansible collection.
ansible-galaxy collection install devsec.hardening

# Run the playbook.
ansible-playbook -i inventory.yaml playbook.yaml --ask-become-pass
```

## License

See [LICENSE](LICENSE) for details.