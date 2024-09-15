import { Client, Teams } from "getapp";

const client = new Client()
    .setEndpoint('https://cloud.getapp.io/v1') // Your API Endpoint
    .setProject('<YOUR_PROJECT_ID>'); // Your project ID

const teams = new Teams(client);

const result = await teams.listMemberships(
    '<TEAM_ID>', // teamId
    [], // queries (optional)
    '<SEARCH>' // search (optional)
);

console.log(result);
