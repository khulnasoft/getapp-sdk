import { Client, Account } from "getapp";

const client = new Client()
    .setEndpoint('https://cloud.getapp.io/v1') // Your API Endpoint
    .setProject('<YOUR_PROJECT_ID>'); // Your project ID

const account = new Account(client);

const result = await account.createPhoneToken(
    '<USER_ID>', // userId
    '+12065550100' // phone
);

console.log(result);
