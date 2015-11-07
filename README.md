# JAXRS-HelloWorld
Jetty Maven Jersey Eclipse Sample project

Original project samples from 

http://examples.javacodegeeks.com/enterprise-java/rest/jersey/jersey-hello-world-example/

https://jersey.java.net/documentation/latest/deployment.html

4.7.1.2. Jersey package scanning

If there is no configuration properties to be set and deployed application consists only from resources and providers stored in particular packages, you can instruct Jersey to scan these packages and register any found resources and providers automatically:

Example 4.12. Configuring Jersey container Servlet or Filter to use package scanning

<init-param>
    <param-name>jersey.config.server.provider.packages</param-name>
    <param-value>
        org.foo.myresources,org.bar.otherresources
    </param-value>
</init-param>
<init-param>
    <param-name>jersey.config.server.provider.scanning.recursive</param-name>
    <param-value>false</param-value>
</init-param>

Jersey will automatically discover the resources and providers in the selected packages. You can also decide whether Jersey should recursively scan also sub-packages by setting the jersey.config.server.provider.scanning.recursive property. The default value is true, i.e. the recursive scanning of sub-packages is enabled. 

