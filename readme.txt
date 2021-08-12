To update prices in DPS calc:
take json from:
https://prices.runescape.wiki/api/v1/osrs/1h
Clean it with:
https://jsonformatter.curiousconcept.com/#
regex edit:
https://regex101.com/

Find and replace/l
(?:")([1-9]|[1-9][0-9]|[1-9][0-9][0-9]|[1-9][0-9][0-9][0-9]|[1-9][0-9][0-9][0-9][0-9])(?:":{)

Also delete:
""data":{"
format should look like {{groups of items}}

Replace:
 outer {} with []

Edit the API Json file:
https://github.com/An0rakX/osrsAPI/edit/main/API.json
