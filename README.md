# Serverless Full-Stack Task Board
A task board UI with a deployable AWS Lambda + API Gateway backend template (AWS SAM). The frontend includes demo mode so it runs without AWS credentials.

## Frontend demo
```bash
npm install
npm run dev
```

## Deploy backend (AWS SAM)
Prerequisites: AWS CLI configured and SAM CLI installed.
```bash
cd backend
sam build
sam deploy --guided
```
After deployment, copy the API endpoint into `src/main.jsx` as `API_URL` (or set it to empty for local demo mode). Backend stores tasks in DynamoDB.

## Features
- Add, complete, and delete tasks
- Demo local storage mode
- AWS Lambda API (GET/POST/DELETE) and DynamoDB table infrastructure template
- Responsive UI
