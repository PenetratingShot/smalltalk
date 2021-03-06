# Smalltalk

Smalltalk is a bash program which tries to use Snips NLU in order to create a chatbot in the terminal. You just need to run the program and it will create a prompt where you can type

## Prerequisites

Install [jq](https://stedolan.github.io/jq/download/) for your OS

Install [python3](https://python.org)

Download snips-nlu (`$pip install snips-nlu`)

## Installation

This assumes that you've already finished the prerequisites for installation above

`$ git clone https://github.com/penetratingshot/smalltalk.git`

`$ cd smalltalk`

`$ chmod +x ./main.sh`

`$ ./main`

That's all! Typing in `./main` will bring up a prompt. You can exit this prompt by using KeyboardInterrupt or `exit()`

## Development Status

- [x] create infinite prompt
- [x] add basic commands
    - [x] help()
    - [x] exit()
    - [x] version()
- [x] Training
    - [x] create training dataset for intents (may split up into different files)
    - [x] sync dataset to python code
- [x] Working with Data
    - [x] transfer utterance to a file
    - [x] read utterance from file
    - [x] shift utterance to python code
    - [x] make prediction in python (can run from bash)
    - [x] shift data to file
- [ ] Weather
    - [ ] read from output file
    - [ ] check whether either only city entity or both city and state entities exist
        - [ ] if only state exists, return error to user
    - [ ] grab api key from .env file
    - [ ] Yahoo Weather API
        - [ ] make GET request with cURL
        - [ ] parse appropriate data with jq
        - [ ] store data in variables
        - [ ] create concatenated string and present to user
- [ ] Adding basic conversations (going to be hard)
- [ ] Implement other commands (coming soon)

## Known Bugs
- [x] commands not working after blank input