import { Client, Avatars } from "getapp";

const client = new Client()
    .setEndpoint('https://cloud.getapp.io/v1') // Your API Endpoint
    .setProject('<YOUR_PROJECT_ID>'); // Your project ID

const avatars = new Avatars(client);

const result = avatars.getFavicon(
    'https://example.com' // url
);

console.log(result);
