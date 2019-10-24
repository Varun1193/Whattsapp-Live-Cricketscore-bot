# Whattsapp-Live-Cricketscore-bot
This is a python program that extracts the live cricket score of a particular team for a specific date using Python's request library from a API and send the updates through a whatsapp text using Pyhton's twilio library.

Input is given to the program in the form of the name of the tesm we are interested in. Whenever the information is extracted from the API , each match is assigned a unique id. The program scans through each match and stores the unique id of the match that contain our team name. Then the match is accessed using its unique id. The entire information is extracted from API and stored in a dictionary. The stats and score of the match is extracted from the dictionary and stored in a message string.

Using twilio library , the program extracts the network id of the reciever's whatsapp address. It assigns a randomly generated unique id to the sender network. Now, using the twilio client function, the netwrok id of the reciever is linked with the network id of the sender. The the updates form the API is loaded in the message function and update is send when the program is executed.

