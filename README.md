# Starter template for Azure Functions in PowerShell

[![Open in Visual Studio Codespaces](https://img.shields.io/endpoint?style=social&url=https%3A%2F%2Faka.ms%2Fvso-badge)](https://online.visualstudio.com/environments/new?name=azure-functions-powershell&repo=mattchenderson/azure-functions-starter-powershell)

This is a starter template meant to help get started with new Azure Functions projects.

The template includes a basic "hello, world" function. The code for this repository was generated by following the instructions at [Create a function in Azure using Visual Studio Code](https://docs.microsoft.com/azure/azure-functions/functions-create-first-function-vs-code?pivots=programming-language-powershell#create-an-azure-functions-project).

Additionally, the repo includes a [dev container](https://code.visualstudio.com/docs/remote/containers) meant for use with [VS Code](https://code.visualstudio.com/) and [Visual Studio CodeSpaces](https://visualstudio.microsoft.com/services/visual-studio-codespaces/). Note that the VS CodeSpaces badge in this README points at the repo through a URL. If you intend to fork this repo, that URL will need to be updated accordingly in `README.md`.

## Generating the dev container for this project

1. In VS Code, run `CTRL+SHIFT+P -> Remote-Containers: Add Development Container Configuration Files...`.

2. Click "Show All Definitions..." if needed and select "Azure Functions & PowerShell 6".

3. In the generated Dockerfile, make sure that [version 3](https://github.com/Azure/azure-functions-core-tools#v3) of the Azure Functions Core tools is being used by updating line 67 to: `&& apt-get install -y azure-cli azure-functions-core-tools-3 \`. _(This step will soon be removed now that https://github.com/microsoft/vscode-dev-containers/pull/321 has been merged.)_
