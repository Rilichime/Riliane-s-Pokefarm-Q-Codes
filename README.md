# Riliane's Pokefarm Q Codes

A monorepo for Pokefarm Q code.

## PFQ Automatic Breeding Pair Matchmaker

Logs the Pokemon in your fields upon opening the individual field. (Note: Requires refresh / waiting 5s for the script to update.)
Then, when viewing another user's field, it will display breeding pair matches.
Matching function pairs individuals of opposite sex that are of the same evolution line and nature.

Features:
- UI panel on your fields page and other user's pages.
- Also shows any Pokemon you have less than 8 of.
- Shows a log of Pokemon on your fields page, with a delete button for each field.

Notes:
- If a field name is changed, you will need to manually delete the data from the old field's name and refresh the page while viewing the field to log the new info.
- If you change the Pokemon in your fields, you will need to refresh the page while viewing the fields changed for the script to log the changes.
- Evolution mapping feature means evolutions are paired with previous forms.
- Formes are considered when matching, so regional variants and PFQ variants are not paired with their original counterparts. However, this means certain Pokemon will not be matched if their forms are different, e.g. Burmy, Cramorant, Eiscue.
- The script does not take OT into account, so you will still need to check that.
- Disable the script if you don't want the UI to show.

## PFQ Market Logger

Logs sold data for items viewed in the market and provides a chart for tracking trends over the last 6 months.

Note that this script is only capable of logging what is viewed, so you have to load each item you want to track, and it will only track the last 10 items sold. But it will keep all data collected, so you can view more than the last 10 provided you have logged it before.

Chart may be changed later because I feel iffy about it. Not sure what I want it to do yet.

Features:
- Ability to add notes to individual sales. Mostly, this is intended to note down things that affect prices like "Evolution Tournaments" for evo stones, or "Type Race", or "Halloween Event" and so on.
- Script runs every 3s. UI will show the most recently selected item.
- Shows when you last scanned prices for each item when viewing a marketboard category.
- Check boxes to optionally ignore data points when viewing the chart. This is mainly intended to be used to filter out unusually low sales (e.g. 99 items being sold for 1 credit).
- Entire panel can be collapsed with the hide button, and re-enabled with a small show button.
- Options to export data in a CSV file to back up data or share it with other users, and options to upload CSV files to import data. Uploaded data will combine with already existing data. Duplicate entries should not be an issue.

Notes:
- Rounds prices to the nearest 1k or for items over 1 mil, to the nearest 100k.

# Deprecated Codes

## PFQ Pokémon Info Extractor
This is a Tapermonkey userscript. It's purpose is to list the Pokemon in a field. It will output the Pokemon's base species, forme, gender, nature, and link in the console.

This information can be accessed by pressing F12 and clicking the console tab.

Information will be exported in the following format.

> Species: Kecleon,  Gender: M,  Nature: Rash,  Forme: N/A,  Link: https://pokefarm.com/summary/Nb94f

## PFQ Console Filter
This is a Tapermonkey userscript. It's purpose is to identify Pokemon of specified base species, forme (optional), and gender (optional). It will output the Pokemon's base species, forme, gender, nature, and link in the console.

This information can be accessed by pressing F12 and clicking the console tab.

Information will be exported in the following format.

> Species: Kecleon,  Gender: M,  Nature: Rash,  Forme: N/A,  Link: https://pokefarm.com/summary/Nb94f

## PFQ Genders Needed
HTML with CSS, and Javascript. Utilized on my [Wix site](https://digitalxdaydreamz.wixsite.com/rilianepfq/genders-needed).

Input Pokemon in the following format.

> Species: Kecleon,  Gender: M,  Nature: Rash,  Forme: N/A,  Link: https://pokefarm.com/summary/Nb94f

Adjust the numbers as needed (default is 7 males, 7 females). 

This tool will list any missing Pokemon, as well as any Pokemon that have less than the chosen number of males/females, along with the number needed.

For example:

> { species: 'Diglett', gender: 'M' }, // need 2 male

> { species: 'Meowth', forme: 'Galarian Forme' }, // need 5 male, 6 female

The output format can be directly copy-pasted into the PFQ Console Filter.

## PFQ Matchmaking

HTML with CSS, and Javascript. Utilized on my [Wix site](https://digitalxdaydreamz.wixsite.com/rilianepfq).

Input Pokemon in the following format.

> Species: Kecleon,  Gender: M,  Nature: Rash,  Forme: N/A,  Link: https://pokefarm.com/summary/Nb94f

This tool is used to find breeding pair matches. It pairs males with females of the same base species and nature.

It outputs the information like so:

> Match found for Species: stunfisk, Nature: timid, Forme: galarian forme.
> 
> Link to Part A Pokémon: https://pokefarm.com/summary/r8kXs
> 
> Link to Part B Pokémon: https://pokefarm.com/summary/lKSxh

Note you will still need to verify that the OT's are different for the Pokemon to make an 80% pair.








