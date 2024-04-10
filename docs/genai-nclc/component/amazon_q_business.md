---
sidebar_position: 1
---
# Amazon Q Business

## Custom Web Experience with Amazon Q Business

Customers often want the ability to integrate custom functionalities into the Amazon Q user interface, such as handling feedback, using corporate colors and templates, custom login, and reducing context switching by integrating the user interface into a single platform. The code repo will show how to use Amazon Cognito for user authentication and use Amazon Q SDK to invoke chatbot application programmatically


### Architecture
1.	First the user accesses the chatbot application, which is hosted behind the Load Balancer.
2.	On the first log in attempt the user is be redirected to the Amazon Cognito log in page for authentication. After successful authentication, the user is redirected back to the chatbot application.
3.	The custom UI, deployed on EC2, parses the token to obtain the user and group information, as well as the user's question. 
4.	The UI sends the above information to Amazon Q using the chat_sync boto3 API. AmazonQ return a response containing the answer and the sources used to generate it.

### [sample code](https://github.com/aws-samples/custom-web-experience-with-amazon-q-business/tree/main)

