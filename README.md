# Twitch Python Examples (examples folder)

### 1. Example Webhook 
Name: webhook_example.py  
Description: program that creates a webhook to listen for twitch channel follows  

### 2. Example API Request 
Name: api_example.py  
Description: program that finds the broadcaster ID associated with a users Twitch channel name  

### 3. Example Twitch IRC Code
Name: irc_example.py  
Description: program that saves twitch chat messages as a text file  


### 4. Example Twitch IRC Listener
Name: irc_listener.py  
Desciption: program that waits for a command in twitch chat to return a response  

# Twitch Chat Markov Model Sentence Generator
1. Twitch Chat Log Collection (log_bot.py)  
Listens to twich chat and saves user info and user logs in a corresponding json file.  This program uses twitch webhooks  
to determine if the channel is online in order to save chat logs exclusively while the stream is live.  

2. Twitch Chat Log Processing (make_model.py)  
Processes the chat logs stored by the log bot to determine token start, end, and transition probabilities.  
This program filters logs to remove specific tokens, chatters, and infrequently used words.  

3. Markov Model Sentence Generation Bot (make_sentence.py)  
Connects to specified channel's twich chat and waits for a command to send a reponse generated by the markov model.  

### Auxilliary Files
1. chatbot.yml  
  conda environment containing the python libraries needed to run all programs  
2. irc_commands.py  
  auxilliary file containing the classes and methods used by other programs to interface with twitch chat  
3. run_XXX_.sh  
  example shell scripts to run their respective python programs

