# DevSecOps-Toolkit-Docker-Container
## Docker container to use with CICD pipelines without the need to install all the bins and dependencies.

### It comprises the following:

> Check Point ShiftLeft Command Framework for DevSecOps

> AWS cli

> Terraform cli

> Ansible cli

> Check Point SourceGuard Static Code Analysis Scanner

> Check point CloudGuard Serverless Security Runtime Security cli.


## The container is available on docker hub:
> docker pull dhouari/devsecops:latest

```

$docker run -it dhouari/devsecops
   __________     ____            _____           ____            
  / ____/ __ \   / __ \___ _   __/ ___/___  _____/ __ \____  _____
 / /   / /_/ /  / / / / _ \ | / /\__ \/ _ \/ ___/ / / / __ \/ ___/
/ /___/ ____/  / /_/ /  __/ |/ /___/ /  __/ /__/ /_/ / /_/ (__  ) 
\____/_/      /_____/\___/|___//____/\___/\___/\____/ .___/____/  
                                                   /_/            
>This is the Check Point DevSecOps Toolkit.
 It includes the Shiftleft CLI Framework, Ansible, Terraform and the AWS cli

shiftleft
===========
DESCRIPTION
	Check Point ShiftLeft CLI framework

SYNOPSIS
	shiftleft [options] <blade> [parameters]

OPTIONS

  -D, --debug                  debug output flag
  -d, --directory string       work dir (default is temp dir)
  -f, --force-version string   use blade specific version
  -h, --help                   show usgae
  -t, --timeout int            timeout (default 600)
  -u, --update                 auto upgrade/update (default true)
  -V, --version                show version

EXAMPLE
	shiftleft -t 30 sourceguard -h

AVAILABLE BLADES:
 1  cloudguard   cloudguard Function Self Protection - FSP , Detects & stops application attacks, such as SQL injection and oth 
                 ers.                                                                                                           
 2  sourceguard  source-code security and visibility into the risk analysis of projects                                         

CloudGuard
----------
Usage: cloudguard [options] [command]

Options:
  -V, --version           output the version number
  -h, --help              output usage information

Commands:
  fsp [options] [action]  FSP protection can be added or removed using actions
  
  Action:
   add (default)
   remove
------------------------------------------------------------------------------------------
SourceGuard
----------
Usage of sourceguard-cli:
  -V	print version
  -d	debug output flag
  -img string
    	path to docker image tar format
  -j	json output flag
  -src string
    	path to source code directory
  -t int
    	timeout (default 600)
  -x value
    	exclusions: path to exclude from scanning .gitignore syntaxAnsible
==========================================================================================
ANSIBLE
-------
All the Check Point Ansible playbooks are located in the cpAnsible directory.
Please enter the ansible cli at the prompt or with docker run command

==========================================================================================
TERRAFORM
---------
All the Check Point Terraform modules for AWS and Azure are located under the cpTerraform directory
Please enter the terraform cli at the prompt or with the docker run command

============================================================================================
awscli 
------
Please use the aws configure command to configure your credentials and region when starting the container.
You can verify your setting using the aws configure list command.


# 

```

