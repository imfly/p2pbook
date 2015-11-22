### DApp Toolkit

The official Crypti decentralized application (DApp) toolkit.

Requires:

  * Crypti 0.5.0

### Directory Structure

  * **modules** - Contains the backend code of your dapp.
  * **public** - Contains the frontend user interface of your dapp.
  * **blockchain.json** - JSON file describing the SQL database schema. You will need this if you want to store any data within your dapp.
  * **config.json** - JSON file containing your dapp's configuration data. By default this file defines a list of peers.
  * **genesis.json** - JSON file containing important information about your dapp's genesis block.
  * **index.js** - JavaScript file used to start your dapp.
  * **modules.full.json** - JSON file containing a list of defined modules, required by **index.js**.
  * **routes.json** - JSON file defining the HTTP routes of every endpoint in your dapp's API.

Full documentation is available [here](https://github.com/crypti/crypti-dapps-docs).

curl -XPUT -H "Content-type: application/json" -d '{
"recipientId": "18298233975495868793C",
"message": "Hello, world!",
"secret": "."
}' 'http://localhost:7040/api/dapps/11700699929086527232/api/messages/add'

curl -XGET 'http://localhost:7040/api/dapps/11700699929086527232/api/messages/list?recipientId=18298233975495868793C'

18298233975495868793C

/dapps/api/11700699929086527232/api/messages/list