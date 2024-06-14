# Helldivers 2 Data Dump
 Datamining for Helldivers 2, supporting the guts of https://helldivers.io/ and others. 
 
 Review the data in an easy frontend @ https://data.helldivers.io/
# Tutorial on how to get planet effects:
 - Go to https://data.helldivers.io/?settings=generated_planet_data
 - Click the planet you want (i.e. Hellmire) https://data.helldivers.io/?settings=generated_planet_data&index=36
 - .gameplay_modifiers will have references to id's if any are available. https://data.helldivers.io/?id=9189059319917937722
 - Check the environmental effect tag https://data.helldivers.io/?id=9189059319917937722&component=EnvironmentalEffectTag
 - EnvironmentalEffectType_IntenseHeat should display, repeat for any other gameplay_modifiers
# Tutorial on how to translate planetInfos from the api server response:
 - Go to https://api.live.prod.thehelldiversgame.com/api/WarSeason/801/warinfo, check planet info, make note of settings hash (i.e. 897386910)
 - Make a map of murmur2 hashes, of the debug_name's (can be seen from https://data.helldivers.io/?settings=generated_planet_data&index=36  (note... sometimes you ignore the actual debug name and just use the index... dunno why)
 - https://helldivers.io/murmur/planet_000 planet_000 has a 32bit murmur hash of 897386910
 - Then map planet_000 to the index of the planet settings @ https://data.helldivers.io/?settings=generated_planet_data
# Why doesn't weapon data seem accurate?
 The WeaponCustomizations component overrides some data, including projectile type and magazine size.
# Leaks?
 I do not support leaks. Please refrain from spreading them. The game devs are getting better at not including unreleased content in the game, but some still exists.
# Hiring a security engineer?
 Drop me an email - shalzuth @ gmail
# Legal stuff
 This project isn't endorsed by Arrowhead Game Studios or Sony Interactive Entertainment. and doesn’t reflect the views or opinions of Arrowhead Game Studios or Sony Interactive Entertainment or anyone officially involved in producing or managing Arrowhead Game Studios or Sony Interactive Entertainment. Game content and materials are trademarks and copyrights of Arrowhead Game Studios or Sony Interactive Entertainment.