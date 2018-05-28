# GxSoapHandlerJava

Se consume un servicio Soap desde un environment con la propiedad Use Native Soap prendida. 
Se provee un mecanismo para poder agregar datos en dicho request SOAP, por ejemplo enviar un token SAM-L para la autenticación.
Es un mecanismo que permite hacer algo similar al tipo de datos location, pero extendiendo sus funcionalidades, 
sin la necesidad de cargar a este tipo de datos con particularidades del lenguage. 

Esto se implementa a traves de un jar externo. Si existe en el classpath una clase llamada com.genexus.util.GXSoapHandler 
se va a invocar a un método static de esa clase llamado setHandlers antes de la llamada al servicio.
 
Ese método tiene los parametros especificados en este proyecto, algo como:
public static void setHandlers(Integer remoteHandle, com.genexus.ModelContext context, String serviceName, javax.xml.ws.BindingProvider bProvider)
 
