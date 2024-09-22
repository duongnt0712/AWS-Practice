# Exercise 1
## Use Case
A sports platform development company is building a web application that updates weather information from Yahoo! Weather.
The company needs to deploy the application on AWS under the domain https://web.ngsport.com, and the application will be deployed on an EC2 cluster in the Singapore Region.

Please design a system that meets the following conditions:
- There must always be at least 2 instances running the application in 2 different availability zones (AZs) to ensure high availability.
- The web application is accessible from the internet while maintaining security.
- The web application must always be able to update weather data even if one of the AZs in Singapore goes down due to a power outage.
- The web application should be protected against DDoS attacks.

The progress detail will be update in the note: [Hands-on: Exercise 1](https://duongnt.notion.site/Exercise-1-e32e33e461cb4020b95b92e1f03393fa)
![Excercise 1 Diagram](https://github.com/duongnt0712/AWS-Practice/blob/main/Exercise%201/Excercise%201%20Diagram.png)
