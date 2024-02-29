## This is a public repository to explore very simple and effective examples/use cases for some OpenAI models on Azure

We currently have two use cases in this repository

### Call Center Analytics:

We will use the Whisper model to get the transcript from a call and send to GPT-4 to analyze the call.

The ideia is to evaluate the agent performance asking the model to analyze some tasks. You can explore this use case further with your own audio files and provide the tasks you want to assess

File: [Speech-CallCenterAnalytics-demo.ipynb](Speech-CallCenterAnalytics-demo.ipynb)

### Purchase Order information extraction:

In this use case we are using GPT-4 Vision to extract all necessary information from a Purchase Order and format the output in JSON format. That way we can automate the process of identifying all the information from the PO

File: [purchaseOrder-gpt4v-demo.ipynb](purchaseOrder-gpt4v-demo.ipynb)

