#### Modpackgression
|         No Tree Punching         |          <          |          <           |         <         |           <            |
|:--------------------------------:|:-------------------:|:--------------------:|:-----------------:|:----------------------:|
|          Tinkers Stuff           |          <          |          <           |         <         |           <            |
|      Immersive Engineering       |     Small Ships     |       Botania        |    Ars Noveau     | Blood Magic/EvilCraft  |
|         Mekanism/EnderIO         |          ^          |          ^           |         ^         |           ^            |
|            JEG/Warium            | Immersive Aircraft  |          ^           | Mana and artifice | Vampirism + Werewolves |
|  Steves Minecarts/Computercraft  | Immersive Machinery |          ^           |         ^         |       Occultism        |
| Immersive Petroleum/Nuclearcraft |    Alex's Caves     |          ^           |         ^         |           ^            |
|             Ad Astra             |          ^          |          ^           |         ^         |           ^            |
|                ^                 |         <->         |    Mythic Botany     |  Twilight Forest  |           ^            |
|                ^                 |         <->         |          ^           |      Aether       |         Nether         |
|               AE2                |          <          |          ^           |   Mahou Tsukai    |           <            |
|           Ex Machinis            |          <          | Mystical Agriculture |         <         |           <            |
|               Psi                |          <          |          ^           |         <         |           <            |
|             ProjectE             |          <          |          <           |         <         |           <            |
|             Kill God             |          <          |          <           |         <         |           <            |
|         Just Dire Things         |          <          |          <           |         <         |           <            |
|             Morph???             |          <          |          <           |         <         |           <            |
|          Godhood Finale          |          <          |          <           |         <         |           <            |
	
#### TO-DO
- [x] Proximity VC
- [ ] desh for the psi and dyson sphere
- [x] Iron + Lead = Raw Gun Metal
- [ ] Tesla Unit for wireless stuff
- [ ] remove stronghold + end dragon
- [x] I WANNA HAVE CHILDREN WITH HOT VAMPIRES
- [ ] Custom Game Intro
- [ ] Custom Video Endings
- [ ] Sentient tinkers constructs items
- [ ] Ally with Pillagers
- [ ] Villager Refugees
- [ ] Add god
- [ ] Gaiss Recipes for both Light and Dark magic
- [ ] Add weird funky Wither-Wither-Tentacle to The Midnight
- [x] One day butchery won't have buggy armour stands
- [ ] Use OEI to Reduce Pain for EVERYONE
#### Lore
- Steve Kills enderdragon but dies to wither
- Wither becomes funky so Alex puts it in The Midnight
- Light and Dark magic were buddies but broke off causing the schism (explains why botania and occultism shares resources for starting them)
- Tech is a rebellion of both and broke off due to schism
- Tech leads to a world war-esque scenario
- Tech becomes Sci-Fi
- Light and Dark magic mend schism due to and turn into Oriental magic (name pending) (Gaiss gives freedom for magicians to have custom allegiances)
- Oriental magic achieve infinite resources with mystical agriculture
- Sci-Fi becomes buddies with Oriental magic bcuz infinite resources (ProjectE is made as a result)
-  smthng smthng juiced up wither is in glacio or smthng
-  JRPG Kill god (refer to Endings)
#### Endings
- Ragnvaldr
- Enki
- Cahara
- Family
- Harem
- Atomwaffen
-  JRPG Kill god (refer to Lore)

#### Maybe helpful code snippets
```
LootJS.modifiers((event) => {
    event.addLootTypeModifier(LootType.ENTITY).removeLoot("minecraft:flint");
});
// priority: 0

// Visit the wiki for more info - https://kubejs.com/

console.info('Hello, World! (Loaded server scripts)')

ServerEvents.recipes((event) => {
	event.recipes.occultism.spirit_trade('minecraft:rotten_flesh', 'minecraft:bone')
	event.recipes.occultism.spirit_fire('minecraft:emerald_ore', '#forge:gems/emerald')
	event.recipes.occultism.crushing(
		'2x #forge:ores/iron',
		'#forge:tools/swords'
	)
	event.recipes.occultism.miner(
		Item.of('minecraft:wooden_pickaxe').withChance(100),
		'#occultism:miners/master'
	)
	event.recipes.occultism.ritual(
		'occultism:spirit_lantern',
		[
			"lapis_lazuli",
			"#forge:raw_materials",
			["minecraft:coal", 'minecraft:charcoal'],
		],
		'#forge:stone',
		'occultism:craft_afrit'
	).dummy("kubejs:dummy_ritual_thing").useItem('minecraft:egg')
})
```
