![github banner bevel](https://github.com/user-attachments/assets/8eef11d8-7923-4ca0-b709-e7e08b95d2c1)

# What is it?


# Installation

On the [releases page](https://github.com/SeanPuller/Houdini-AI-Code-Nodes/releases). Download and unzip Houdini.AI.Code.Nodes.zip. Then place the hda's in your otls folder. 

The first time you open Houdini after adding the nodes you will see some updates in the console. This is adding the openai python package dependency. When this is done, restart Houdini.

## Dependencies
### openai python package
This is the standard api for communicating with llms.
The openai package should install automatically using pip the first time the nodes are added. You will see some updates in the console, When this is done, restart Houdini.

### Troubleshooting
If you need to manually add the python package. Using the correct version of python for your installation of Houdini and run:
```
pip install openai
```

# Connecting to an LLM

The settings dropdown has the properties for the API key, URL and Model. Update these parameters to work with your preferred service.

After updating the parameters right click the properties and 'Make current value default' so you don't have to do this every time create a new node.

The default parameters are setup to work with LMStudio.

![image](https://github.com/user-attachments/assets/ec73e658-0df5-4d13-a550-c1a34c44fe87)

# LLM Options
These nodes should work with any llm service, local or remote, that uses the openai api.
## Local
### [LM Studio](https://lmstudio.ai/)
LM Studio has a great interface for downloading and using models.
To use with the nodes, go to the developer tab, load a model and start the server.

Settings Example:
```API Key: lm-studio```
```URL: http://localhost:1234/v1```
```Model: model-identifier```


### [Ollama](https://ollama.com/)
Settings Example:
```API Key: ollama```
```URL: http://localhost:11434/v1/```
```Model: llama2```

## Cloud
[Here is a good list of providers](https://github.com/XueyanZhang/awesome-ai-mode-api?tab=readme-ov-file)

### [OpenRouter (Free)](https://openrouter.ai/)
OpenRouter is a great service that has free models you can use. The free gemini models are quite good
Settings Example:
```API Key: generated api key```
```URL: https://openrouter.ai/api/v1/```
```Model: google/gemini-2.0-flash-lite-preview-02-05:free```


# Features
Create Code

Modify Code

Fix Errors
