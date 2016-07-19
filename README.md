# Plus UI

## What's needed

The User Interface needs to be more modular so the following changes are needed:

* CSS Frameworks should be moved out of app.css
* Main segments of code should be style independent(no classes on header/section)
* CSS Comments
* Navigation menus should be evident by use of navbar class on the menu itself


## Requirements

Make sure all dependencies have been installed before moving on:

* [Ansible](http://docs.ansible.com/ansible/intro_installation.html#latest-releases-via-pip) 2.0.2
* [Virtualbox](https://www.virtualbox.org/wiki/Downloads) >= 4.3.10
* [Vagrant](https://releases.hashicorp.com/vagrant/1.8.1/) 1.8.1
* [vagrant-bindfs](https://github.com/gael-ian/vagrant-bindfs#installation) >= 0.3.1 (Windows users may skip this)
* [vagrant-hostmanager](https://github.com/smdahlen/vagrant-hostmanager#installation)

## Dev Setup

The recommended directory structure for Plus UI looks like:

```shell
site/      # → Root folder for the project
├── fonts/      # → Main fonts directory
└── css/         # → Main Css directory
    ├── framework/  # → css framework directory (margin rules, icon rules etc.)
    └── dependencies/   # → Bower Folder (don't touch!)
    └── custom/   # → custom css directory
└── js/         # → A Bedrock-based WordPress site
    ├── framework/  # → js framework directory
    └── dependencies/   # → Bower Folder (don't touch!)
    └── custom/   # → custom js directory
└── images/
    ├── icons/  # → icon directory
    └── home/   # → images which need to be on home page - with descriptive name        
```

See a complete working example in the [plus-ui repo](https://github.com/2wce/plus-ui).

1. Create a new project directory: `$ mkdir site && cd site`
2. Clone plus-ui: `$ git clone --depth=1 https://github.com/2wce/plus-ui.git && rm -rf plus-ui/.git`

Windows user? [Read the Windows docs](#) for slightly different instructions.
