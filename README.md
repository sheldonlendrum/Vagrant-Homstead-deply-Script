# Vagrant-Homstead-deply-Script

This is a simple script that uses shuttle (or called manually) to reply a new Vagrant/Homestead local dev site. 

## Shuttle
Download the Shuttle app: https://fitztrev.github.io/shuttle/
![alt text](https://fitztrev.github.io/shuttle/images/how-shuttle-works.gif "Shuttle Preview")

## Shuttle Config. 
```javascript
{
	"editor": "default",
	"launch_at_login": true,
	"terminal": "Terminal.app",
	"iTerm_version": "nightly",
	"default_theme": "Basic",
	"open_in": "tab",
	"show_ssh_config_hosts": true,
	"ssh_config_ignore_hosts": [  ],
	"ssh_config_ignore_keywords": [  ],
	"hosts": [{
		"Vagrant": [{
			"name": "Start Vagrant",
			"cmd": "cd ~/Homestead; vagrant up"
		},{
			"name": "Stop Vagrant",
			"cmd": "cd ~/Homestead; vagrant halt"
		},{
			"name": "Provision New Site",
			"cmd": "cd ~/Scripts; sudo ./provision_site.sh"
		}]
	}]
}
```
