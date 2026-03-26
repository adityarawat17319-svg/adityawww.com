https://github.com/adityarawat17319-svg/adityawww.com.gitstart
def chatbot():
    print("🤖 AI Bot: Hello! Main aapka AI assistant hoon.")
    
    while True:
        user = input("You: ").lower()
        
        if "hello" in user:
            print("🤖 AI Bot: Hello Aditya 😄")
            
        elif "kaise ho" in user:
            print("🤖 AI Bot: Main badhiya hoon! Tum batao?")
            
        elif "bye" in user:
            print("🤖 AI Bot: Bye! Phir milte hain 👋")
            break
            
        else:
            print("🤖 AI Bot: Mujhe samajh nahi aaya, thoda aur clear bolo.")

chatbot()import openai

openai.api_key = "YOUR_API_KEY"

def ai_chat():
    while True:
        user = input("You: ")
        
        response = openai.ChatCompletion.create(
            model="gpt-4o-mini",
            messages=[{"role": "user", "content": user}]
        )
        
        print("AI:", response['choices'][0]['message']['content'])

ai_chat() bot start bot
