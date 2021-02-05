# Shell : GitHub + VScode project automation

Automate the process of creating a new project and adding it to GitHub with a single command.
The command creates a new directory on your machine, initializes a Github repo with a README and pushes it to the configured Github account.
It then navigates to the newly created directory and runs `code .` to open your project folder in VS Code.

## Requirements

* VScode
* Git (Bash)
* Node
* dotenv
* [Github API](https://docs.github.com/en/github/authenticating-to-github/creating-a-personal-access-token)

Uses [**dotenv**](https://www.npmjs.com/package/dotenv) to load up environment variables from the **_.env_** file and the Github API through [**octonode**](https://www.npmjs.com/package/octonode) which is '_a library for nodejs to access the github v3 api_'.

## Setup

1. Download / clone this project
2. Open terminal in the project directory
3. Run `npm i dotenv octonode`
4. Open **.env**
  - add GitHub username, use your GitHub **token** as password
  - I recommend the following path: `DIRECTORY='../Documents/'`
5. Open file explorer, and move **_.my_commands.sh_** to: `windows/Users/<your username >` 
6. Open **.bashrc** in the same location
  - Type: `source ~/.my_commands.sh`
  - If you don't have this file, open Git Bash and type: `echo "source ~/.my_commands.sh" >> ~/.bashrc`
7. Move the **Bash_VScode_Project_automation**-folder to the same location. Result: `windows/Users/<your username >/Shell_VScode_Project_automation`
7. Restart your terminal

## Usage

From Git Bash

```
create <name of your project>
```

## Credits

Copied from [boubacar-io](https://github.com/boubacar-io/project-creation-automation) -> inspired by KalleHallden's [ProjectInitializationAutomation](https://github.com/KalleHallden/ProjectInitializationAutomation) which uses Python.

## Disclaimer

I don't take responsibility for any faults related to this guide
