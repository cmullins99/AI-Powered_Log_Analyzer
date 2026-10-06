#  🛠️ AI-Powered Log Analyzer
  Instead of reading thousands of lines of server logs manually, you will write a Python program that automatically scans a log file, flags suspicious hacker activity, and passes that activity to an AI to generate a security report.
  1. The Software Engineering Piece (The Backbone)
    You will write a Python script that reads a mock server log file (a text file tracking everyone who tries to log into a website).
      •	What you'll do: Use Python's built-in file handling to open and read a log file line-by-line.
      •	The logic: Write basic conditional statements (like if/else loops) to look for anomalies—such as a single IP address failing to log in 5 times in less than a minute.
  2. The Cybersecurity Piece (The Context)
     You will learn how to spot a Brute-Force Attack or an SQL Injection, which are fundamental web security concepts.
      • What you'll do: Create a fake log file populated with normal traffic and a few malicious lines (e.g., 192.168.1.50 - [Failed Login] admin).
      •	The logic: Your script will isolate the hacker's IP address and group their suspicious behavior together so it can be evaluated.
  3. The AI Piece (The Intelligence)
    Instead of just printing "Attack Detected," your script will hand the malicious logs over to an AI to get expert context.
      •	What you'll do: Use a beginner-friendly API like OpenAI or Google Gemini (or a free local model using Ollama).
      •	The logic: You will write a prompt template that feeds the flagged logs into the AI. For example: "You are a Security Operations Center (SOC) analyst. Analyze these suspicious log lines, explain what the hacker is trying to do, and write a 3-bullet-point remediation plan for our network team."
________________________________________
# 🚀 Step-by-Step Blueprint to Build It
  1.	Step 1: Create a text file named server_logs.txt and paste 10–20 lines of fake server data into it. Mix normal page visits with a burst of 5 failed login attempts from a single IP.
  2.	Step 2: Write a Python script using standard file reading (open('server_logs.txt', 'r')) to parse the text file and identify any IP address with multiple failed logins.
  3.	Step 3: Sign up for a free or low-cost AI API key (like OpenAI or Anthropic). Install their official Python SDK via terminal (pip install openai).
  4.	Step 4: Pass the failed login data into the API query and print the AI's intelligent security response directly to your console or save it as a new security_report.md file.

