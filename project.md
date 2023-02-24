# ANSIBLE DYNAMIC ASSIGNMENTS (INCLUDE) AND COMMUNITY ROLES

## Introducing Dynamic Assignment Into Our structure
In your https://github.com/<your-name>/ansible-config-mgt GitHub repository start a new branch and call it dynamic-assignments

![Git-branch](./images/dynamic-assignments.PNG)

## Create a new folder, name it dynamic-assignments. Then inside this folder, create a new file and name it env-vars.yml. We will instruct site.yml to include this playbook later

![Dynamic-env-yml](./images/dy-ass-env.PNG)

## create a folder to keep each environment’s variables file. Therefore, create a new folder env-vars, then for each environment.

![Env-vars-yml](./images/env-vars.PNG)

## Now paste the instruction below into the env-vars.yml file

![dynamic-envyml-file](./images/dy-envs-varyml.PNG)

## Update site.yml file to make use of the dynamic assignment

## Download Mysql Ansible Role, Apache and Nginx by Geerlingguy In roles directory

![Downloaded-roles](./images/Downloaded-roles.PNG)

## Configure the Apache and Nginx roles to suit our usage

![Apache-de-main](./images/apa-de-mai-config.PNG)

![Apache-main](./images/apac-config1.PNG)

![Apache](./images/apac-rehat-setup.PNG)

![Nginx-main](./images/loop-nginx.PNG)

![Nginx](./images/ngin-http-opt.PNG)

![Nginx-config](./images/nginx-load.PNG)

![Nginx-2](./images/nginx-upstreams.PNG)

## Since you cannot use both Nginx and Apache load balancer, you need to add a condition to enable either one

![Nginx-define](./images/nginx-load.PNG)

![Apache-2](./images/apa-de-mai-config.PNG)
## Create loadbalancers yml file, db yml file and update site yml file in playbook

![Lb-yml](./images/lb-ymlf.PNG)

![Db-yml](./images/db-files.PNG)

![webserver](./images/webs-static.PNG)

![site-yml](./images/site-yml.PNG)

![site-yml](./images/site-yml2.PNG)

## Now you can make use of env-vars\uat.yml file to define which loadbalancer to use in UAT environment by setting respective environmental variable to true

![define-uat-envfile](./images/env-uat-yml.PNG)

# Run ansible playbook

![Ansible-playbook](./images/ansible-playbook.PNG)
