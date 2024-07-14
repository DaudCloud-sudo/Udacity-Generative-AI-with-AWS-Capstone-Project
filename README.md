# LLM-model-evaluation-and-Fine-tuning
Evaluation and fine-tuning of Meta Llama 2 7B model using AWS SageMaker for text generation in IT domains.

---

# UDACITY: Introduction to Generative AI with AWS

## Project Documentation Report

### Contents
1. [Step 1: Environment and Project Setup](#step-1-environment-and-project-setup)
   1. [Create an AWS SageMaker IAM Role](#create-an-aws-sagemaker-iam-role)
   2. [Create an AWS SageMaker Notebook Instance](#create-an-aws-sagemaker-notebook-instance)
   3. [Request a GPU Instance for Training](#request-a-gpu-instance-for-training)
2. [Step 2: Domain Choice](#step-2-domain-choice)
3. [Step 3: Model Evaluation](#step-3-model-evaluation)
4. [Step 4: Fine-tuning the Model](#step-4-fine-tuning-the-model)

---

### Step 1: Environment and Project Setup

#### 1. Create an AWS SageMaker IAM Role
- Log into the AWS console using the "Launch Cloud Gateway" button in the course menu.
- Navigate to the SageMaker home page.
- In the left navigation menu, choose Role Manager and click on "Create a role."
- Name the role and configure it with the necessary permissions.

![Creating AWS Sagemaker IAM Role](C:\Users\DAUD\Desktop\AWS Project/to/IAM-Role_Sagemaker-1.png)

#### 2. Create an AWS SageMaker Notebook Instance
- Go to the SageMaker home page and choose Notebook -> Notebook instances from the left navigation menu.
- Click on "Create notebook instance" and ensure you choose the IAM SageMaker role created in Step 1.

#### 3. Request a GPU Instance for Training
- Visit the AWS Service Quotas dashboard and request an `ml.g5.2xlarge` instance for training job usage.
- Verify your request was approved by checking the Quota request history page.

---

### Step 2: Domain Choice
**Information Technology**  
I chose the IT domain to fine-tune the Meta Llama 2 7B model.

---

### Step 3: Model Evaluation

The Llama2 model was successfully deployed on AWS SageMaker. The output of the `Model_Evaluation.ipynb` file verifies the deployment.

**Screenshots of model deployment:**

![Model Deployment](path/to/model_deployment_screenshot.png)

**Response to domain-specific input:**
The model initially generated IT-specific content with a moderate level of relevance and coherence. It needs to be fine-tuned to produce highly accurate responses.
**Screenshots of model evaluation:**

![Model Evaluation](path/to/model_evaluation_screenshot.png)

The `Model_Evaluation.ipynb` file is attached for reference.

---

### Step 4: Fine-tuning the Model

I fine-tuned the model using a dataset relevant to the IT domain. The `Model_FineTuning.ipynb` notebook demonstrates the fine-tuning process. The dataset used for fine-tuning is specified in the `Model_FineTuning.ipynb` notebook file.

**Screenshots of fine-tuning process:**

![Fine-tuning Process](path/to/fine_tuning_screenshot.png)

The `Model_FineTuning.ipynb` file is attached for reference.

### Evaluate the Fine-tuned Llama2 Large Language Model

After fine-tuning, I deployed the fine-tuned Llama2 model on AWS SageMaker. The deployment steps are shown in the `Model_FineTuning.ipynb` notebook cell output.

**Screenshots of fine-tuned model deployment:**

![Fine-tuned Model Deployment](path/to/fine_tuned_model_deployment_screenshot.png)

**Response to domain-specific input after fine-tuning:**
The fine-tuned model's performance on domain-specific text generation tasks showed a significant improvement. It provided more relevant and coherent responses to IT-specific queries.

**Screenshots of fine-tuned model evaluation:**

![Fine-tuned Model Evaluation](path/to/fine_tuned_model_evaluation_screenshot.png)

The `Model_FineTuning.ipynb` file is attached for reference.

---

This structured format should make it easy for anyone to follow the steps and understand the project setup and evaluation process.
