# vscode-using-http-restclient-.vscode-settings.json-for-testing
How to use rest client in vscode and put environment variables under .vscode/settings.json file

Basically in order to test our REST APIs directly from vscode-> we can use RestAPI extension and we are free from all hassles of using browsers
espcially for Micro-Service based APIs where we will get our results immediately

Ofcourse for long running processing (e.g. batch load - gisupdate project where the load takes 1 hour) then we can use browser 
http://localhost:3003/docs (swagger).  All based on our requirement

After intalling RestClient extension in vscode just refer to test_api.http script to see how you setup APIs for different environments
# References:
1. https://marketplace.visualstudio.com/items?itemName=humao.rest-client - valid vscode extension to setup REST client
2. https://medium.com/refinitiv-developer-community/how-to-test-rest-api-with-visual-studio-code-rest-client-extensions-9f2e061d0299
