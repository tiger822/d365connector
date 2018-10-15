# d365connector
Dynamics 365 webservice connector
A single spring webservice for access Dynamics 365 webservice.


run d365connector configuration file:
java.exe -jar d365tunnel-0.0.1-SNAPSHOT.jar --spring.config.location=classpath:/application.properties,d:/temp/application-live1.properties --spring.profiles.active=live1


wait for a comment , d365connector service is ready, last message on console is :
D365 endpoint:https://usnconeboxax1aos.cloud.onebox.dynamics.com
Current company:****
Access method:soap
Use proxy:******
Server port is listened:8081


as my example:
    dynamics 365 webservice is ready:
    https://usnconeboxax1aos.cloud.onebox.dynamics.com/api/services/AEL_RNote/AEL_RNote_Service/
    This XML file does not appear to have any style information associated with it. The document tree is shown below.
<ServiceGetResponse xmlns:i="http://www.w3.org/2001/XMLSchema-instance" xmlns="http://schemas.datacontract.org/2004/07/Microsoft.Dynamics.Platform.Integration.Services.Xpp">
<Operations>
<Name>getVendTable</Name>
</Operations>
</ServiceGetResponse>

   I can call getVendTable service by chrome browser:
   http://192.168.1.2:8081/soapcall/AEL_RNote/AEL_RNote_Service/getVendTable
   
