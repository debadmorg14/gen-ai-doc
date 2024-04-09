---
sidebar_position: 1
---

# Amazon Q - Welcome to a new world of work with Amazon Q

Amazon Q can help you get fast, relevant answers to pressing questions, solve problems, generate content, and take actions using the data and expertise found in your company's information repositories, code, and enterprise systems. When you chat with Amazon Q, it provides immediate, relevant information and advice to help streamline tasks, speed decision-making, and help spark creativity and innovation at work.

## Amazon Q Business
Amazon Q Business is a fully managed, generative-AI powered assistant that you can configure to answer questions, provide summaries, generate content, and complete tasks based on data in your enterprise. Amazon Q provides immediate and relevant information to employees, and helps streamline tasks and accelerate problem solving.

Amazon Q integrates with services such as Amazon Kendra and other supported data sources such as Amazon S3, Microsoft SharePoint, and Salesforce.

## Amazon Q  Quicksight (Generative BI)

Amazon Q in QuickSight enhances business productivity using Generative BI capabilities to accelerate decision-making. With new dashboard authoring capabilities in Amazon Q, business analysts can use natural language prompts to build, discover, and share meaningful insights in seconds. Amazon Q makes it easier for business users to understand data with executive summaries, a new context-aware data Q&A experience, and customizable, interactive data stories.


## Amazon Q  Developer (Accelerate your SDLC)

Amazon Q Developer harnesses cutting-edge generative artificial intelligence (AI) to accelerate your software development lifecycle (SDLC). With deep understanding of your code and AWS resources, it streamlines research, design, coding, testing, debugging, troubleshooting, and modernization. Amazon Q is there to help wherever you need it—in the AWS Management Console, integrated development environment (IDE), AWS documentation, and through Slack and Microsoft Teams.


## Custom Web Experience with Amazon Q Business

Customers often want the ability to integrate custom functionalities into the Amazon Q user interface, such as handling feedback, using corporate colors and templates, custom login, and reducing context switching by integrating the user interface into a single platform. The code repo will show how to use Amazon Cognito for user authentication and use Amazon Q SDK to invoke chatbot application programmatically


### Architecture
1.	First the user accesses the chatbot application, which is hosted behind the Load Balancer.
2.	On the first log in attempt the user is be redirected to the Amazon Cognito log in page for authentication. After successful authentication, the user is redirected back to the chatbot application.
3.	The custom UI, deployed on EC2, parses the token to obtain the user and group information, as well as the user's question. 
4.	The UI sends the above information to Amazon Q using the chat_sync boto3 API. AmazonQ return a response containing the answer and the sources used to generate it.

