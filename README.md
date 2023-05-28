# Performance Portafolio
Performance Testing with Jmeter Scripts
All scripts have to be saved under "scripts" folder
___

1. Requirement.- create a basic script using JMeter to hit the following API about Jokes: <p>
  https://official-joke-api.appspot.com/random_joke
2. Requirement.- create a basic script that use query parameters in the URL for the cat facts endpoint, use the follwing swagger documentation: <p>
  https://catfact.ninja/#/Facts
3. Requierment.- create a basic script that hits 5 different endpoints using query parameters for the Bored API using the following API documentation:<p>
  https://www.boredapi.com/documentation
4. Requirement.- Create a JMeter script that is able to request all the US (Unated State) holidays for the year 2022. To do this use the following page: <p>
https://calendarific.com/api-documentation <p>
You will need to create an account on this page and get an API Key, so click on Sign UP create an account and go to the url: <p>
https://calendarific.com/account <p>
Once there copy the API Key in the API Access Details section:
![api-key-description-image](img/api-key.PNG)
Then use this API Key as explained in the official documentation described above.
5. Requirement.- Create a JMeter based on the Postman file to get the tracks of spotify. You can get the Postman project from [This file](postman/Spotify.postman_collection.json) <p>
In order to be able to do the request you will need the following dependencies:
- Create or already have an existing Spotify Account (Free is ok)
- Go to [this link](https://developer.spotify.com/documentation/web-api/concepts/apps) and click on dasbhoard (make sure you are logged in spotify first)
![Dasboard link](img/sp-img1.PNG)
- In the next screen click on **Create App** ![Create App](/img/sp-img2.PNG)
- Fill the main details of the application name and description fields can be as you want. But make sure you fill in the same way the refresh uri ![app creation](/img/sp-img3.PNG)
- Go to the Settings section:
![settings](/img/sp-img4.PNG)
- Copy the CLIENT ID and Client Secret
- Finally use this information in the Post call in your postman collection in the authentication part. ![Postman collection](/img/sp-img5.PNG)
6. Requirement.- Create a JMeter script to solve the business process [in this excel](/data/Performance_Test_Case_Template%20-%20PDF%20Creator.xls), to do it, you are going to need access to the follwing [Postman Collection](/postman/postman_collection_pdf_creation). <p>
Finally in order to make the PDF collection work, you are going to need to get the a working session token (JWT token), follow the instructions below. <p>
  - ### How to get your JWT token
  - Go to the following page and create a free account [PDF Generator Account](https://pdfgeneratorapi.com/login). Login using your google or github account or create your account using your email and custom password.
  - Once you have created your account you will see the following dasboard: <p>
  ![dashboard](/img/pdf-1.PNG)
  - Now go to the Templates section and create a new template using the create template button ![create template](/img/pdf-2.PNG)
  - Do anything in the template and Save it with the name you want: ![Save tamplate](/img/pdf-2.1)
  - The template now will appear in your template list if you go to Templates in the menu section.
  - Now go to the **Account Settiings** Section in the left menu and in case you dont see any API Credentials listed like the image, then click in the highlghted button **Generate new pair Keys**
  - Now click on **Generate Temporary JWT token** Button ![JWT Token](/img/pdf-3.PNG)
  - You will see in the button of the screen your new created JWT token. Now copy this token and use it in your piostman collection. ![Token](/img/pdf-4.PNG)
  - Finally use this copied JWT token in your postman collection in the Autentication section on the collection level like the following image: ![Postman reference](/img/pdf-5.PNG)
  - ## IMPORTANT
    - Use all the good practices that you know so far (Transactions, Assertions, Correlations and parameters)
    - If you need to understand more about the API here is the [API Documentation](https://docs.pdfgeneratorapi.com/v3/#section/Authentication/Creating-a-JWT)