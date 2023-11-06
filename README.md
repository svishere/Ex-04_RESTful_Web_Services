# Ex-04_RESTful_Web_Services
## Aim:

To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation
## Procedure:

### Server side:
Step 1: Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.
Step 2: Right-click on the project name and select New->RESTful Web Services from Patterns.
![image](https://github.com/snoopydj911/Ex-04_RESTful_Web_Services/assets/122033587/78fc4e7c-9dc7-4b71-b246-3bf282e43691)





Step 3: A new window will appear. Select “Simple Root Resource” and click Next.
![image](https://github.com/snoopydj911/Ex-04_RESTful_Web_Services/assets/122033587/fbf6169b-fd4f-4fac-a243-5b8c833e87cc)

 
 


Step 4: In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.
![image](https://github.com/snoopydj911/Ex-04_RESTful_Web_Services/assets/122033587/80f4ebde-d937-453e-8a68-ccf8b5564ed8)



Step 5: Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.
Step 6: Alter getHtml() method as shown below.
Step 7: Save your project, clean and build it. Deploy your project.
![image](https://github.com/snoopydj911/Ex-04_RESTful_Web_Services/assets/122033587/9229ae26-28b9-41a2-aa28-6168ec15f9cd)

 

 


Step 8: To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).



Client-Side:


Step 1: Create a new Java Web Project. Follow steps 1-5 as in section 1.1.
Step 2: Right-click on the project and select New->RESTful Java Client.
![image](https://github.com/snoopydj911/Ex-04_RESTful_Web_Services/assets/122033587/0f3d1ef1-22e7-41fc-a18b-130bbcbc5316)




Step 3: A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse. Step 4: Carefully select your RESTful resource (web service) and click OK.
![image](https://github.com/snoopydj911/Ex-04_RESTful_Web_Services/assets/122033587/3f41f4ea-08b8-474e-a75b-05ad772eb7be)

 
 


Step 5: Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.
![image](https://github.com/snoopydj911/Ex-04_RESTful_Web_Services/assets/122033587/b3b04b85-3720-486b-919a-c0ba14ce18d9)



Step 6: An editing tab will open. Alter getHtml() method with the following.

![image](https://github.com/snoopydj911/Ex-04_RESTful_Web_Services/assets/122033587/b008e315-9f03-41ab-b78a-2b538455bb1d)

 


Step 7: Right-click on the Libraries folder under your project and select “Add JAR/Folder”.
![image](https://github.com/snoopydj911/Ex-04_RESTful_Web_Services/assets/122033587/d3295ed2-9082-4aca-ba17-ffdfb6e9e69c)



Step 8: A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.
![image](https://github.com/snoopydj911/Ex-04_RESTful_Web_Services/assets/122033587/4de50618-77a0-4ce7-8d9c-258c426c483e)

 
 


Step 9: Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.
Step 10: A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.
![image](https://github.com/snoopydj911/Ex-04_RESTful_Web_Services/assets/122033587/5b3c7d23-a691-4eb3-a32c-0a439cb81a39)


Step 11: Save the project and build it.
Step 12: Run the JSP file and you should see the output in a new browser window.
 
 ![image](https://github.com/snoopydj911/Ex-04_RESTful_Web_Services/assets/122033587/e64b6ca8-ca1f-46c4-a658-8e2cf9d8fb48)



Client-Side Remote Invocation:


Step 1: Follow steps 1-5 as in Section 2.2
Step 2: In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";
Step 3: Follow steps 6-12 as in Section 2.2


## Result:
 Thus, the RESTful web service program has been successfully created and executed.
