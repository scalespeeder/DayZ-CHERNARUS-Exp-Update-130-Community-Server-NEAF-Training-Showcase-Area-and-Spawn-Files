DayZ 1.30 Experimental CHERNARUS North East Airfield Training / Showcase Area For Console and PC xml json Mods Instructions & Terms Of Use

This file spawns multiple items at the NEAF which you can use for training and or video showcases.

Included new motorbikes and weapon skins.

Also included is a player spawn file that will spawn you at the North East Airfield. 

Limited Testing on PC Local Server, September 2026.

ONLY WORKS ON DAYZ 1.30 EXPERIMENTAL Chernarus Map & WHEN 1.30 GOES PUBLIC.

When 1.30 goes public this will be usuable on PC, XBox & PlayStation Community Servers.

Many Thanks To Inclement Dab for his amazing DayZ Editor that makes this all possible: https://steamcommunity.com/sharedfiles/filedetails/?id=2250764298

TERMS OF USE
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS
OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN
AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH
THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

Using these modded xml / json files and instructions could break the functioning of your DAYZ server, requiring a reinstall that would wipe
all player progress.

Using these modded files neccessitates increased regular restarts to prevent server crashing.

It is suggested you thoroughly test your server after applying these files to ensure proper
functioning of your server.

I always recomend you validate your files at: https://www.xmlvalidation.com/ and https://jsonformatter.curiousconcept.com/

Instructions:

Click the "Code" button and "Download Zip" on the Github Repository and extract the files on your local PC for access.

Ensure your DayZ Server has activated the cfggameplay.json. For console users on Nitrado Servers, go to "General Settings" on your server and tick "Enable cfggameplay.json".

On PC Servers add the following line to your serverDZ.cfg:

enableCfgGameplayFile = 1;

(On some PC servers, including Nitrado, the serverDZ.cfg is "hidden", so you need to enable "expert mode" in settings,
then go to "expert settings", which is the serverDZ.cfg. Stop the server before making changes this way.)

Upload "NEAF-Training-Area-130exp.json" from the extracted files to inside the "custom" folder of the (Chernarus) mission directory on your server. This file places the structures on your map.
(If you haven't got a "custom" folder, create one.)

In the main folder, first backup your vanilla cfgplayerspawnpoints.xml file by renaming it to cfgplayerspawnpoints.xml.bak , then upload the supplied cfgplayerspawnpoints.xml in its place.

Open the cfggameplay.json file in the correct mission file for your server and look for the "objectSpawnersArr" line.

This file tells your server to access your custom file.

Edit it to look like this: 

	"objectSpawnersArr": ["custom/NEAF-Training-Area-130exp.json"],
	
	
If you already are calling custom jsons to spawn items, seperate the files like this:

	"objectSpawnersArr": ["custom/NEAF-Training-Area-130exp.json","custom/differentfile.json"],
	
Save your changes & upload if you need to.
	
Restart your server and the new structures & items will appear immediatly. 

If you kill your existing character they will then re-spawn at the NEAF.

Thank you and enjoy :)  

Thanks, Rob.



