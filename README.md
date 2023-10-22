# Ex-03-SOAP-based-Web-Services

## Aim:

To create and execute SOAP-based web service program using server, client and client- side remote invocation.

## Procedure:

### Server-side:
#### Step 1:
Open NetBeans IDE.
#### Step 2:
Click File->New Project. Choose Java Web and then Web Application and click Next.

![image](https://github.com/MaheshS03/Ex-03-SOAP-based-Web-Services/assets/128498431/2178fb11-13da-4f49-9127-6010620999e4)

#### Step 3:
Give your Project a suitable Name and then click Next.
#### Step 4:
In the next window, make sure you have selected Server as “GlassFish Server” and Java EE Version as “Java EE 7 Web”. Click Finish.

![image](https://github.com/MaheshS03/Ex-03-SOAP-based-Web-Services/assets/128498431/3c5cbac7-8c87-4fa0-bfbc-c436f7fee561)

#### Step 5:
Your new project will appear in the Projects tab in the left-most part of NetBeans.

#### Step 6:
Right click your Project and select New->Web-Service.

![image](https://github.com/MaheshS03/Ex-03-SOAP-based-Web-Services/assets/128498431/2f5c166d-8792-49a0-b92b-a157ec097ed6)

#### Step 7:
In the new window, give your web service a name and a package name. Click Finish.
 
![image](https://github.com/MaheshS03/Ex-03-SOAP-based-Web-Services/assets/128498431/ee9899f1-3d29-4b1c-9435-653b78b18da9)

#### Step 8:
A new coding tab will open that contains your web service.

#### Step 9:
Expand the folder “Web Services” under your project. You should see your newly created web service. Right-click on it and choose “Add Operation”.

![image](https://github.com/MaheshS03/Ex-03-SOAP-based-Web-Services/assets/128498431/5aea50ee-bd08-40a3-ae1b-dde58097c955)

#### Step 10:
A new window to add operation will appear. In that give Name, Return Type to your operation. Then click the Add button to add necessary arguments/parameters for that operation. (Since we are demonstrating simple addition, we use two arguments/parameters.) Once you are happy with your parameters/arguments, click OK.

![image](https://github.com/MaheshS03/Ex-03-SOAP-based-Web-Services/assets/128498431/1736f33c-a606-43a6-967b-385340a9639d)

#### Step 11:
NetBeans will automatically generate the skeleton for the operation which will be like,

![image](https://github.com/MaheshS03/Ex-03-SOAP-based-Web-Services/assets/128498431/f287b46f-5ba9-4ed6-9c95-310f4138b4c6)

#### Step 12:
Replace return 0.0 with return (a+b)

#### Step 13:
Save your project. Right-click on the project, select “Clean and Build”. Once the Building process is successful, again Right-click on the project, select “Deploy”. Deploying might take time depending on the size of the project. 

#### Step 14:
Once your project is successfully deployed, right-click on your web service name and select “Test Web Service”

![image](https://github.com/MaheshS03/Ex-03-SOAP-based-Web-Services/assets/128498431/ea32f20b-0790-46cf-806d-1f37c03b5cef)

#### Step 15:
A new browser window will appear which will look like this

![image](https://github.com/MaheshS03/Ex-03-SOAP-based-Web-Services/assets/128498431/c046d2bb-7275-44dc-8e6b-44fccd3f53a3)

#### Step 16: 
You can give inputs to your web service and check whether it is working properly or not. If it is working properly, you will get a page like this

![image](https://github.com/MaheshS03/Ex-03-SOAP-based-Web-Services/assets/128498431/79900111-5f3b-49e8-afce-358fcf162e91)

### Client-side:

#### Step 1:
Create a new Java Web Project in NetBeans. (Follow Steps 1-5 as in section 1.1)
#### Step 2:
Right-click on the project and select New->Web Service Client.

![image](https://github.com/MaheshS03/Ex-03-SOAP-based-Web-Services/assets/128498431/3dfa7285-af23-4960-b6e3-fa741c51967a)

#### Step 3: 
A new window will appear. Select “Project” under the heading “Specify the WSDL file of the Web Service.” and click Browse

#### Step 4: 
A new window will appear, in that carefully choose appropriate web service and click OK.

 ![image](https://github.com/MaheshS03/Ex-03-SOAP-based-Web-Services/assets/128498431/1187f25a-dace-416a-9575-31f73aefaf82)

#### Step 5:
The Project file will be filled with the location to the WSDL file of the web service. If you prefer, you can give a package name. Or else click Finish

![image](https://github.com/MaheshS03/Ex-03-SOAP-based-Web-Services/assets/128498431/d943fd39-3e06-4e74-90ab-aebe9ed43928)

#### Step 6:
In the Output Window at the bottom of NetBeans, you can notice that the client gathers the operations available in the web service.

#### Step 7:
Once it is done, you should see “BUILD SUCCESSFUL”.

#### Step 8:
Right-click on “Web Pages” under your Project and select “JSP”.

![image](https://github.com/MaheshS03/Ex-03-SOAP-based-Web-Services/assets/128498431/20d79f3c-04c3-4440-8912-ff4b53e0a342)

#### Step 9: 
A new window will appear, give a name to your jsp page and click Finish.

#### Step 10: 
Expand the folder named “Web Service References”-> “Addition” “Addition” “AdditionPort”. Once expanded you should see all the operations available in your web service.

#### Step 11: 
Carefully drag “add” operation and drop it into the JSP page. NetBeans will automatically create the code for invoking this operation which will be like,
 
![image](https://github.com/MaheshS03/Ex-03-SOAP-based-Web-Services/assets/128498431/d6bd1f52-2635-4edd-b376-3f19bcedd570)

#### Step 12: 
Give values to your arguments and run the JSP file. 

#### Step 13:
A new browser window with the output will appear. 

### Client-Side Remote Invocation

#### Step 1: 
Follow Step 1 and Step 2 as in Client-side (section 1.2).

#### Step 2:
A new window will appear. Select “WSDL URL” under the heading “Specify the WSDL file of the Web Service.” and type the URL of the web service’s WSDL file. (Typically, the URL of the form http://ip:8080/Proj_name/Webservice_name?wsdl)
 
![image](https://github.com/MaheshS03/Ex-03-SOAP-based-Web-Services/assets/128498431/1abcb9f9-4e63-47de-9ff6-db659094488a)

#### Step 3: 
The remaining procedure is the same as the Client-side.

## Result:
Thus, the SOAP based addition program using Web service is executed successfully.
