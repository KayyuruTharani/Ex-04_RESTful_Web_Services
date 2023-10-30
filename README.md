# Ex-04_RESTful_Web_Services
## Aim:

To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation
## Procedure:

### Server side:
Step 1: Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.
Step 2: Right-click on the project name and select New->RESTful Web Services from Patterns.






<img width="426" alt="image" src="https://github.com/KayyuruTharani/Ex-04_RESTful_Web_Services/assets/142209319/05d4476b-7e2e-4ed8-b0bd-a4bed35a6959">








Step 3: A new window will appear. Select “Simple Root Resource” and click Next.





<img width="357" alt="image" src="https://github.com/KayyuruTharani/Ex-04_RESTful_Web_Services/assets/142209319/6f25213b-5b4c-4e2e-8b40-c301ba28f5c3">





 
 


Step 4: In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.






<img width="388" alt="image" src="https://github.com/KayyuruTharani/Ex-04_RESTful_Web_Services/assets/142209319/eeff89ae-fa48-46bb-85c5-524d49f96417">






Step 5: Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.
Step 6: Alter getHtml() method as shown below.
Step 7: Save your project, clean and build it. Deploy your project.
 



<img width="420" alt="image" src="https://github.com/KayyuruTharani/Ex-04_RESTful_Web_Services/assets/142209319/2c3c75c1-883b-4675-8b1e-a7b4aa4a6502">








Step 8: To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).



Client-Side:


Step 1: Create a new Java Web Project. Follow steps 1-5 as in section 1.1.
Step 2: Right-click on the project and select New->RESTful Java Client.





<img width="455" alt="image" src="https://github.com/KayyuruTharani/Ex-04_RESTful_Web_Services/assets/142209319/38731476-5eea-4ec5-b6bb-dd0b98baeca5">







Step 3: A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse. 
Step 4: Carefully select your RESTful resource (web service) and click OK.







<img width="417" alt="image" src="https://github.com/KayyuruTharani/Ex-04_RESTful_Web_Services/assets/142209319/3ef1d157-d199-489f-b857-201486b66ea8">






 
 


Step 5: Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.








<img width="429" alt="image" src="https://github.com/KayyuruTharani/Ex-04_RESTful_Web_Services/assets/142209319/dd4bf175-6268-4d5e-b849-d2e377363f88">





Step 6: An editing tab will open. Alter getHtml() method with the following.
 




<img width="410" alt="image" src="https://github.com/KayyuruTharani/Ex-04_RESTful_Web_Services/assets/142209319/0948f7c3-da0f-4e0b-ade4-facc3bc7c029">





 


Step 7: Right-click on the Libraries folder under your project and select “Add JAR/Folder”.




<img width="226" alt="image" src="https://github.com/KayyuruTharani/Ex-04_RESTful_Web_Services/assets/142209319/3527b705-c5d1-4c74-a695-455286da2a13">







Step 8: A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.
 




<img width="433" alt="image" src="https://github.com/KayyuruTharani/Ex-04_RESTful_Web_Services/assets/142209319/62a48c1b-6f40-4d29-a0f8-852eded61c3f">





 


Step 9: Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.
Step 10: A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.






<img width="444" alt="image" src="https://github.com/KayyuruTharani/Ex-04_RESTful_Web_Services/assets/142209319/58071346-09fb-4c8c-a29a-f6cb55d64da5">







Step 11: Save the project and build it.
Step 12: Run the JSP file and you should see the output in a new browser window.
 
 


<img width="381" alt="image" src="https://github.com/KayyuruTharani/Ex-04_RESTful_Web_Services/assets/142209319/1ca0d2d2-64ba-4ed9-8b19-eefd7430721a">




Client-Side Remote Invocation:


Step 1: Follow steps 1-5 as in Section 2.2
Step 2: In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";
Step 3: Follow steps 6-12 as in Section 2.2


## Result:
 Thus, the RESTful web service program has been successfully created and executed.
