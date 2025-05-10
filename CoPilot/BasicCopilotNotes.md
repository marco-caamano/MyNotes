# Basic Copilot Notes

## See alternate suggestions
Use ```Ctrl+ENTER``` to see other alternatives than the copilot suggested ghost text


## Custom Copilot Instructions

From https://code.visualstudio.com/docs/copilot/copilot-customization#_use-instruction-files

Create a file under ```.github/copilot-instructions.md``` and use this file to give general guidance for copilot like:

- Project Overview and Description
- Setup Instructions
- Coding Conventions
- Best Practices
- Prompts and suggestions

The info here will be added to the context when copilot generates code...

### Custom GIT Messages

From https://code.visualstudio.com/docs/copilot/copilot-customization#_specify-custom-instructions-in-settings

Create ```.vscode/settings.json``` and set customer git commit message instructions:

```
{
    "github.copilot.chat.commitMessageGeneration.instructions": [
        {
            "text": "Frist line should provide a short summary under 50 characters. Second Line should be blank. If the current branch is called jira_XXXX where XXXX is a number, then on the third line list the Jira ticket number. If there is a JIRA ticket number leave a blank line after the third line. Then add a detailed list description of all changes made"
        }
    ]
}
```

Can also specify files to read instructions from:
```
{
    "github.copilot.chat.commitMessageGeneration.instructions": [
        {
            "text": "Frist line should provide a short summary under 50 characters. Second Line should be blank. If the current branch is called jira_XXXX where XXXX is a number, then on the third line list the Jira ticket number. If there is a JIRA ticket number leave a blank line after the third line. Then add a detailed list description of all changes made"
        },
        {
            "file": ".CustomGit.md"
        }
    ]
}
```
Can also add custom files like .sql with Database SQL schema to the custom instructions

### Other scpecific custom settings for Copilot

Other specific settings:
```
github.copilot.chat.testGeneration.instructions
github.copilot.chat.reviewSelection.instructions
github.copilot.chat.pullRequestDescriptionGeneration.instructions
```
