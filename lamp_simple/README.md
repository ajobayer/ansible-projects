Building a simple LAMP stack and deploying Application using Ansible Playbooks.
-------------------------------------------------------------------------------
These playbooks are meant to be a reference and starter's guide to building
Ansible Playbooks. These playbooks were tested on CentOS 6.x so we recommend
that you use CentOS or RHEL to test these modules.

This LAMP stack can be on a single node or multiple nodes. The inventory file
'hosts' defines the nodes in which the stacks should be configured.

	[webservers]
	192.168.1.1

	[dbservers]
	192.168.1.2

Here the webserver would be configured on the 192.168.1.1 and the dbserver on a
server called "192.168.1.2". The stack can be deployed using the following
command:

        ansible-playbook -i hosts site.yml

Once done, you can check the results by browsing to http://192.168.1.1/index.php.
You should see a simple test page and a list of databases retrieved from the
database server.

	├── group_vars
	│   ├── all
	│   └── dbservers
	├── hosts
	├── README.md
	├── roles
	│   ├── common
	│   │   ├── handlers
	│   │   │   └── main.yml
	│   │   ├── tasks
	│   │   │   └── main.yml
	│   │   └── templates
	│   │       └── ntp.conf.j2
	│   ├── db
	│   │   ├── handlers
	│   │   │   └── main.yml
	│   │   ├── tasks
	│   │   │   └── main.yml
	│   │   └── templates
	│   │       └── my.cnf.j2
	│   └── web
	│       ├── handlers
	│       │   └── main.yml
	│       ├── tasks
	│       │   ├── copy_code.yml
	│       │   ├── install_httpd.yml
	│       │   └── main.yml
	│       └── templates
	│           └── index.php.j2
	└── site.yml
