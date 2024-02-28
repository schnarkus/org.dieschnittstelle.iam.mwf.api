## MWF Framework simple API server. 
For educational use only. Also see LICENSE file.

# Prerequisites
- make sure that Node.js and npm are installed; see: https://docs.npmjs.com/downloading-and-installing-node-js-and-npm
- you also need a local installation of the MongoDB community server; see: https://www.mongodb.com/try/download/community

# Install dependencies
in the project directory, run: npm install

# Run
- start mongodb
- in the project directory, run: node webserver.js

# Access
try accessing: http://localhost:7077/api/mediaitems; you should receive the following result: {"data":[]}

# Note
- please note that api access is neither password-protected, nor, by default, secure
- therefore, currently, the server is setup for running under localhost / 127.0.0.1; in case you want to run it with your network IP address, make sure that you are situated in some environment where you can exclude unauthorised access. For starting the server with the network IP address, set the localOnly constant in webserver.js, line 5, to false. 
- if the port shall be changed, change the assignment in line 7 of webserver.js
- note that, in case of a change of ip address and/or port, in the oncreate() method of the application class of the MWF client application the new base url needs to set using the xhr.setBaseUrl() method.
