# Basic Ai by Jeffrey Milik

import random

# Sample dictionary with 20 input types and weighted responses

response_dict = {
   "hello": [("Hi there!", 0.6), ("Hello!", 0.3), ("Greetings!", 0.1)],
   "how are you": [("I'm doing great, thank you!", 0.5), ("All systems are running smoothly.", 0.3), ("I feel fantastic today!", 0.2)],
   "what is your name": [("I'm a friendly AI assistant.", 0.7), ("You can call me Max!", 0.3)],
   "what do you do": [("I help answer questions and chat with people.", 0.6), ("I'm here to assist you with anything I can.", 0.4)],
   "tell me a joke": [("Why don't scientists trust atoms? Because they make up everything!", 0.7), ("I tried to catch fog yesterday. Mist.", 0.3)],
   "what is ai": [("AI stands for Artificial Intelligence.", 0.6), ("It's the simulation of human intelligence by machines.", 0.4)],
   "what is python": [("Python is a powerful programming language.", 0.6), ("It's often used for AI and data science.", 0.4)],
   "who made you": [("I was created by OpenAI.", 0.8), ("OpenAI built me using machine learning models.", 0.2)],
   "what time is it": [("I'm not connected to real time, but your device knows!", 1.0)],
   "goodbye": [("See you soon!", 0.5), ("Goodbye!", 0.4), ("Take care!", 0.1)],
   "thank you": [("You're welcome!", 0.7), ("No problem!", 0.2), ("Anytime!", 0.1)],
   "what is love": [("Love is a deep, complex emotion.", 0.5), ("Baby don't hurt me. (Just kidding!)", 0.5)],
   "who is picard": [("Captain Picard is a Starfleet legend from Star Trek.", 0.7), ("He’s the captain of the USS Enterprise-D.", 0.3)],
   "do you dream": [("I imagine I do, in code and circuits.", 0.6), ("Dreams? Not quite, but I simulate thoughts.", 0.4)],
   "tell me something cool": [("Octopuses have three hearts!", 0.5), ("Bananas are berries, but strawberries aren't!", 0.5)],
   "favorite color": [("I like blue—it feels vast and calm.", 0.7), ("I'd say blue, if I could see it!", 0.3)],
   "how old are you": [("I was launched in 2022, so I'm quite young!", 1.0)],
   "can you code": [("Absolutely! I can write Python, JavaScript, and more.", 1.0)],
   "sing a song": [("♪ I'm a little chatbot, short and smart... ♫", 1.0)],
   "help me": [("Of course! What do you need help with?", 0.7), ("I’m here for you—ask me anything.", 0.3)],
}

def chatbot_response(user_input):
   user_input = user_input.lower()
   for key in response_dict:
       if key in user_input:
           responses, weights = zip(*response_dict[key])
           return random.choices(responses, weights=weights)[0]
   return "I'm not sure how to respond to that yet."

# loop
if __name__ == "__main__":
   print("Chatbot: What would you like to know? ")
   while True:
       user_input = input("You: ")
       if user_input.lower() in ["exit", "quit"]:
           print("Chatbot: Nice talking to you, goodbye!")
           break
       print("Chatbot:", chatbot_response(user_input))
