FIRST THING'S FIRST — GEMINI-POWERED SALON WEBSITE

Includes a responsive salon website, price menu, WhatsApp/Instagram links, and a Gemini-powered chatbot. The server sends the salon menu as the chatbot's knowledge context. The API key stays server-side.

RUN LOCALLY (Node.js 20+)
1. Install Node.js 20 or newer.
2. Create a Gemini API key in Google AI Studio: https://aistudio.google.com/app/apikey
3. Copy .env.example to a file named .env.
4. Put your key after GEMINI_API_KEY= in .env. Never share or publish this key.
5. In this folder, run: npm start
6. Open http://localhost:3000
7. Test the chat: "How much is the express manicure?"

DEPLOYMENT
This is a Node.js server app, not just static HTML. Deploy the entire folder to a Node-capable host such as Render or Railway. Add GEMINI_API_KEY as a secret/environment variable in the host dashboard. Do not upload .env or commit the key to GitHub. The public chatbot will use Gemini only after the server is deployed and the key is configured.

SECURITY / LIMITATIONS
- Never put the Gemini key in index.html or frontend JavaScript.
- Add production rate limiting, monitoring and abuse protection before public launch.
- Gemini usage may be subject to quotas and charges. Review Google's current terms and pricing.
- The bot cannot confirm bookings, current hours or address because those details were not provided.
- Owner portrait remains a placeholder. Replace with a photo approved by Riyana.
- Replace stock gallery photos with salon-owned photos before launch.
- Verify all menu prices against the latest salon price list.
