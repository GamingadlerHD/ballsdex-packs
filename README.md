# ballsdex-packs
### Optional packages for the ballsdex discord bot


## License
Licensed under the Apache License, Version 2.0 (the "License");
You may obtain a copy of the License at:

    http://www.apache.org/licenses/LICENSE-2.0
    
Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.



## **HOW TO INSTALL:**

### NOTE: MAKE CREDITS TO GAMINGADLERHD

1. Place your Package (the folder you also downloaded) in  ```/ballsdex/packages/ ```

2. Open  ```/ballsdex/core/bot.py ``` with any text/code editor

3. At line 35 you will find a list of packages 
 ```PACKAGES = ["config", "players", "countryballs", "info", "admin", "trade"] ```

4. Add your folder name to this list, for example, if you want to add gafusion, edit the line like this:
 ```PACKAGES = ["config", "players", "countryballs", "info", "admin", "trade", "gafusion"] ```

5. Now you have to do special edits, which are different for all packs.

5a. gafusion

- at line 97 in  ```/gafusion/cog.py ``` you find the number 12, right after  ```special= ```, replace that number with your special ID of the card you want to use for fusion.
you find the id at the Admin-Panel>Specials>Left side

5b. gafusionv2 

- at line 81, 83 and 197 in  ```/fusionv2/menu.py ``` you find the number 10, replace all of them with (for example) 7 if the users should only need 7 countryballs to fuse.

- at line 390 in  ```/gafusionv2/cog.py ``` you find the number 12, right after  ```special= ```, replace that number with your special ID of the card you want to use for fusion.
you find the id at the Admin-Panel>Specials>Left side

5c. gararity

- You can skip that part

5d. gaspawnping

- replace  ```/ballsdex/packages/countryballs/countryball.py ``` with the 2. file you downloaded, named  ```countryball.py ```.

5e. gavote

- go to https://webhook-topgg.com/ 
- press get started
- enter your discord webhook (The channel should be private, otherways everyone can trigger rewards) and press next
- set the content to  ```r.votereward <user> ``` and press next
- for Embed Presets select "None" and press Test
- if the message on discord says  ```r.votereward 311553339261321216 ``` you done everything right
- Press next. You will get a URL and Authorization, coppy them
- Open the top.gg side of your bot and press edit.
- on the left select webhooks, then you will find 2 fields, where you can place your URL and Authorization.
- press save and exit the website
- now coppy the id of the channel where your webhook is.
- open  ```gavote/cog.py ``` and replace the id on line 48 with your id.
- get the id of the channel where you want to send the reward info (User321 got a reichtangle for voting)
- replace the id in  ```gavote/cog.py ``` on line 51 with your channel id.


6. Restart your bot by running the following commands in your command line:

         docker compose down

         docker compose build 

         docker compose up

7. Test your feature.



















