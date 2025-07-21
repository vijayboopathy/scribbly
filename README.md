# scribbly
A simple personal note taking app based on Markdown and written in Python

## Feature list
 - [ ] App should work on my linux server and phone
 - [ ] Write/Store/Sync from linux server
 - [ ] Write/Store/Sync from android phone
 - [ ] Simple UI that performs the following
 - [ ] A directory browser to the left
 - [ ] A writer pane and a preview pane in the focus area
 - [ ] Sync and Cancel bottons at the bottom

## Requirements
 - [ ] A linux server(pc)
 - [ ] An android phone
 - [ ] Some kind of remote storage(sqlite in s3?)

## Framework decision
 - [Kivy](https://kivy.org/) and [Beeware](https://beeware.org/) seems to be the two obvious choices for this project. I don't know which one to chose. 
   - From the initial analysis, Kivy seems to have more project showcases that are similar to mine. So proceeding with it.

## Installation
 - Install [uv](https://github.com/astral-sh/uv)
 ```bash
 # On macOS and Linux.
 curl -LsSf https://astral.sh/uv/install.sh | sh
 ```

 - Initialize the project
 ```bash
 uv init ../scribbly
 ```

 - Install python 3.xx
 ```bash
 uv python install 3.13
 ```

 - Pin python version
 ```bash
 uv python pin 3.13
 ```

 - Create a virutal environment
 ```bash
 uv venv
 ```

 - Compire requirements
 ```bash
 uv pip compile pyproject.toml \
 --universal \
 --output-file requirements.txt
 ```

 - Install kivy
 ```bash
 uv add kivy
 ```
 - Install the locked requirements
 ```bash
 uv pip sync requirements.txt
 ```

