Wazuh Custom rules and decoders
To add to wazuh-manager:
``` 
git clone https://github.com/re-toor/Wazuh-Custom-rules-and-decoders.git && cd Wazuh-Custom-rules-and-decoders
```
Copy all custom decoders and rules to manager
```
cp decoders/* /var/ossec/etc/decoders/
```
```
chown wazuh:wazuh /var/ossec/etc/decoders/*
```
```
cp rules/* /var/ossec/etc/rules/
```
```
chown wazuh:wazuh /var/ossec/etc/rules/*
```
Restart Wazuh-manager to apply all change
```
restart wazuh-manager
```

Based on [Advanced Wazuh Detection Rules](https://github.com/socfortress/Wazuh-Rules)
