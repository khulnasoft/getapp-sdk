import { Client, Teams } from "getapp";

const client = new Client()
    .setEndpoint('https://cloud.getapp.io/v1') // Your API Endpoint
    .setProject('<YOUR_PROJECT_ID>'); // Your project ID

const teams = new Teams(client);

const result = await teams.create(
    '<TEAM_ID>', // teamId
    '<NAME>', // name
    [] // roles (optional)
);

console.log(result);
