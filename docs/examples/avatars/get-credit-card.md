import { Client, Avatars, CreditCard } from "getapp";

const client = new Client()
    .setEndpoint('https://cloud.getapp.io/v1') // Your API Endpoint
    .setProject('<YOUR_PROJECT_ID>'); // Your project ID

const avatars = new Avatars(client);

const result = avatars.getCreditCard(
    CreditCard.AmericanExpress, // code
    0, // width (optional)
    0, // height (optional)
    0 // quality (optional)
);

console.log(result);
