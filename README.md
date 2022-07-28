
# How to run this application

## Backend

To deploy this application run the following commands:

```
cd backend
npm install
sls deploy -v
```

## Frontend

To run a client application first edit the `client/src/config.ts` file to set correct parameters. And then run the following commands:

const apiId = 'you will this apiId after deploying the backend succefuly to AWS'

export const apiEndpoint = `https://${apiId}.execute-api.us-east-1.amazonaws.com/dev`

export const authConfig = {
  domain: '',           // Auth0 domain
  clientId: '',  // Auth0 client id
  callbackUrl: 'http://localhost:3000/callback'
}
```
cd client
npm install
npm run start
```

This should start a development server with the React application that will interact with the serverless TODO application.
user will be able to login wuth auth verification ,creat and edit his or her to do list 



