## This is a public repository to explore very simple and effective examples/use cases for some OpenAI models on Azure

We currently have two use cases in this repository

### Call Center Analytics:

We will use the Whisper model to take a transcript of a call and send it to GPT-4 to analyze the call.

The idea is to evaluate the agent's performance by asking the model to analyze some tasks. You can further explore this use case with your own audio files and provide the tasks you want to evaluate

File: [Speech-CallCenterAnalytics-demo.ipynb](Speech-CallCenterAnalytics-demo.ipynb)

### Purchase Order information extraction:

In this use case, we are using GPT-4 Vision to extract all the necessary information from a purchase order and format the output in JSON format. This way we can automate the identification process of all PO information

File: [purchaseOrder-gpt4v-demo.ipynb](purchaseOrder-gpt4v-demo.ipynb)

## Configurations

Configure the [template.env](template.env) file accordingly. You need to provide endpoint, key, model name and deployment values in order to run the demos sucessfully.

### Service Deployment instructions

Guide for model deployment: [https://learn.microsoft.com/en-us/azure/ai-services/openai/how-to/create-resource?pivots=web-portal[(https://learn.microsoft.com/en-us/azure/ai-services/openai/how-to/create-resource?pivots=web-portal)

#### Quick instructions about env.env file:

#### For Vision endpoint you need to put the value in the following format:

```yaml annotate
openai_completion_endpoint_vision = "https://{your_service_endpoint}.openai.azure.com/openai/deployments/{deployment}/extensions/chat/completions?api-version=2023-07-01-preview"
```

Do the same for the openai_completion_endpoint

#### For the Whisper you need to use the base url:

```yaml annotate
openai_completion_endpoint_whisper = "https://{your_service_endpoint}.openai.azure.com/"
```

Same for openai_api_endpoint

This is what env.env should look like:

![image](https://github.com/jlobrant/OpenAI-Public/assets/31459994/84a57aeb-4fa3-42c4-a029-4736f221d41e)

You might have multiple deployments in different regions due to current model availability. Example:

- Whisper model is only available in North Central US or West Europe (as of Feb 29 2024)
- GPT-4 Vision is only available in Sweden Central, West US, Japan East, Switzerland North and Australia East (as of Feb 29 2024)

Note: You can use GPT-4 Vision for Vision and as the defaul model for completion too.

Use this link to be check the current situation: [https://learn.microsoft.com/en-us/azure/ai-services/openai/concepts/models](https://learn.microsoft.com/en-us/azure/ai-services/openai/concepts/models)
