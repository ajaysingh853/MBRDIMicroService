---------------------------------------------------------------------------------------------
Project Name - MBRDIService
Technologies Used - .Net Core Microservice API.
Docker - Dockerfile

--------------------------------------------------------------------------------------------
open project folder and then open powershell/cmd.
1. Redirect to this project folder in powershell/cmd
2. Create Docker Image Run Below Command in powershell/cmd.
   >docker build -t mbrdimicroservice .

3. create docker container and run docker image. run below command
    >docker run -it --rm -p 8080:80 --name mbrdimicroservicecontainer mbrdimicroservice

4. open postman to test api and then pass below API url in postman
    Request Method - POST
    API URL - http://localhost:8080/MBRDI/GetCurrentStatus
    JsonBody - {
                    "vin": "W1K2062161F0046",
                    "source": "Home",
                    "destination": "Movie Theatre"
                }

Thank you
