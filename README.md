# GoogleTranslate
This is an example of how to translate using Google Translate via google-cloud.

**NOTE:** This example requires a Google Cloud account with access to the Google Translate API.

## Prerequisites
1. Ensure you have an account with [Converse.AI](http://www.converse.ai/)
2. Converse.AI extensions run on **Node.JS** `v6.11.1` on **Alpine Linux** so ensure your node development environment matches this setup. We recommend installing Node.JS via [Node Version Manager (NVM)](https://github.com/creationix/nvm).
3. Install and Authorize [Converse.AI CLI tool](https://dash.readme.io/project/converseai/v2/docs/converse-ai-cli).

## Install
5. Clone repo
6. Initialize extension by running `converse-cli plugin init` from your project root.
7. Set up Google Translate project.
    1. In the Cloud Platform Console, go to the Projects page and select or create a new project – [Google Projects Page](https://console.cloud.google.com/project)
    2. Enable billing for your project – [Google Billing Page](https://support.google.com/cloud/answer/6293499#enable-billing)
    3. Enable the Cloud Translation API – [Google Cloud Translation API](https://console.cloud.google.com/flows/enableapi?apiid=translation.googleapis.com)
    4. Go to **Credentials** and create a new **Service account key** and download the JSON file. 
    5. Rename the file `credentials.json` and add it to the project root.
8. Run `npm test` from your project root to ensure everything was initialized correctly.
9. Deploy the plugin to your Converse.AI account by running `converse-cli deploy` from your project root.
10. If there are no errors, the plugin should be available under "User" in the left hand menu of the designer.
