- Tools to software development - JSON Server: create a file named db.json in the root directory to be used by the JSON Server.

```
npm install -g json-server --save-dev
# Execute the server
npx json-server --port 3001 --watch db.json
# or `json-server --port 3001 --watch db.json` to execute the server
```
