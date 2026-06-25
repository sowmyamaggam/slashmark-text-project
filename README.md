# slashmark-text-project
# Simple Text Assistant 

import datetime
import webbrowser

print("=== SIMPLE ASSISTANT ===")
print("Type 'bye' to exit.\n")

while True:
    command = input("You: ").lower()

    if "hello" in command:
        print("Assistant: Hello! How can I help you?")

    elif "time" in command:
        current_time = datetime.datetime.now().strftime("%H:%M:%S")
        print("Assistant: Current time is", current_time)

    elif "date" in command:
        today = datetime.date.today()
        print("Assistant: Today's date is", today)

    elif "open google" in command:
        print("Assistant: Opening Google...")
        webbrowser.open("https://www.google.com")

    elif "open youtube" in command:
        print("Assistant: Opening YouTube...")
        webbrowser.open("https://www.youtube.com")

    elif "bye" in command:
        print("Assistant: Goodbye!")
        break

    else:
        print("Assistant: Sorry, I don't understand.")
