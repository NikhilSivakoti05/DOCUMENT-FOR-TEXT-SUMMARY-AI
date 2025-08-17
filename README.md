# DOCUMENT-FOR-TEXT-SUMMARY-AI

When you visit the website and gave prompt please wait it is free AI API Key it may be slow sometimes due to traffic
I used the MERN stack for my project. My initial approach was to handle everything from the frontend: the app takes user uploads, uses an AI API key (I also used the Deepseek API key) to generate responses, and then sends emails to a particular person using EmailJS.

At first, the frontend fetched and displayed the data directly. However, I realized that scaling the application would become difficult with this setup. So, I created a simple backend proxy for my application, following this flow:

Frontend → Backend → Deepseek → Frontend

Now, if I want to scale the application or add other features, it’s much easier. I used ChatGPT and Lovable for my templates, but the main files are aiservice.js and emailshare.jsx, where all the main logic resides. I hosted the frontend on Vercel and the backend (proxy server) on Render.com.
