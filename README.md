# Bionic-GPT Installed Version

## Install Instructions - My hacked workaround

Start the [ollama server](https://github.com/addictgamer/ollama-runner) and install `llama2_uncensored`.
You can use these commands if you clone [that repo](https://github.com/addictgamer/ollama-runner) and start a terminal session in there:
```bash
task start
```
Then open a second terminal in that same repo and run this:
```bash
NAME=llama2-uncensored task download-model-from-library
```

Then start a terminal in this repo and start docker:
```bash
task start # or `task start-daemon`
```
Then configure Bionic GPT to use your ollama endpoint.

## Bad Install Instructions

Directions from: https://bionic-gpt.com/docs/running-locally/gpu-setup-ollama/

~~Get the docker file:~~
```bash
# curl -O https://raw.githubusercontent.com/bionic-gpt/bionic-gpt/main/docker-compose/docker-compose.yml
# curl -O https://raw.githubusercontent.com/bionic-gpt/bionic-gpt/main/docker-compose/docker-compose-ollama.yml
```
~~Then to launch it:~~
```bash
#docker-compose -f docker-compose.yml -f docker-compose-ollama.yml up # This one's ollama app doesn't work for me!
```
Theirs don't work. Use the one provided in this repo.

