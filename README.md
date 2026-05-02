 AI-Powered Job Application Tracker

An automated workflow that generates personalized internship cold 
emails using AI and saves them to Notion automatically.

  Tech Stack
- n8n (workflow automation)
- Groq API + LLaMA 3.3 70B (AI email generation)
- Notion API (application database)
- Webhook (trigger)

  How It Works
1. Webhook receives company name and role
2. Edit Fields node stores the input data
3. HTTP Request calls Groq API → LLaMA writes personalized email
4. Notion saves company, role, AI email, status, and date

  How to Use
1. Import the .json file into your n8n instance
2. Add your Groq API key in the HTTP Request node
3. Connect your Notion account and select your database
4. Send a POST request with company and role to the webhook
5. Check Notion for the saved application!

  Real World Value
Reduces time spent writing cold emails from 10 minutes to 3 seconds.
Tracks all applications in one place automatically.
