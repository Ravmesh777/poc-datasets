# Build and deploy
#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
Command to build the application. PLease remeber to change the project name and application name
```
gcloud builds submit --tag gcr.io/streamilit-app/streamilit-app  --project=streamilit-app
```

Command to deploy the application
```
gcloud run deploy --image gcr.io/966395558829/streamilit-app --platform managed  --project=966395558829 --allow-unauthenticated
```