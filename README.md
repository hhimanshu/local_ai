# Steps

- Start the containers

```bash
docker-compose up -d
```

- Install the model

```bash
docker exec -it ollama ollama pull llama3
```

Here `llama3` is the model name and version. You can find the list of available models [here](https://ollama.com/library). This may take a while to complete as it depends on

1. Your internet speed
2. The size of the model.

Leav the command running. You should be able to see progress in the terminal like below

```txt
(base) ➜  data docker exec -it ollama ollama pull llama3
pulling manifest 
pulling 00e1317cbf74...  27% ▕████████████████████████████████████████                                                                                                              ▏ 1.2 GB/4.7 GB   56 MB/s    1m0s                                                                                                                                                      ▏  71 KB/ 39 GB
```

The models will be downloaded at `data/ollama/models` directory.

- Access the Web UI. Open your browser and navigate to `http://localhost:3333`. If this is your first time running the application, you will be prompted to create an account. Once you have created an account, you will be redirected to the dashboard. Use any email and password to create an account. It does not matter since this is a local setup.
- Once you, you can see the downloaded model in the dashboard. You may see it a view similar to the following
![Dashboard](https://i.imgur.com/aQv7bMn.png)

That's it, you can now start using the model. Here is a demo of how to use the model  

![Imgur](https://i.imgur.com/0QsE8Sf.mp4)  
