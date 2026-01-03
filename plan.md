homelab-ansible/
├── ansible.cfg
├── inventory                     # or inventory/ dir
│   └── home.ini
├── group_vars/
│   ├── all.yml
│   ├── photos.yml
│   └── git.yml
├── host_vars/
│   └── git.home.arpa.vault
├── site.yml                      # <-- single entry-point playbook
├── roles/
│   ├── docker/
│   │   ├── defaults
│   │   │   └── main.yml
│   │   ├── tasks
│   │   │   └── main.yml
│   │   └── handlers
│   │       └── main.yml
│   ├── nextcloud_compose/
│   │   ├── tasks
│   │   │   └── main.yml
│   │   ├── templates
│   │   │   └── docker-compose.yml.j2
│   │   └── defaults
│   │       └── main.yml
│   └── immich_compose/
│       └── …
└── playbooks/                    # optional extra playbooks
└── backup.yml