# AZURE_CERTIFICATION

The purpose of this repo is to document and navigate of various learning tasks in regards to AZURE CERTIFICATIONS. 


## Table of Contents
1. Usefull Links
2. Tips and Tricks

## Usefull Links
[AI Foundry](https://ai.azure.com/)

[AI Foundry in VS Code](https://learn.microsoft.com/en-us/azure/ai-studio/how-to/develop/vscode)


## Tips and Tricks

### AI applications in Azure AI Foundry

To provision an entirely new set of resources, including a new hub and project, and deploy these sample applications, you can use the [Azure Developer CLI](https://learn.microsoft.com/en-us/azure/developer/azure-developer-cli/) (AZD) in your local development environment.


### AI Foundry in VS Code container

Even if you [enable idle shutdown on your compute instance](https://learn.microsoft.com/en-us/azure/ai-studio/how-to/create-manage-compute#configure-idle-shutdown), it will not occur for any compute that is set up with this custom VS Code container. This is to ensure the compute doesn't shut down unexpectedly while you're working within a container.

### Network isolation

If your Azure AI Foundry project is configured for network isolation you might need to open ports to the internet, For more information, visit [How to configure network isolation](https://learn.microsoft.com/en-us/azure/ai-studio/how-to/configure-managed-network#scenario-use-visual-studio-code).


#### Container folder structure

The container is configured with the Azure AI folder hierarchy (afh directory), which is designed to orient you within your current development context, and help you work with your code, data, and shared files most efficiently. This afh directory houses your Azure AI Foundry projects, and each project has a dedicated project directory that includes `code`, `data`, and `shared` folders.

| Folder | Description |
| --- | --- |
| `code` | Use for working with git repositories or local code files. |
| `data` | Use for storing local data. |
| `shared` | Use for working with a project's shared files and assets such as prompt flows. |


It's recommended that you work within this project directory. Files, folders, and repos you include in your project directory persist on your host machine (your compute instance). Files stored in the code and data folders will persist even when the compute instance is stopped or restarted, but will be lost if the compute is deleted. However, the shared files are saved in your hub's storage account, and therefore aren't lost if the compute instance is deleted.

#### When workin across multiple repositories

If you plan to work across multiple code and data directories, or multiple repositories, you can use the split root file explorer feature in VS Code. To try this feature, follow these steps:

1. Enter Ctrl+Shift+p to open the command palette. Search for and select Workspaces: Add Folder to Workspace.
2. Select the repository folder that you want to load. You should see a new section in your file explorer for the folder you opened. If it was a repository, you can now work with source control in VS Code.
3. If you want to save this configuration for future development sessions, again enter Ctrl+Shift+p and select Workspaces: Save Workspace As. This action saves a config file to your current folder.
