import { Client, Locale } from "getapp";

const client = new Client()
    .setEndpoint('https://cloud.getapp.io/v1') // Your API Endpoint
    .setProject('<YOUR_PROJECT_ID>'); // Your project ID

const locale = new Locale(client);

const result = await locale.listCountriesEU();

console.log(result);
