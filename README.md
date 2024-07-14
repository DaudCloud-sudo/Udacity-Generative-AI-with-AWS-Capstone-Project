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
5. [Step 5: Deploy and Evaluate the Fine-tuned Model](#step-4-deploy-and-evaluate-the-fine-tuned-model)

---

### Step 1: Environment and Project Setup

#### 1. Create an AWS SageMaker IAM Role
- Log into the AWS console using the "Launch Cloud Gateway" button in the course menu. Ensure you are working in the US-west-2 Region by selecting it from the dropdown menu in the top of the AWS console.
- Navigate to the SageMaker home page.
- In the left navigation menu, choose Role Manager and click on "Create a role."
- Name the role and configure it with the necessary permissions.

![image](https://github.com/user-attachments/assets/6ba72168-66f7-4c36-ad3a-ce1d5964a9cb)


#### 2. Create an AWS SageMaker Notebook Instance
- Go to the SageMaker home page and choose Notebook -> Notebook instances from the left navigation menu.
- Click on "Create notebook instance" and ensure you choose the IAM SageMaker role created in Step 1.

![image](https://github.com/user-attachments/assets/04a29a4c-346b-4bdd-a83d-a6663200bcf5)


#### 3. Request a GPU Instance for Training
- Visit the AWS Service Quotas dashboard and request an `ml.g5.2xlarge` instance for training job usage.
- Verify your request was approved by checking the Quota request history page.

![RequestingGPUForTraining](https://github.com/user-attachments/assets/d849d486-cf90-40ff-acd1-bba93e6a33a3)

---

### Step 2: Domain Choice
**Information Technology**  
I chose the IT domain to fine-tune the Meta Llama 2 7B model.

---

### Step 3: Model Evaluation

The Llama2 model was successfully deployed on AWS SageMaker. The output of the `Model_Evaluation.ipynb` file verifies the deployment.

![image](https://github.com/user-attachments/assets/753e4f0b-41a5-44f6-842d-587db13b0772)


**Response to domain-specific input:**
The model initially generated IT-specific content with a moderate level of relevance and coherence. It needs to be fine-tuned to produce highly accurate responses.

![image](https://github.com/user-attachments/assets/0dc4a43b-089e-4c7d-b821-83084f39ca6b)

The `Model_Evaluation.ipynb` file is attached for reference.

---

### Step 4: Fine-tuning the Model

I fine-tuned the model using a dataset relevant to the IT domain. The `Model_FineTuning.ipynb` notebook demonstrates the fine-tuning process. The dataset used for fine-tuning is specified in the `Model_FineTuning.ipynb` notebook file.

![image](https://github.com/user-attachments/assets/ad704b24-2a3e-4cdb-b49d-06b4f5df2f44)


The `Model_FineTuning.ipynb` file is attached for reference.

### Step 5: Evaluate the Fine-tuned Llama2 Large Language Model

After fine-tuning, I deployed the fine-tuned Llama2 model on AWS SageMaker. The deployment steps are shown in the `Model_FineTuning.ipynb` notebook cell output.


**Response to domain-specific input after fine-tuning:**
The fine-tuned model's performance on domain-specific text generation tasks showed a significant improvement. It provided more relevant and coherent responses to IT-specific queries.

![image](https://github.com/user-attachments/assets/397edcd6-83f3-4534-8529-58b93ee95317)


The `Model_FineTuning.ipynb` file is attached for reference.

---

