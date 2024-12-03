# Riliane's Pokefarm Q Codes

A monorepo for Pokefarm Q code.

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
HTML with CSS, and Javascript. Utilized on my [Wix site](https://digitalxdaydreamz.wixsite.com/rilianepfq/genders-needed)

Input Pokemon in the following format.

> Species: Kecleon,  Gender: M,  Nature: Rash,  Forme: N/A,  Link: https://pokefarm.com/summary/Nb94f

Adjust the numbers as needed (default is 7 males, 7 females). 

This tool will list any missing Pokemon, as well as any Pokemon that have less than the chosen number of males/females, along with the number needed.

For example:

> { species: 'Diglett', gender: 'M' }, // need 2 male

> { species: 'Meowth', forme: 'Galarian Forme' }, // need 5 male, 6 female

The output format can be directly copy-pasted into the PFQ Console Filter.

## PFQ Matchmaking

HTML with CSS, and Javascript. [Wix site](https://digitalxdaydreamz.wixsite.com/rilianepfq)

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








