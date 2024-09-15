import { Client, Storage } from "getapp";

const client = new Client()
    .setEndpoint('https://cloud.getapp.io/v1') // Your API Endpoint
    .setProject('<YOUR_PROJECT_ID>'); // Your project ID

const storage = new Storage(client);

const result = await storage.listFiles(
    '<BUCKET_ID>', // bucketId
    [], // queries (optional)
    '<SEARCH>' // search (optional)
);

console.log(result);
