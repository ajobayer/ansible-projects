_simple-web-db-lb-template_
 **Web APP Database server provisioning with Ansible palybook template**


		├── ansible.cfg
		├── control.yml
		├── demo
		│   ├── app
		│   │   ├── demo.py
		│   │   ├── demo.wsgi
		│   │   └── requirements.txt
		│   └── demo.conf
		├── dev
		├── loadbalancer.yml
		├── webserver.yml
		├── database.yml
		├── playbooks
		│   ├── hostname.yml
		│   ├── stack_restart.yml
		│   └── stack_status.yml
		├── roles
		│   ├── apache2
		│   │   ├── defaults
		│   │   │   └── main.yml
		│   │   ├── handlers
		│   │   │   └── main.yml
		│   │   ├── meta
		│   │   │   └── main.yml
		│   │   ├── README.md
		│   │   ├── tasks
		│   │   │   └── main.yml
		│   │   └── vars
		│   │       └── main.yml
		│   ├── control
		│   │   ├── defaults
		│   │   │   └── main.yml
		│   │   ├── handlers
		│   │   │   └── main.yml
		│   │   ├── meta
		│   │   │   └── main.yml
		│   │   ├── README.md
		│   │   ├── tasks
		│   │   │   └── main.yml
		│   │   └── vars
		│   │       └── main.yml
		│   ├── demo_app
		│   │   ├── defaults
		│   │   │   └── main.yml
		│   │   ├── handlers
		│   │   │   └── main.yml
		│   │   ├── meta
		│   │   │   └── main.yml
		│   │   ├── README.md
		│   │   ├── tasks
		│   │   │   └── main.yml
		│   │   └── vars
		│   │       └── main.yml
		│   ├── mysql
		│   │   ├── defaults
		│   │   │   └── main.yml
		│   │   ├── handlers
		│   │   │   └── main.yml
		│   │   ├── meta
		│   │   │   └── main.yml
		│   │   ├── README.md
		│   │   ├── tasks
		│   │   │   └── main.yml
		│   │   └── vars
		│   │       └── main.yml
		│   └── nginx
		│       ├── defaults
		│       │   └── main.yml
		│       ├── handlers
		│       │   └── main.yml
		│       ├── meta
		│       │   └── main.yml
		│       ├── README.md
		│       ├── tasks
		│       │   └── main.yml
		│       └── vars
		│           └── main.yml
		├── templates
		│   └── nginx.conf.j2
		



