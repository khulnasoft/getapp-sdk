import { Client, Account } from "getapp";

const client = new Client()
    .setEndpoint('https://cloud.getapp.io/v1') // Your API Endpoint
    .setProject('<YOUR_PROJECT_ID>'); // Your project ID

const account = new Account(client);

const result = await account.updatePhone(
    '+12065550100', // phone
    'password' // password
);

console.log(result);
