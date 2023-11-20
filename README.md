# toolsense

A starter project for playing with how well OpenAI and other API-compatible models work with tools to answer questions.

## Setup
If using OpenAI, set OPENAI_API_KEY in environment or in a .env file

## Running

poetry run python toolsense/toolsense.py --base-url https://api.openai.com/v1/ --model gpt-3.5-turbo-1106 --max-steps 5 'what was the weather here 3 days ago?'

This is a tool dependency graph test: it should ask for current date/time and current location and then ask for the weather give the date and location. It sometimes works with gpt35 and seems to always work with gpt4.

I haven't gotten it working with any open source models yet, but I think that's mostly a matter of prompt formatting. See https://twitter.com/abacaj/status/1726343354902802517

## Hacking

Right now this is just a single file to play with: toolsense.py. Make any changes to functions, prompts, memory, etc. there.
