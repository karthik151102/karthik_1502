# karthik_1502
# Define the chatbot's responses
responses = {
    "hello": "Hello! How can I help you today?",
    "how are you": "I'm just a computer program, but I'm here to help you. How can I assist you?",
    "bye": "Goodbye! Have a great day!"
}

# Continuously prompt the user for input
while True:
    user_input = input("You: ").lower()
    
    # Check if the user's input matches a key in the responses dictionary
    if user_input in responses:
        print("Chatbot: " + responses[user_input])
    elif user_input == "":
        continue
    else:
        print("Chatbot: I'm sorry, I don't understand. Can you please rephrase that?")
    
    # Exit the loop if the user says "bye"
    if user_input == "bye":
        break
