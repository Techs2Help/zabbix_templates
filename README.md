# Custom Zabbix Templates
Different custom created Zabbix Templates
__The templates are only a Proof of Concept and they still need to work, be free to make a commit so that together we can help other people to monitor their services with Zabbix__

Templates:
- Cardano Node Monitoring:<br>
--> uses Prometheus node export statistics to monitor a Cardano Block producer or Relay (P2P ready)
--> uses ${HOST_IP} Macro to retrieve data from Prometheus

- Cardano Pool Monitoring: <br>
--> uses Cexplorer static APIs to retrive data
--> the template can be added to any host with Internet access
--> uses {$POOL_ID_MNT} macro to set pool_id (basically any pool listed in Cexplorer can be monitored)
--> uses {$NETWORK_MNT} macro to set the link of the API to use:<br>
1. Mainnet set: "js.cexplorer.io"<br>
2. Preprod set: "preprod-js.cexplorer.io"<br>
3. Preview set: "preview-js.cexplorer.io"<br>

