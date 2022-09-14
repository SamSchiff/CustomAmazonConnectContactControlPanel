# Amazon Connect Custom Contact Control Panel

## Steps to run
1. install npm: https://docs.npmjs.com/downloading-and-installing-node-js-and-npm
1. run `git clone https://github.com/SamSchiff/CustomAmazonConnectContactControlPanel.git`
1. run `cd CustomAmazonConnectContactControlPanel`
1. run `npm install`
1. In the index.html file, add in your Connect instance url on the line that says "UPDATE URL HERE". Leave out the trailing "/"
1. Go to your Connect instance page in the AWS console. Find the "Approved Origins" page. Add in "http://localhost:4000" and "https://localhost:4000". This will allow the Connect instance to be iframed by this application.
1. run `npm run dev`. This will start your application at localhost:4000

## Advanced
1. Update the Streams version by updating the version number in the script tag url "https://unpkg.com/amazon-connect-streams@2.3.1/release/connect-streams.js"
1. Customize your `initCCP` call in the index.html with the options specified here https://github.com/amazon-connect/amazon-connect-streams/blob/master/Documentation.md#connectcoreinitccp