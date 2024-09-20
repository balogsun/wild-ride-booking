
# Architecture
![Screenshot 2024-05-28 182547](https://github.com/juggernaut09/wildrydes-site/assets/25864009/eca4897a-ba58-4246-bc36-7bf291633d4c)

# Wild Rydes Serverless Web Application
This application allows users to request unicorn rides from the Wild Rydes fleet. The project includes an HTML-based user interface for indicating a pick-up location and a RESTful web service on the backend to submit requests for dispatching a unicorn. Additionally, it provides user registration and login functionalities to ensure a secure and personalized experience.

The Wild Rydes serverless web application leverages AWS cloud services to deliver a scalable and secure platform for requesting unicorn rides. Users can sign up, log in, and specify their pick-up locations via a user-friendly web interface. The backend processes these requests and dispatches unicorns accordingly.

## The application consists of the following components:

- Static Web Hosting: Hosted on AWS Amplify, providing HTML, CSS, JavaScript, and image files.
- User Management: Managed by Amazon Cognito for secure authentication and authorization.
- Serverless Backend: Implemented using AWS Lambda for handling business logic.
- RESTful API: Exposed through Amazon API Gateway to interact with the Lambda functions.
- Data Persistence: Utilizes Amazon DynamoDB for storing request data.

## Technologies Used
- **AWS Lambda**: provide backend process for handling requests from your web application, i.e. function that is invoked whebver a user requests a unicorn to be sent to a location of his/er choice. The function will select a unicorn from the fleet, record the request in a DynamoDB table and then respond to the front-end application with details about the unicorn being dispatched.
- **Amazon API Gateway**: makes it easy for developers to create, maintain, and secure APIs. It's used to expose the Lambda function built as a RESTful API..
- **Amazon DynamoDB**: NoSQL database service used to provide a table to record the unicorn requests in a DynamoDB table.
- **Amazon Cognito**: lets you add user sign-up, sign-in, and access control to your web and mobile apps quickly and easily. In this solution, it's used to manage users, federate identities, and manage user pools.
- **AWS Amplify**: simplify application lifecycle, including builds and deploys the web application by following a continuous integration and delivery model.
- **Amazon S3**: Object storage for hosting static web site content (HTML, CSS, JavaScript, images and other files).

# Setup and Deployment

## Hosting the Static Website
> Configure AWS Amplify to host the static resources for your web application, ensuring continuous deployment is set up for easy updates and maintenance.

## Managing Users
> Create an Amazon Cognito user pool to handle user accounts, providing secure registration and login capabilities for the application.

## Building the Serverless Backend
> Develop backend processes using AWS Lambda to handle ride requests from users. These functions will execute the core logic of the application.

## Deploying the RESTful API
> Use Amazon API Gateway to expose the Lambda functions as a RESTful API, allowing the frontend to communicate with the backend seamlessly.




