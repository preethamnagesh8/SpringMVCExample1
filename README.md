This example shows how to initialize a simple spring MVC based web application. The project has been initialized with a Maven project and imported spring dependencies. The project uses annotation based configurations and eliminates usage of an XML based deployment descriptor i.e web.xml to define servlet mappings.


**WEB.XML Based Archiecture**

A call to any controller, is checked first at the web.xml level to identify the servlet to refer to.
```Ex - A call to http://localhost:8080/SpringMVC1/add - a call to add controller to add 2 numbers.```

Here, the web.xml file is first checked to understand the servlet to refer to for the add controller. Then the corresponding XML configuration of the add-servlet is checked to get the package containing the definition of the controller. The request is then processed by the corresponding function and a web page is built dynamically to be returned.
