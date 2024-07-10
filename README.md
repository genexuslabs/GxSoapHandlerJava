# GxSoapHandler

## Spanish
Se consume un servicio Soap desde un environment GeneXus, con la propiedad Use Native Soap prendida.

Se provee un mecanismo para poder agregar datos en dicho request SOAP, por ejemplo enviar un token SAM-L para la autenticación.

Es un mecanismo que permite hacer algo similar al tipo de datos location, pero extendiendo sus funcionalidades, sin la necesidad de cargar a este tipo de datos con particularidades del lenguage. 

Esto se implementa a través de un jar externo. Si existe en el classpath una clase llamada com.genexus.util.GXSoapHandler se va a invocar a un método static de esa clase llamado setHandlers antes de la llamada al servicio.
 
Ese método tiene los parámetros especificados en este proyecto, algo como:
```
public static void setHandlers(Integer remoteHandle, com.genexus.ModelContext context, String serviceName, javax.xml.ws.BindingProvider bProvider)
```
 
## English
A Soap service is consumed from an GeneXus environment with the Use Native Soap property set true. 

A mechanism is provided to add data to this SOAP request, for example sending a SAM-L token for authentication. 

It is a mechanism that allows you to do something similar to the location data type, but extending its functionalities, without the need to load this type of data with language particularities.

This is implemented through an external jar. If a class called com.genexus.util.GXSoapHandler exists in the classpath, a static method of that class called setHandlers will be invoked before the call to the service.

That method has the parameters specified in this project, something like this: 
```
public static void setHandlers(Integer remoteHandle, com.genexus.ModelContext context, String serviceName, javax.xml.ws.BindingProvider bProvider)
```
