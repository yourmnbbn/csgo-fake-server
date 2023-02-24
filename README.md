# csgo-fake-server
- Fake server with fake online players in the csgo community browser.  

Yes, this is exactly what you want, a fully functioning csgo fake server with fake online support. Follow the instructions and you'll get your's for free. It has been tested but still there might be problems during using. If you encounter any problems or bug, or just want to request for a new feature please open an issue. I maintain all my repos in my free time so the responses or fixes might be very quick or very slow.

## How to setup
1. Compile and run [tiny-csgo-server](https://github.com/yourmnbbn/tiny-csgo-server). This project will help to register a server which will be displayed in the community server browser. As for how to compile or configure please refer to the readme of that repo. Once this is setup, you'll get a fake server displayed. Ofc you can run multiple servers at a time. But online players of the fake servers will always be 0. To solve this problem, you have to follow the next instruction.

2. Compile and run [tiny-steam-client](https://github.com/yourmnbbn/tiny-steam-client). This project will help to login steam accounts, generating app ticket and send them to tiny-csgo-server to authenticate. As for how to compile or configure please refer to the readme of that repo. You'll need tons of accounts to support your fake online. You just have to configure all the accounts ahead of time and then tiny-steam-client will do everything left for you.

tiny-csgo-server and tiny-steam-client support both on linux and windows.

## Special notice about accounts
One account can only be authenticated by one single server, it can't be authenticated by multiple server. For example you want to create 3 fake servers, each with 32 fake online players, you have to prepare 3*32 which is 96 accounts with steam guard turned off.
