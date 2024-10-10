
# Building a Serverless Text-to-Speech Application with Amazon Polly

This project demonstrates how to build a serverless text-to-speech application using **Amazon Polly**, **Amazon S3**, **API Gateway**, and **AWS Lambda**. The application converts text input into lifelike speech and delivers the audio output in a scalable, cost-effective, and efficient manner.

## Project Overview

The serverless application allows users to input text through an API, which is then processed by Amazon Polly to generate speech in real time. The audio output is stored in Amazon S3, making it easily accessible for users to download or stream.

### Key AWS Services Used

- **Amazon Polly**: Provides lifelike speech synthesis by converting text into natural-sounding speech.
- **AWS Lambda**: Executes the text-to-speech conversion logic using Amazon Polly.
- **Amazon S3**: Stores the generated audio files for users to access.
- **Amazon API Gateway**: Serves as the entry point for users to input text and trigger the Lambda function.

### Architecture

The architecture of this project includes the following components:

1. **Amazon API Gateway**: Provides a REST API interface for users to submit text input.
2. **AWS Lambda**: The backend logic for invoking Amazon Polly and processing the text-to-speech conversion.
3. **Amazon Polly**: Converts the submitted text into speech.
4. **Amazon S3**: Stores the resulting audio files for easy access.
5. **IAM Roles and Permissions**: Secure access between services (Polly, S3, Lambda) and the API.

### How It Works

1. **Text Input**: A user submits text through the API Gateway.
2. **Invoke Lambda**: API Gateway triggers a Lambda function that processes the input.
3. **Text-to-Speech Conversion**: Lambda calls Amazon Polly to convert the input text into an audio file.
4. **Store in S3**: The resulting audio file is stored in an S3 bucket.
5. **Return Audio File URL**: Lambda returns the URL of the audio file stored in S3 for the user to access.

### Benefits of the Serverless Approach

- **Scalability**: The solution automatically scales to handle varying workloads.
- **Cost Efficiency**: With pay-per-use pricing for Lambda and Polly, costs are kept low when the application is idle.
- **Ease of Management**: No server provisioning or management is needed thanks to the serverless architecture.

## Setup and Deployment

To replicate this project, follow these steps:

1. **Create an API Gateway**: Set up an API Gateway with a POST method to accept text input.
2. **Deploy Lambda Function**: Write a Lambda function to process text input and call Amazon Polly to convert it into speech.
3. **Set Up Amazon Polly**: Ensure that Polly is configured to handle requests from your Lambda function.
4. **Create an S3 Bucket**: Store the generated audio files in an S3 bucket.
5. **Grant Permissions**: Assign appropriate IAM roles to Lambda for interacting with Polly and S3.
6. **Test the Application**: Use API Gateway to submit text and retrieve the generated audio file URL.

## Skills and Learnings

Through this project, I gained experience in:

- Using Amazon Polly to convert text into speech.
- Building a fully serverless architecture with Lambda, S3, and API Gateway.
- Managing security and permissions using IAM roles.
- Implementing event-driven architectures for on-demand services.

## View Project Details

You can view the project details [here](https://awsportfolio.sila.studio/project/building-a-serverless-text-to-speech-application-with-amazon-polly/).

## Acknowledgments

This project was completed as part of the **Digital Cloud Training** bootcamp. 

![Screenshot 2024-05-10 154146](https://github.com/user-attachments/assets/c2450f06-014b-46f4-b958-ed9016ca0948)
