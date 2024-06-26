# Real U.S. Radio mod for American Truck Sim.

### Get it on Steam: [Workshop](https://steamcommunity.com/sharedfiles/filedetails/?id=3211499388) | [Guide](https://steamcommunity.com/sharedfiles/filedetails/?id=975427716)

Hello! Here are some radio stations formatted for American Truck Simulator.  

When I bought ATS I found the in-game radio pathetic. There were less than 40 streams added by “update from internet” in-game so I started looking for more streams on my own. Initially, this was just a list of a few radio stations I listen to daily but now includes over 360 radio streams. Most of these stations are U.S. based, but the list also now covers Canada and includes national programming. Each URL is a publicly available radio stream I gathered from the internet myself using an internet browser’s network traffic monitor (F12).  

## Update, 1 Apr 2024:
-	The list is updated, removing and replacing many dead stream URLs. Every stream has been tested and all currently work.  
-	Over 100 more stations are added, bringing the total to 361 stations with over 300 of those being geographically-based stations.  
-	The list now includes a minimum of 3 stations from each of the 50 U.S. states and all 10 provinces of Canada.  
-	The non-English selection has been expanded, with 18 Spanish stations, 7 French stations, and even Chinese and Native American language streams.  
-	There are 57 non-geographic streams made up of national programs, TV simulcast, and a small selection of web-based RFC streams.  
-	Bitrate has been replaced. Instead, the streams can now be arranged alphabetically by location using the “bitrate” column. All streams from Alabama have a listed bitrate of 1, all streams from Alaska have a listed bitrate of 2, and so on for every state. The Capitol, Washington D.C., is listed as 51 and non-location based streams are 52. The 10 provinces of Canada are 53 through 62.  

# How to Use

## Option A
1.	Download my live_streams.sii file [available here](https://github.com/GabeValentine/ATS_Real_US_Radio/releases/tag/Release)  
2.	Place this file in \Users\YOU\Documents\American Truck Simulator.  
3.	Overwrite old file and enjoy. WARNING: This will overwrite any other custom stations you have added.  
4.	(optional) Open ATS and select radio. Click "update from internet" to add default stations.  

## Option B (Merge Custom Stations)
1. Download my live_streams.sii file [available here](https://github.com/GabeValentine/ATS_Real_US_Radio/releases/tag/Release)
2. Locate your live_streams.sii file, located in \Users\YOU\Documents\American Truck Simulator.
3. Open both files in Notepad++ or similar program and copy whichever has less entries to the file that has more entries.
4. Change stream number to be unique for each line (if last entry was 360, new stations start at 361).
5. Save finalized file in \Documents\American Truck Simulator and enjoy.

## Option C (Only on Github)
1. Browse the stream_data lists to find the stations you would like to import:  
[All by Genre](https://github.com/GabeValentine/ATS_Real_US_Radio/blob/main/All%20by%20Genre.md)  
[U.S. by State](https://github.com/GabeValentine/ATS_Real_US_Radio/blob/main/U.S.%20By%20State.md)  
[National U.S. Programming](https://github.com/GabeValentine/ATS_Real_US_Radio/blob/main/National%20Streams.md)  
[Canada by Province](https://github.com/GabeValentine/ATS_Real_US_Radio/blob/main/Canada%20by%20Province.md)  
2.	Locate your live_streams.sii file, located in \Users\YOU\Documents\American Truck Simulator.  
3.	Open with Notepad++ or similar program.  
4.	Copy entries from my list to the end of the file.
5.	Change stream number to be unique for each line (if last entry was 234, new stations start at 235).  
6.	Save file and enjoy.  

## Tips:  
- Don't worry about sorting! The game will rearrange the list when you sort stations in-game, so don't waste your time.  
- Don't worry about first few lines of code (live_stream_def and number of streams). You can change them manually but ATS updates them automatically when you launch the radio.  
- You can replace any existing entry (for example, non-working streams) without problem.  
- ATS can be running when you edit live_streams.sii. Game will re-check file each time you click "radio" in-game.  
- A couple stations do not broadcast 24/7. They're not dead, just sleeping. If you do notice consistent problems with a specific station, let me know in the comments and it will be replaced.  
- You can leave an entry blank; ATS will add dividers and set bitrate 0 when you sort in-game. Example:  
 stream_data[111]: ""  
 stream_data[111]: "|||0|0"  

# How to Read ATS Formatting
Every link should be formatted like this:  
 stream_data[Number]: "URL|Name|Genre|Language|Bitrate|Favorite"  
- Number is unique stream id number, used by the game to organize the list. These must be sequential starting with 0.  
- URL is a direct link to the stream and can be tested in web browser. Watch out for dividers!  
- Name is in-game description of station. I use the following format: call sign, branding and/or info (such as HD# or station affiliation), frequency & band, then location.  
- Genre can be changed for organizing preferences. I use the genre listed on each station’s Wikipedia page or directly in stream metadata.  
- Language is ISO two-letter code (639-1). The list currently includes English (EN), Spanish (ES), French (FR), Chinese (ZH), and Cree (CR) language streams.  
- Bitrate is not bitrate anymore! I have replaced this with an “alphabetical by location” filter.  
- Favorite is boolean, 0 or 1.  
