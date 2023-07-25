# Following the chatgpt-retrieval Tutorial

Simple script to use ChatGPT on your own files.

Link to the [YouTube Video](https://youtu.be/9AXP7tCI9PI).

## Changes made
Pulling requirements from `requirements.txt`

## Further optimizations to come
Next iteration, will implement a webscraper to pull in and dump data via script.
Beyond that, will set up api calls to pull data from AWS.
Will Dockerize.

## Deps and Constants

Install required packages.
```
pip3 install -r requirements.txt
```
or manually
```
pip3 install langchain openai chromadb tiktoken unstructured
```

Create a `constants.py` and put your own [OpenAI API key](https://platform.openai.com/account/api-keys) in it, named `OPENAI_API_KEY`.

Place your own data/files into the `/data` directory in `.txt` format, like so, `data/<filename>.txt`.


## Example usage
Create a `data/data.txt` file. Put anything in here. Example:
`My name is Bob`
```
> python chat.py "what is your name?"
My name is Bob.
```

Example with proprietary data
![Screen Shot](https://github.com/vanessaholland/pythonML/blob/main/proprietary-gpt/images/local_data.png?raw=true)
