#Python Voice Assistant

A versatile and interactive voice-activated personal assistant built in Python. This assistant can understand voice commands to perform a variety of tasks, from fetching real-time information to controlling your local machine.
Features

    Real-time Information:

        Current Time: Asks for and speaks the current time.

        Live Weather: Fetches and reports the current weather for any specified city, or automatically detects the user's location.

        Top News Headlines: Retrieves and prints the latest news headlines from India (or any configured country).

    Desktop Control:

        Open Applications: Opens common applications like Notepad, Microsoft Word (or equivalents), and Excel. Easily customizable for any OS (Windows, macOS, Linux).

    Personal Assistant Tools:

        Set Reminders: A conversational two-step process to set reminders for specific tasks and times.

    Customization:

        Adjustable Speaking Speed: The assistant's voice rate can be controlled via a simple voice command.

        Secure Configuration: Uses a .env file to securely manage private API keys, keeping them separate from the source code.

#Tech Stack

    Language: Python 3

    Core Libraries:

        Speech Recognition: SpeechRecognition (using Google Web Speech API)

        Text-to-Speech: pyttsx3

        Web Requests: requests

        Environment Variables: python-dotenv

        Date/Time Parsing: parsedatetime

    APIs:

        OpenWeatherMap API for weather data.

        NewsAPI.org for news headlines.

#Setup and Installation

Follow these steps to get the voice assistant running on your local machine.
1. Prerequisites

    Python 3.7+

    pip package manager

    A working microphone

2. Clone the Repository

First, clone this repository to your local machine:

git clone https://github.com/YourUsername/voice-assistant-project.git
cd voice-assistant-project

3. Create a Virtual Environment

It is highly recommended to use a virtual environment to manage project dependencies.

 Create the virtual environment
python3 -m venv venv

 Activate it (on Windows)
venv\Scripts\activate

 Activate it (on macOS/Linux)
source venv/bin/activate


4. Set Up Environment Variables

This project requires API keys for weather and news.

    Create a file named .env in the root directory of the project.

    Sign up for free accounts and get your API keys from:

        OpenWeatherMap

        NewsAPI.org

    Add your keys to the .env file as shown below:

    .env file
    WEATHER_API_KEY="your_actual_openweathermap_key_goes_here"
    NEWS_API_KEY="your_actual_newsapi_org_key_goes_here"

#Usage

Once the setup is complete, you can run the assistant from your terminal:

python assistant.py

The assistant will greet you and start listening for your commands.
Example Commands

    "What time is it?"

    "What's the weather like?"

    "What's the weather in London?"

    "Tell me the news" or "Show me the sports headlines"

    "Remind me to take a break" (followed by a time)

    "Open notepad"

    "Create a document"

    "Set speed to 170"

    "Stop" or "Exit"

