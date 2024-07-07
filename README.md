python -m venv ./ollama-langchain-venv

.\ollama-langchain-venv\Scripts\activate

docker build . -t abvijaykumar/ollama-langchain:0.2

docker-compose up

docker exec -it ollama-langchain-ollama-container-1 ollama run phi3
