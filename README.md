# Snippet to configure usage of external decryption in Shibboleth IDPv4

## Datasource definition

The [data source definiton](attribute-resolver.xml) to include /opt/shibboleth-idp/conf/attribute-resolver.xml

The [bean definition](attribute-resolver-beans.xml) /opt/shibboleth-idp/conf/attribute-resolver-beans.xml

The bean is configured in: /opt/shibboleth-idp/conf/services.xml:

```
    <util:list id ="shibboleth.AttributeResolverResources">
         <value>%{idp.home}/conf/attribute-resolver.xml</value>
         <value>%{idp.home}/conf/attribute-resolver-beans.xml</value>
    </util:list>
```



