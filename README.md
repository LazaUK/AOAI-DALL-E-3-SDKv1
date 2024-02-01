# Image generation with Azure OpenAI DALL-E 3
DALL-E 3 is a Generative AI model from OpenAI, which can be used to generate images based on your textual input (prompt). You will find a Jupyter notebook in this repo, that can utilise Azure OpenAI deployment of DALL-E 3 to generate caricature image of a famous Disney character.

To build this demo, I used the latest OpenAI Python SDK v1.x. To upgrade your _openai_ Python package, please use the following pip command:
```
pip install --upgrade openai
```

## Table of contents:
- [Part 1: Configuring solution environment](https://github.com/LazaUK/AOAI-DALL-E-3-SDKv1/tree/main?tab=readme-ov-file#part-1-configuring-solution-environment)
- [Part 2: Generating and visualising required image](https://github.com/LazaUK/AOAI-DALL-E-3-SDKv1/tree/main?tab=readme-ov-file#part-2-generating-and-visualising-required-image)

## Part 1: Configuring solution environment
1. To use API key authentication, assign the API endpoint name, version and key, along with the Azure OpenAI deployment name of DALL-E 3 model to **OPENAI_API_BASE**, **OPENAI_API_VERSION**, **OPENAI_API_KEY** and **OPENAI_API_DEPLOY_DALLE** environment variables respectively.
![screenshot_1.1_environment](images/environment_var.png)
>**Note**: If you want to use the Entra ID (former Azure Active Directory) authentication instead, you may find some implementation options [here](https://github.com/LazaUK/AOAI-EntraIDAuth-SDKv1).
2. Install the required Python packages, by using the **pip** command and the provided requirements.txt file.
```
pip install -r requirements.txt
```

## Part 2: Generating and visualising required image

![dalle3_image](/images/dalle3_generated.png)
