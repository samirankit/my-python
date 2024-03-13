# my-python
questions= {
 "hi": "hello, How can I help You",   
    
    "hello": "hi, How can I help You",
 "what is your name?": "My name is ChatBot.",
 "name?": "My name is uma.",
 "name please": "My name is uma.",
 "your name?": "My name is uma.",
 "wow are you?": "I'm doing well, thank you!",
 "what is the weather today?": "Trying to connect an API..... but API Not Found....Please Try Later",
 "who created you?": "I was created by You.",
 "your technology?": "I have been created using simple Python Script",
 "python?": "Python is a High Level Programming as well as Scripting language",
 "what is python?": "Python is a High Level Programming as well as Scripting language",
 "goodbye": "Goodbye! Have a nice day!"
}

# Function to get the chatbot's response
def get_chatbot_response(user_input):
    user_input = user_input.lower()
    if user_input in questions:
        return questions[user_input]
    else:
        return "I'm sorry, I don’t have any answer, Please try another question..... "


# Main chatbot loop
while True:
    user_input = input("User: ") # Get user input
    if user_input.lower() == "bye":
        print("uma: " + "Bye Bye, have a nice day !!")
        break # Exit the loop
    else:
        print("uma: " + get_chatbot_response(user_input))

        
