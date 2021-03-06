---
title: "&lt;transport&gt; of &lt;netPeerTcpBinding&gt;"
ms.date: "03/30/2017"
ms.assetid: c44d86d2-1160-44d7-9c7a-297b12eccc7f
---
# &lt;transport&gt; of &lt;netPeerTcpBinding&gt;
Specifies settings for transport level security when using the [\<netPeerTcpBinding>](../../../../../docs/framework/configure-apps/file-schema/wcf/netpeertcpbinding.md).  
  
 \<system.ServiceModel>  
\<bindings>  
\<netPeerTcpBinding>  
\<binding>  
\<security>  
\<transport>  
  
## Syntax  
  
```xml  
<netPeerTcpBinding>
  <binding>
    <security>
      <transport credentialType="Certificate/Password" />
    </security>
  </binding>
</netPeerTcpBinding>
```  
  
## Attributes and Elements  
 The following sections describe attributes, child elements, and parent elements  
  
### Attributes  
  
|Attribute|Description|  
|---------------|-----------------|  
|credentialType|Optional. Specifies the type of credentials used to verify messages sent with the peer transport. This attribute is of type <xref:System.ServiceModel.PeerTransportCredentialType>.|  
  
## credentialType Attribute  
  
|Value|Description|  
|-----------|-----------------|  
|Certificate|Authentication of the peer channel transport requires an X509 certificate.|  
|Password|Authentication of the peer channel transport requires a correct password.|  
  
### Child Elements  
 None  
  
### Parent Elements  
  
|Element|Description|  
|-------------|-----------------|  
|[\<security>](../../../../../docs/framework/configure-apps/file-schema/wcf/security-of-netpeerbinding.md)|Defines the security settings for the [\<netPeerTcpBinding>](../../../../../docs/framework/configure-apps/file-schema/wcf/netpeertcpbinding.md).|  
  
## See also
- <xref:System.ServiceModel.Configuration.PeerTransportSecurityElement>
- <xref:System.ServiceModel.PeerSecuritySettings.Transport%2A>
- <xref:System.ServiceModel.Configuration.PeerSecurityElement.Transport%2A>
- <xref:System.ServiceModel.PeerTransportSecuritySettings>
- [Securing Services and Clients](../../../../../docs/framework/wcf/feature-details/securing-services-and-clients.md)
- [Bindings](../../../../../docs/framework/wcf/bindings.md)
- [Configuring System-Provided Bindings](../../../../../docs/framework/wcf/feature-details/configuring-system-provided-bindings.md)
- [Using Bindings to Configure Services and Clients](../../../../../docs/framework/wcf/using-bindings-to-configure-services-and-clients.md)
- [\<binding>](../../../../../docs/framework/misc/binding.md)
