# Ryujinx Games Compatibility List

Anyone be free to update or share his results here. But you need to follow some advices to get them validate.
When you update or add some feedback, please, be much precise as possible, don't forget to enable `Logging_Enable_Debug = true` in the conf file of Ryujinx. In your pull request, add some lines of the logs, some screenshots, or anything usefull to get your result validate. (We can't just trust you by words. Sorry!)

Thanks.

## Folder structure

A folder is equal to a tested game. It's named like that `new-amazing-ryu-games-supported`, not number, not extra chars, just text with spaces replace by `-`. For now, there are 3 files in this folder:

* **boxart.png**

   Who is a picture of the game boxart in PNG format (only!!). Please use a clean picture, without hudge size, and cropped. (A standard size will be probably determined later.)

* **info.json**

   It's a JSON file who contain specific fields (Don't forget to remove comments if you Copy/Paste)
   
```javascript
 { 
	"title_id": 
	[ 
		"0100000000000000", // Game title ids who can be found on swithbrew or in your gamedump too.
		"0100000000000001", // You can add more of them if game is multi region.
		"0100000000000002", // Or if there is an update of the game.
		"etc..."
	],
	"name": "Cave Story+",           // Game name in clean version (folder name is a raw version).
	"state": "In Game",              // Current state of the game, be revelant here.
	"state_emu_version": "7ac5f40",  // Last Ryujinx commit of your current executable version (for now).
	"state_last_date": "19/05/2018", // Date of your test.
	"comment": "Explain what going on here." //Be more precise as possible.
}
```

* **screenshot.png** (Optionnal)

   Who is the Ryujinx in-game full screenshot in PNG format (only!!). Please use a clean picture, sized at 1280px x 720px (or around). If the game don't show anything in the emulator, please don't provide anything for this file. The `boxart.png` is used instead of this one.