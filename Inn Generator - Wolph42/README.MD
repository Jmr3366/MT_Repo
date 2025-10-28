Wolph42🐺 — 5/16/2020 9:58 AM


	HOW TO USE THIS
	This map is standalone. That means you can load it, use it  and remove it from your campaign file without issue. Just keep in mind that when you do this you either:
	- run 'onCampaignLoad' macro (yelllow, under '50. tools' group OR 
	- save and reload the campaign file
	so the macros are initialized.

	To load an MT map: go to menu-->Map-->Import Map
	To delete an MT map: go to menu-->Map-->delete...
 
	Given that this map is rather 'asset heavy' (=its big) my adivice is to do exactly that: load it, run OCL, create a couple of Inns, place them on other maps and remove this map again. 

	How?
	Here a short step by step of the basic process:
	1. There is a token on this map (upper left of the red area) with a wolf on it. Select or impersonate that. Then check the 'selection' or 'impersonation' panel.
	2. At the top you will find two blue buttons: the manual and generate inn. Those two are basically the only ones you really need.
	3. Generate an inn, it will appear in the (red) 'construction area'
	4. At the top left corner of the generated Inn you will see a 'stone brown corner piece' (on the TOKEN layer). This is the 'InnStant'. You can create multiple InnStants HOWEVER its important that you copy paste it (anywhere you like) BEFORE you generate the next Inn. This because the original InnStant will be deleted as soon as you generate a new Inn. 
	5. rince and repeat 3 and 4 as often as you want.
	6. The InnStant represents the Upper left of you Inn and you can place them anywhere in your campaign file (so also on other maps). To employ them:
	a. put them where you want the Inn (token layer is fine)
	b. select the InnStant
	c. go to the selection panel
	d. here you find three buttons 'InnStant' and 'deInnStall' (lights currently dont work, working on it), hit the 'InnStant' macro and the Inn will appear 
	
	One really important drawback however is that Inns can ONLY BE CONSTRUCTED ON 100px map!!. Usually not a big deal but this is important. On any other map you will get an error message. To set the map to 100px: menu --> map --> edit map --> set 'pixels per cell' to '100'. 
	
	THATS IT!
	
	Now you can delete the Inn Generator Map from your campaign file
	Keep in mind that the InnStants can ONLY construct the Inn while the Inn generator Map is in your campaign file!!
This because it needs the assets on that map (floor, table, bar, lights, pillar, etc.) as these are only present on that map. After you constructed the Inn(s) you can safely delete the Inn Generator Map.
	
	
	
		GENERATING A NEW INN
	
	Just hit the Generate Inn button go through the settings and hit ok.
	
	Alternatively you can construct an Inn step by step by hitting the following macros:
	0. Clear Map
	1. Setup Choices
	2. Construct Floor
	3. Raise Walls
	4. Place Bar
	5. Add Features
	6. Move Tables
	7. Invite Patrons
	8. Add Dividers
	9. Create Innstant
	
	Each stage you can hit the macro multiple times to cycle through different renderings until you hit one you like
	That means you can also generate an inn and if youre not happy about e.g. the floor you can hit the 'construct floor' button to create a new one without resetting the rest.
	Note that when you are done you have to hit the 'create innstant' one more time to update it with the last changes. 
	
	
	ADDING ASSETS
	Lets take floor tiles as example. 
	You want to add 3 'common' 'scifi' floor tiles. 
	1. Drag the images onto the map (TOKEN layer)
	2. Select an existing 'common' 'scifi' floor tile already on the map (this is used to get the name from) and select the new image. Hit the blue macro: 'Rename Auto' (group: 'Naming Tools')
	3. You get a popup with the correct name for the assets (check this). Make sure the setting and quality are correct. Hit ok. 
	4. Check if the numbering is correct, if not: select ALL the 'common' 'scifi' floor tiles and hit the yellow 'Renumber Assets' macro. 
	5. When youre done with adding all the new assets you want to add: hit the gray (with red):'buildAssetDB' macro. 
	
	
	ADDING NEW SETTING OR QUALITY
	Keep in mind that if you add a new quality this applies to ALL the settings, so you'll need quite some assets! However if the asset required does not exist the generator automatically check 'neighbouring' assets and if all fails it will revert to 'Common' 'Fantasy' asset.
	
	If you want to add a new setting (quality works EXACTLY the same) you pick one asset (image) on the map (doens't matter which one) e.g. 'Dancefloor_Wall_Fantasy_Poor__1' and change the setting (in this case 'Fantasy') to the new setting e.g. 'Western' so you get: 'Dancefloor_Wall_Western_Poor__1'. The only thing that is important (next to the new setting) is the number '1'. Make sure its 1. 
	Then hit the 'Update Asset Database' macro.
	You have now added a new setting. Obivously you'll need to add all the relevant assets (images) to the map to make this work. And as said: if an asset does not exist the generator will FRIST check if theres a 'common' asset of that setting (so make sure you start with the common assets) and if that fails it will pick a 'common' 'fantasy' asset in its stead. So its not vital to have the entire asset setting collection complete. 
	The new setting will automatically be added to the generator options. 
	To check the 'completeness' of your set (and to get an idea of which assets are required) you can run macro: 'Show Asset Database'. Alternatively theres a green 'Check Complete' macro (in the naming tools) which simply ports the lot to the chat. 
	

	TOOLS
	Some additional tools at your disposal
	
	SIZE TOOL
	That concerns the entire '55. adjust token size' macro group. Just select all the assets you want to resize and hit the blue buttons (W=Width; H=Height; white buttons do nothing). 
	
	NAME GENERATOR
	This concerns macro group 60. Name generator. There are two buttons you can use:
	1. Random Inn: provides a name for you Inn
	2. Random Name: provides a random name for the chosen gender and race. Both are fairly basic but help for a quick fix. 
	If you feel upto it: in  'NameData' contains the name part database, you can update that with stuff you like. 

