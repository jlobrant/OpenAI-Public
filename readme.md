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

Will be updated soon!!!
