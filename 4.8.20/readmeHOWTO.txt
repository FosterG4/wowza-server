1) block your host 
Windows "C:\Windows\System32\drivers\etc\hosts"
Linux    /etc/hosts

127.0.0.1   wowzamedia.com
127.0.0.1   wowzalicense1.wowzamedia.com
127.0.0.1   wowzalicense2.wowzamedia.com
127.0.0.1   wowzalicense3.wowzamedia.com
127.0.0.1   wowzalicense4.wowzamedia.com
127.0.0.1   wowzalicense5.wowzamedia.com
127.0.0.1   wowza.netmasters.nl
127.0.0.1   www.towza.com
127.0.0.1   www.towza.tom

1.1) block in your firewall
129.153.100.158
129.153.114.13
129.154.207.194
132.145.253.238
138.3.255.30
141.147.1.186
146.56.156.1
158.101.43.210
193.123.241.42

2) install Windows
Just open WowzaStreamingEngine-4.8.20+1-windows-installer.exe and see Wizard

2) install Linux
chmod +x ./WowzaStreamingEngine-4.8.20+1-linux-x64-installer.run
./WowzaStreamingEngine-4.8.20+1-linux-x64-installer.run

Enter license ( ET1A4-KxrGd-Eaj9T-dTbcf-rZNza-9xaJd )  Linux and Windows

4)Replace wms-server.jar under '/usr/local/WowzaStreamingEngine-4.8.20+1/lib' for Linux
'Wowza Media Systems\Wowza Streaming Engine 4.8.20+1\lib' for Windows

5) restart wowza

service WowzaStreamingEngine restart
service WowzaStreamingEngineManager restart
or
/etc/init.d/WowzaStreamingEngine restart
/etc/init.d/WowzaStreamingEngineManager


6) If you want disable check updates version and check version java on wowza.com replace 2 of folder disable update watch and place to ->

For Windows:Wowza Media Systems\Wowza Streaming Engine 4.8.20+1\manager\temp\webapps\enginemanager\WEB-INF\classes\org\apache\jsp\tag\web\wmsform

For Linux: WowzaStreamingEngine/manager/temp/webapps/enginemanager/WEB-INF/classes/org/apache/jsp/tag/web/wmsform

7) restart wowza again

ENJOY........