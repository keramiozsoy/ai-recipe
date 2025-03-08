# ai-recipe



## recipe-1

## aim

"n8n" is running on docker but ollama can't. Let's run "ollama" locally for "deepseek language model"

![recipe1 - Screenshot](https://github.com/keramiozsoy/ai-recipe/blob/main/resources/images/recipe1.png)


## install


### install docker 

https://docs.docker.com/desktop/setup/install/mac-install )

### install ollama

https://ollama.com

### install deepseek language model

Open your terminal

```SHELL

ollama run deepseek-r1:1.5b

```
### install n8n kit

```SHELL

git clone https://github.com/n8n-io/self-hosted-ai-starter-kit.git
cd self-hosted-ai-starter-kit

```

Open docker-compose.yml and replace OLLAMA_HOST

```
 - OLLAMA_HOST=host.docker.internal:11434
```

Let's see ui of n8n

```SHELL
docker compose up
```

Additionally, after you see "Editor is now accessible via: http://localhost:5678/":

1 Head to http://localhost:5678/home/credentials
2 Click on "Local Ollama service"
3 Change the base URL to "http://host.docker.internal:11434/"


### Run 

Open chat and ask your questions.



### resources

https://github.com/n8n-io/self-hosted-ai-starter-kit?tab=readme-ov-file#for-mac--apple-silicon-users

