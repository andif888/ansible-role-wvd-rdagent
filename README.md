ansible-role-wvd-rdagent
=========

Installes Powershell Core 7 and Windows Virtual Desktop RDAgent, RDAgent Bootloader.   
The machine registers it self at the WVD host pool.

Requirements
------------

Remote Desktop Session Host Role needs to be pre-installed.

Role Variables
--------------

**wvd_rdagent_tenant_id** (required)  
Azure tenant id
```yaml
wvd_rdagent_tenant_id: abc12345-1234-5678-bbbb-15817fa15cca
``` 

**wvd_rdagent_subscription_id** (required)    
Azure subscription id
```yaml
wvd_rdagent_subscription_id: abd89889-1111-2222-3333-306117795364
``` 

**wvd_rdagent_client_id** (required)   
service principal app id
```yaml
wvd_rdagent_client_id: 12345678-abbc-1111-2222-fe4502393322
``` 

**wvd_rdagent_client_secret** (required)   
service principal client secret
```yaml
wvd_rdagent_client_secret: "79823472389432432324"
```

**wvd_rdagent_resource_group** (required)    
Azure resource group 
```yaml
wvd_rdagent_resource_group: my_resource_group
```

**wvd_rdagent_host_pool** (required)    
Azure WVD host pool  
```yaml
wvd_rdagent_host_pool: my_wvd_host_pool
```

References
--------------
https://docs.microsoft.com/en-us/azure/virtual-desktop/create-host-pools-powershell#register-the-virtual-machines-to-the-windows-virtual-desktop-host-pool   
https://github.com/Azure/RDS-Templates/tree/master/ARM-wvd-templates/DSC   
https://github.com/MicrosoftDocs/azure-docs/blob/master/articles/virtual-desktop/create-host-pools-powershell.md   