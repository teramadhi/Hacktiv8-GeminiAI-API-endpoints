# Hacktiv8-GeminiAI-API-endpoints
Hacktiv8 - AI Wave 2 Developer -Implement Gemini AI API endpoints

2025-07-15, Version 22.17.1 'Jod' (LTS)
Gemini API 

npm install express dotenv @google/generative-ai multer

- express: Sets up the REST API.  
- dotenv: Loads the Gemini API key securely from a .env file.  
- @google/generative-ai: Connects to the Gemini API (including Flash 2.0). (July 2025)  
- multer: Handles file uploads (image, audio, document inputs).  

.env file : This file holds environment variables, especially sensitive credentials like your Gemini API key. i.e : GEMINI_API_KEY=your_credential_key

const { prompt } = req.body; Retrieves the user’s prompt input sent from the client (e.g., Postman or frontend).

Test text API using POSTMAN  
1.Open Postman  
2.Method: POST  
3.URL: http://localhost:3000/generate-text  
4.Tab: Body → raw → JSON  
5.Input prompt  
6.Click Send  
7.See the response  

Test file (image, audio & document) API using POSTMAN  
1.Open Postman  
2.Method: POST  
3.URL: http://localhost:3000/generate-from-image  
4.Tab: Body → form-data  
5.Added 2 key:  
A. image (type: File) → upload file .png, .jpg, etc.  
B. prompt (type: Text) → i.e : Describe this image/audio/document  
6.Click Send  
7.See the response  

