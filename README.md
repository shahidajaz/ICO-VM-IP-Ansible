# Provisioning web servers by using Cisco Intersight Cloud Orchestrator (ICO)

The automated process of creating a virtual machine, customising the hostname and & IP address, and utilising a configuration management application, Ansible, to install packages (in this case, NGINX) by using Cisco Intersight Cloud Orchestrator

## What is Cisco Intersight Cloud Orchestrator (ICO)?

Cisco Intersight Cloud Orchestrator provide a consistent, cloud-like experience across your hybrid IT environment by providing an easy-to-use workflow designer. 

With Cisco Intersight Cloud Orchestrator you can truly evolve your automation strategy to provide consistent experience across on-premises resources and public clouds.

<img width="1758" alt="image" src="https://user-images.githubusercontent.com/70768079/183657135-e1021a2c-f61a-4261-b480-7718d426ac8a.png">

## Cisco Intersight Cloud Orchestrator Workflow for Web Servers provisioning

There are four tasks used in this work flow
1. Create VM from a template
2. Guest Customization for a virtual machine (customize hostname and IP address)
3. Update hosts file for Ansible to install the NGINX web server by using SSH task built in ICO
4. Finally use Ansible to install the NGINX web servers and start the NGINX service

<img width="598" alt="image" src="https://user-images.githubusercontent.com/70768079/183659753-28f29202-8039-442f-ac6e-d07e51ed0f31.png">

## Fill the inputs into the workflow
<img width="1768" alt="image" src="https://user-images.githubusercontent.com/70768079/183887674-9a93d8b8-5471-41ca-a592-bd98c03b1e4c.png">

## Workflow Execution
<img width="1276" alt="image" src="https://user-images.githubusercontent.com/70768079/183888836-fbc342d2-a51a-4bb6-b963-4e5a674645a6.png">


## Check the VM in the vCenter

<img width="789" alt="image" src="https://user-images.githubusercontent.com/70768079/183888956-c5e28932-022c-4bb5-9813-8e5f65be5cd8.png">


# Rollback
ICO supports the functionality of rollbacks by reverting entities created or modified when executing a workflow. You can choose one or more tasks to revert back as shown in the figure below:

<img width="1530" alt="image" src="https://user-images.githubusercontent.com/70768079/183889375-b8ca5d4b-a1f4-485d-99e4-216016650857.png">

