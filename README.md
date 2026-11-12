# skyrim-ae-visual-immersion-guide
A vanilla-friendly Skyrim Anniversary Edition modlist focused on visuals, atmosphere, animations and immersion. Includes the complete mod list, MO2 installation order, DynDOLOD setup and DLSS configuration. Original gameplay preserved.
Skyrim Anniversary Edition — Vanilla-Friendly Visual & Immersion Modlist

1. Introduction

This guide covers my personal Skyrim Anniversary Edition setup. The goal is to improve the original game’s graphics, atmosphere, environments, animations and audio while keeping Skyrim recognizably Skyrim.

This is not a gameplay overhaul. The original combat system, progression, quests, balance and general gameplay are preserved.

The setup focuses on:

* Improved textures, meshes and environmental details.
* Better mountains, trees, grass, landscapes and water.
* More atmospheric weather, lighting and interiors.
* Improved character, creature and weapon visuals.
* More natural movement and additional animations.
* Enhanced ambient sounds, footsteps, weather and shouts.
* Distant object and landscape detail through DynDOLOD.
* Optional DLSS and Frame Generation.

The visual direction is realistic and atmospheric, but still faithful to Skyrim’s original art style. No anime-style character overhauls or major gameplay changes are required.

Important: This is my actual mod setup, not a universal compatibility list. Mod versions, requirements and patches can change. Always read the current Nexus Mods description and requirements before installing a mod.

⸻

2. My PC and game version

Game: The Elder Scrolls V: Skyrim Anniversary Edition (Steam)
Game runtime: 1.7.104.0
Mod manager: Mod Organizer 2
GPU: NVIDIA GeForce RTX 4050 Laptop GPU
RAM: 16 GB
Laptop: MSI Katana 17

My observed performance is approximately 90–110 FPS with DLSS enabled. This is my personal result on my hardware, not a guaranteed benchmark for other systems.

⸻

3. Required tools

Before installing mods, prepare the following:

1. Skyrim Anniversary Edition from Steam.
2. Mod Organizer 2 (MO2).
3. SKSE64, matching your exact Skyrim runtime.
4. LOOT, for sorting plugins.
5. 7-Zip, for extracting archives.
6. DynDOLOD Standalone, for generating distant details.

Useful websites:

* Mod Organizer 2: https://www.modorganizer.org/
* MO2 on Nexus Mods: https://www.nexusmods.com/site/mods/6
* Nexus Mods: https://www.nexusmods.com/skyrimspecialedition
* SKSE: https://skse.silverlock.org/
* LOOT: https://loot.github.io/
* DynDOLOD documentation: https://dyndolod.info/

Do not install MO2 inside the Skyrim game directory. Keep your modding tools, downloads and game files organized in separate folders.

⸻

4. Installing Mod Organizer 2

1. Download and install Mod Organizer 2.
2. On the first launch, choose Create a portable instance.
3. Select Skyrim Special Edition. Anniversary Edition uses the Special Edition version of the modding tools.
4. Choose a location with enough free disk space.
5. Connect MO2 to your Nexus Mods account.
6. Allow MO2 to handle Nexus download links when prompted.
7. Select the correct Skyrim installation when MO2 asks for the game location.

A portable instance keeps its modding data together, making it easier to manage and back up.

My own MO2 instance is located at:

E:/Modding/MO2

You can use another drive or folder. Just make sure there is enough free space for downloads, installed mods and generated files.

Understanding the MO2 interface

MO2 has two important lists:

Left panel — Mod priority

This controls which installed mod’s files take priority when multiple mods provide the same file.

A mod lower in the left panel generally wins file conflicts against a mod above it.

Right panel — Plugin load order

This controls the order in which ESP, ESM and ESL plugins are loaded by the game.

These are two different things. A mod can appear in the left panel without having a plugin in the right panel.

Do not confuse the two lists.

⸻

5. Installing SKSE and essential mods

Download SKSE from its official website. Make sure the version matches your installed Skyrim runtime.

For Skyrim runtime 1.7.104.0, use a compatible SKSE64 release.

Follow the SKSE installation instructions carefully. The loader and required files must be installed in the correct locations.

After installing SKSE:

1. Open MO2.
2. Add skse64_loader.exe as an executable if MO2 has not detected it.
3. Select SKSE in the executable dropdown.
4. Launch the game through MO2 using SKSE.
5. Confirm that the game starts correctly.

Do not launch the modded game through the normal Skyrim launcher after completing the setup.

Essential framework mods

These are part of my setup:

* Address Library for SKSE Plugins
* SkyUI
* powerofthree’s Papyrus Extender
* EngineFixes
* SSE Display Tweaks
* Open Animation Replacer
* Animation Queue Fix
* Paired Animation Improvements
* Faster HDT-SMP
* SKSE Menu Framework

Always install the requirements listed on each mod’s Nexus page. Some SKSE plugins require a particular game runtime or Address Library version.

⸻

6. Installing mods from Nexus Mods

The general installation process is the same for most mods:

1. Open the mod page on Nexus Mods.
2. Read the description and requirements.
3. Open the Files tab.
4. Download the correct file using Mod Manager Download when available.
5. Wait for the download to appear in MO2’s Downloads tab.
6. Double-click the downloaded archive.
7. Check the installation options if an installer appears.
8. Finish the installation.
9. Make sure the mod is enabled in the left panel.

Some mods require manual installation or additional configuration. Follow their individual instructions.

File conflicts

When MO2 displays a lightning-bolt icon, it means that files are being overwritten.

This is not automatically an error. Texture replacers and mesh improvements are expected to overwrite some files.

The important thing is to understand which mod should win the conflict.

Do not blindly resolve every conflict by choosing one mod over another. Follow the intended priority of your setup and the instructions from the mod authors.

⸻

7. My complete MO2 left-panel order

The following is the actual left-panel priority order from my working setup.

This is the final priority order, not a requirement to download every mod in precisely this chronological sequence. Install requirements first, then arrange the left panel to match the list.

The order matters because lower entries can overwrite files from higher entries.

Essential mods and animation frameworks

1. Address Library for SKSE Plugins
2. SkyUI
3. powerofthree’s Papyrus Extender
4. EngineFixes
5. SSE Display Tweaks
6. Open Animation Replacer
7. Animation Queue Fix
8. Paired Animation Improvements
9. Vanargand Animations - Male Idle Walk and Run — superseded entry in my original list; do not install this old entry if using its replacement
10. Vanargand Animations II - Female Idle Walk And Run
11. Vanargand Animations II - Sprint
12. Vanargand Animations - One Handed Normal Attacks
13. Vanargand Animations - One Handed Power Attacks
14. Leviathan Animations - Two-Handed Normal Attacks
15. Animation Motion Revolution - Skyrim 1.7.104.0 Update
16. Leviathan Animations - Two-Handed Power Attacks
17. Vanargand Animations - Archery
18. Goetia Animations - Magic Spell Casting
19. NPC Animation Remix (OAR)
20. Comprehensive First Person Animation Overhaul - CFPAO
21. Immersive Diving Animation
22. EVG Animated Traversal
23. Stronger Swimming Animations SE
24. SD’s Seamless Sneak Transition and Idles OAR
25. Take a Seat - New Sitting Animations for OAR or DAR
26. Faster HDT-SMP

DLSS and Frame Generation

27. Theo’s Render Pipeline - DLSS - FrameGen
28. Theo’s Render Pipeline - DLSS - Frame Gen - Neural Rendering
29. SKSE Menu Framework

Main textures, meshes and environmental visuals

30. Static Mesh Improvement Mod
31. Project Clarity AIO - Skyrim Textures Redone
32. Skyland AIO
33. CC’s HD Dwemer Automatons - Remastered
34. Skyland Bits and Bobs - A Clutter Overhaul
35. SLOPPY Spider Webs
36. Skeleton.and.Human.Bones.by.Kajuen
37. Simply Skin - Female Texture Replacer
38. Simply Skin - Male Texture Replacer
39. Vanilla hair - Salt and Wind
40. Vanilla hair remake
41. Vanilla hair remake SMP
42. Majestic Mountains Main
43. Simplicity of Snow
44. Embers XD
45. Happy Little Trees
46. Skoglendi - A Grass Mod
47. Cathedral - 3D Mountain Flowers
48. Landscape Fixes For Grass Mods
49. Water for ENB
50. Natural Waterfalls
51. Natural Waterfalls - Majestic Mountains Patch

Weather, lighting and Community Shaders

52. Cathedral Weathers and Seasons
53. Cathedral Weathers and Seasons - Brighter Nights
54. Relighting Skyrim SE
55. Luminosity Lighting Overhaul - The Cathedral Concept
56. Community Shaders
57. Upscaling - Community Shaders
58. Wetness Effects - Community Shaders
59. Hair Specular - Community Shaders
60. Skylighting - Community Shaders
61. Screen Space Global Illumination (SSGI) - Community Shaders
62. Terrain Blending - Community Shaders
63. Grass Optimizations - Community Shaders
64. Interiors Fix Temporary — personal temporary component from my setup; not a standard public requirement for this guide

Creatures, equipment and effects

65. Cathedral - Armory
66. Bellyaches Animal and Creature Pack Revamp
67. Bellyaches 16K-8K Dragon Replacer Pack
68. Draugr.by.Kajuen
69. Falmer.by.Kajuen
70. Skyrim Food Expansion
71. Common Clothing Retexture SE
72. Next Gen Dragon VFX
73. Deadly Spell Impacts
74. Flame VFX Edit

JK’s Skyrim and interior collection

75. JK’s Skyrim
76. JK’s Dragonsreach
77. JK’s Blue Palace
78. JK’s Palace of the Kings
79. JK’s Mistveil Keep
80. JK’s Castle Dour
81. JK’s Understone Keep
82. JK’s The Bannered Mare
83. JK’s The Bee and Barb
84. JK’s Candlehearth Hall
85. JK’s The Winking Skeever
86. JK’s Silver-Blood Inn
87. JK’s Sleeping Giant Inn
88. JK’s The Ragged Flagon
89. JK’s The Drunken Huntsman
90. JK’s Warmaiden’s
91. JK’s Arcadia’s Cauldron
92. JK’s Belethor’s General Goods
93. JK’s Radiant Raiment
94. JK’s White Phial
95. JK’s Elgrim’s Elixirs
96. JK’s Angeline’s Aromatics
97. JK’s Bits and Pieces
98. JK’s Riverwood Trader
99. JK’s Arnleif and Sons Trading Company
100. JK’s Haelga’s Bunkhouse
101. JK’s New Gnisis Cornerclub
102. JK’s Nightgate Inn
103. JK’s Sadri’s Used Wares
104. JK’s Temple of Dibella
105. JK’s Temple of Kynareth
106. JK’s Temple of Talos
107. JK’s Temple of the Divines
108. JK’s The Temple of Mara
109. JK’s The Hag’s Cure
110. JK’s The Pawned Prawn
111. JK’s Interiors Patch Collection
112. JK’s Skyrim - Towns

Encounters and audio

113. Extended Encounters
114. NPCs Ain’t Hachikos
115. Immersive Patrols SE AE
116. Immersive Patrols SE AE - Russian Translation
117. Sound Record Distributor
118. Acoustic Space Improvement Fixes
119. Audio Overhaul for Skyrim (4.1.2)
120. Ash Footsteps Fixed for Skyrim Audio Overhaul
121. Immersive Sounds - Compendium
122. Immersive Sounds Compendium Drinking Sound Fix
123. Audio Overhaul - Immersive Sounds Integration (AOS - ISC Compatible)
124. Regional Sounds Expansion (SRD - Wilds Dungeons Towns Ambience)
125. Reverb Interior Sounds Expansion
126. Thundering Shouts
127. Authentic Wolf Howls and Aggro
128. Nordic Winds

DynDOLOD resources and generated output

129. DynDOLOD Resources SE
130. DynDOLOD DLL NG
131. TexGen Output New
132. DynDOLOD_Output New

Important notes about this list:

* The superseded Vanargand male animation entry is shown because it appeared in my original list. It is not a required active mod when using its replacement.
* Interiors Fix Temporary is a personal temporary component, not a public dependency that every reader should search for.
* TexGen Output New and DynDOLOD_Output New are generated files, not ordinary Nexus downloads. Their creation is explained below.
* Some mods in this setup have optional files and patches. Install only the options appropriate for your game and installed mods.

⸻

8. Visual improvements

Textures and meshes

The main visual foundation consists of:

* Static Mesh Improvement Mod (SMIM)
* Project Clarity AIO
* Skyland AIO
* Skyland Bits and Bobs
* CC’s HD Dwemer Automatons
* SLOPPY Spider Webs
* Skeleton and Human Bones by Kajuen

SMIM improves many of Skyrim’s original 3D objects. Project Clarity and Skyland replace large portions of the original textures.

Together, they improve the appearance of buildings, clutter, architecture, dungeons and the general environment without changing the overall visual identity of the game.

Mountains, grass and trees

* Majestic Mountains
* Happy Little Trees
* Skoglendi
* Cathedral - 3D Mountain Flowers
* Landscape Fixes For Grass Mods
* Simplicity of Snow

These mods improve the natural environment and make the landscape feel more detailed.

Landscape Fixes For Grass Mods is particularly important when using grass mods alongside edited locations. Make sure to install the relevant patches for your setup.

Water and waterfalls

* Water for ENB
* Natural Waterfalls
* Natural Waterfalls - Majestic Mountains Patch

These improve water appearance and waterfall visuals.

Read the requirements and optional patch descriptions carefully. Water mods often have specific compatibility patches for other landscape and location mods.

Weather and lighting

* Cathedral Weathers and Seasons
* Cathedral Weathers and Seasons - Brighter Nights
* Relighting Skyrim SE
* Luminosity Lighting Overhaul

The goal is to improve atmosphere, lighting and weather while retaining the original feel of Skyrim.

Community Shaders

Community Shaders is the main shader framework in this setup.

Additional modules used:

* Upscaling
* Wetness Effects
* Hair Specular
* Skylighting
* Screen Space Global Illumination
* Terrain Blending
* Grass Optimizations

Community Shaders has its own requirements and configuration options. Install the framework first, then add compatible modules.

Do not assume every shader module is suitable for every GPU. Test the game after adding modules and disable individual effects if performance becomes unacceptable.

⸻

9. Character, creature and equipment visuals

The character setup intentionally avoids major face overhauls.

Mods used:

* Simply Skin - Female Texture Replacer
* Simply Skin - Male Texture Replacer
* Vanilla hair - Salt and Wind
* Vanilla hair remake
* Vanilla hair remake SMP

For creatures and equipment:

* Cathedral - Armory
* Bellyaches Animal and Creature Pack Revamp
* Bellyaches 16K-8K Dragon Replacer Pack
* Draugr by Kajuen
* Falmer by Kajuen
* Common Clothing Retexture SE
* Skyrim Food Expansion

These improve character textures, hair, creatures, armor, clothing and everyday objects without turning the game into a completely different visual style.

Vanilla Hair Remake SMP uses hair physics. This does not mean that all clothing or armor in the setup has physics.

⸻

10. Animations and movement

The animation section improves movement while keeping Skyrim’s original gameplay mechanics.

Mods used:

* Open Animation Replacer
* Animation Queue Fix
* Paired Animation Improvements
* Vanargand animation packs
* Leviathan animation packs
* Goetia Animations
* NPC Animation Remix
* Comprehensive First Person Animation Overhaul
* Immersive Diving Animation
* EVG Animated Traversal
* Stronger Swimming Animations
* SD’s Seamless Sneak Transition and Idles
* Take a Seat
* Faster HDT-SMP
* Animation Motion Revolution

These cover movement, attacks, magic casting, first-person animations, swimming, diving, traversal and sitting.

Animation mods can have requirements and conflicts. Install their frameworks and requirements first. Check each mod’s description for the correct version and any required patches.

⸻

11. JK’s Skyrim and interiors

JK’s Skyrim and the associated location mods are a major part of the environment overhaul.

They improve towns, buildings, interiors and important locations throughout Skyrim.

The setup includes JK’s Skyrim, JK’s Skyrim - Towns, and many individual location mods.

Do not install every optional patch automatically.

Only install patches for mods that are actually present in your setup. For example, a patch for Embers XD is not needed if Embers XD is not installed.

The JK’s collection also requires attention to compatibility with other mods that edit the same locations. Read the patch collection’s requirements and compatibility notes.

⸻

12. Audio and atmosphere

The audio setup is designed to make Skyrim feel more alive.

Mods used:

* Sound Record Distributor
* Acoustic Space Improvement Fixes
* Audio Overhaul for Skyrim
* Ash Footsteps Fixed for Skyrim Audio Overhaul
* Immersive Sounds - Compendium
* Immersive Sounds Compendium Drinking Sound Fix
* Audio Overhaul - Immersive Sounds Integration
* Regional Sounds Expansion
* Reverb Interior Sounds Expansion
* Thundering Shouts
* Authentic Wolf Howls and Aggro
* Nordic Winds

These improve ambient sounds, interiors, footsteps, weather, creatures and shouts.

When using Audio Overhaul for Skyrim and Immersive Sounds Compendium together, use the appropriate integration patch. Do not install the integration patch without both parent mods.

⸻

13. LOOT and plugin load order

The right panel in MO2 contains the game’s plugins.

Use LOOT to sort the plugin order:

1. Open MO2.
2. Select LOOT from the executable dropdown if configured.
3. Run LOOT through MO2.
4. Sort the plugins.
5. Review any warnings and missing requirements.
6. Apply the sorted order.
7. Return to MO2 and check that the plugins are enabled.

LOOT is a sorting tool, not a guarantee that every compatibility issue has been solved. Read the mod authors’ instructions and install the required patches.

The following is the plugin order from my setup, after sorting and configuring the installed mods. It is included as a reference for comparing your right panel. Different mod versions or installed options may produce a different order.

My plugin order

1. MajesticMountains_Landscape.esm
2. Cathedral - 3D Mountain Flowers.esp
3. Natural Waterfalls.esp
4. MajesticMountains_Moss.esp
5. Embers XD.esm
6. Natural Waterfalls - Dawnguard.esp
7. Natural Waterfalls - Blackreach.esp
8. JK’s Blue Palace.esp
9. JKs The Drunken Huntsman.esp
10. Natural Waterfalls - Dragonborn.esp
11. EVGAnimatedTraversal.esl
12. DynDOLOD.esm
13. SkyUI_SE.esp
14. SMIM-SE-Merged-All.esp
15. Audio Overhaul Skyrim.esp
16. Immersive Sounds - Compendium.esp
17. AOS_ISC_Integration.esp
18. Project Clarity AIO Half Res Packed3.esp
19. Project Clarity AIO Half Res Packed4.esp
20. Project Clarity AIO Half Res Packed2.esp
21. Project Clarity AIO Half Res Packed1.esp
22. Project Clarity AIO Half Res Packed.esp
23. Project Clarity AIO Half Res Packed0.esp
24. Project Clarity AIO Half Res Packed5.esp
25. Project Clarity AIO Half Res Packed6.esp
26. RelightingSkyrim_SSE.esp
27. JKs Skyrim.esp
28. Landscape Fixes For Grass Mods.esp
29. HappyLittleTrees.esp
30. JK’s Understone Keep.esp
31. JK’s Nightgate Inn.esp
32. JK’s Castle Dour.esp
33. Embers XD.esp
34. MajesticMountains.esp
35. JK’s The Winking Skeever.esp
36. JK’s Temple of the Divines.esp
37. JK’s Arnleif and Sons Trading Company.esp
38. JK’s Mistveil Keep.esp
39. JK’s Haelga’s Bunkhouse.esp
40. JK’s Temple of Mara.esp
41. JK’s Palace of the Kings.esp
42. JK’s Temple of Dibella.esp
43. JK’s The Hag’s Cure.esp
44. JK’s Dragonsreach.esp
45. JK’s Silver-Blood Inn.esp
46. JKs Elgrims Elixirs.esp
47. JK’s Bee and Barb.esp
48. JK’s New Gnisis Cornerclub.esp
49. Lit Road Signs.esp
50. Simplicity of Snow.esp
51. SunDaytimeNorth_MM_default.esp
52. Regional Sounds Expansion.esp
53. Cathedral Weathers.esp
54. cathedralbrighter66.esp
55. Skoglendi - A Grass Mod.esp
56. Generic Grass Limiter.esp
57. Skoglendi - Brown Tundra Add-On.esp
58. Landscape For Grass Mods JK’s Skyrim.esp
59. JK’s Radiant Raiment.esp
60. Reverb Interior Sounds Expansion.esp
61. AcousticTemplateFixes.esp
62. Immersive Patrols II.esp
63. JKs Nightgate Inn - Embers XD patch.esp
64. Landscape For Grass Mods - Military Camps.esp
65. JK’s Riverwood Trader.esp
66. JK’s The Bannered Mare.esp
67. Water for ENB - Patch - Whiterun Waterfalls.esp
68. DeadlySpellImpacts.esp
69. LucaoySDragonVFX.esp
70. Embers XD - Fire Magick Add-On.esp
71. Embers XD - Patch - Survival Mode.esp
72. Embers XD - Patch - Goldenhills Plantation.esp
73. interiorsfixtemp.esp
74. simplicity of splatter.esp
75. smallerfirewoodpileshlt.esp
76. Vanilla hair remake SMP NPCs.esp
77. Natural Waterfalls - Sounds.esp
78. JK’s White Phial.esp
79. JK’s Sleeping Giant Inn.esp
80. JK’s Angelines Aromatics.esp
81. JK’s Temple of Talos.esp
82. JK’s Candlehearth Hall.esp
83. JK’s The Ragged Flagon.esp
84. JK’s Bits and Pieces.esp
85. JK’s Warmaiden’s.esp
86. JK’s Arcadia’s Cauldron.esp
87. JK’s Belethor’s General Goods.esp
88. JK’s Sadris Used Wares.esp
89. JK’s Temple of Kynareth.esp
90. JKs Blue Palace - JKs Skyrim Patch.esp
91. JKs Winking Skeever - Fishing Patch.esp
92. JKs Pawned Prawn - Embers XD Patch.esp
93. JKs Elgrims Elixirs - Bee and Barb Patch.esp
94. JKs Bee and Barb - Embers XD Patch.esp
95. JKs Candlehearth Hall - Embers XD Patch.esp
96. JKs Candlehearth Hall - JKs Skyrim patch.esp
97. JKs Drunken Huntsman - Civil War Champions Patch.esp
98. JKs Elgrims Elixirs - Embers XD Patch.esp
99. JKs Haelgas Bunkhouse - JKs Skyrim Patch.esp
100. JKs Hags Cure - Embers XD Patch.esp
101. JKs Mistveil Keep - Embers XD Patch.esp
102. JKs Palace of the Kings - Embers XD Patch.esp
103. JKs Palace of the Kings - Civil War Champions patch.esp
104. JKs Ragged Flagon - Embers XD Patch.esp
105. JKs Silver-Blood Inn - Embers XD Patch.esp
106. JKs Sleeping Giant Inn - Embers XD Patch.esp
107. JKs Understone Keep - Embers XD Patch.esp
108. JKs White Phial - Embers XD Patch.esp
109. Reverb Interior Sounds Expansion_VolumeSlider_Thunder.esp
110. Reverb Interior Sounds Expansion_VolumeSlider_Rain.esp
111. AcousticTemplateFixes_CC_Farming.esp
112. AcousticTemplateFixes_CC_Seducers.esp
113. Thundering Shouts (normal pitch).esp
114. Nordic Winds.esp
115. AudioOverhaulAshSoundsFixed.esp
116. ISC_drinking_sound_fix.esp
117. Extended Encounters.esp
118. NPCs Ain’t Hachikos.esp
119. DivingJump.esp
120. Water for ENB (Shades of Skyrim).esp
121. Water for ENB - Patch - Calm Water.esp
122. Water for ENB - Patch - Clear Underwater.esp
123. Natural Waterfalls - Water for ENB Patch (Shades of Sk…).esp
124. Luminosity Lighting Overhaul.esp
125. DynDOLOD.esp
126. Occlusion.esp

Note: The list above preserves the plugin names and order from my supplied MO2 list. Some names may be truncated in the MO2 display or differ slightly between mod releases. If your installation has different plugins, do not create empty plugins or rename files to force a match. Use the actual files installed by your mods and let LOOT handle the initial sorting.

⸻

14. Installing and generating DynDOLOD

DynDOLOD improves distant objects and makes the world look more detailed from a distance.

It is not just another mod to download and enable. You must generate files for your own load order.

Required components

* DynDOLOD Resources SE
* DynDOLOD DLL NG
* DynDOLOD Standalone

Install the resources and DLL through MO2, following the official instructions.

Extract DynDOLOD Standalone into a separate tools folder outside the game directory and outside MO2’s mod folders.

Official instructions: https://dyndolod.info/Installation-Instructions

Step 1 — Finalize your load order

Before generating anything:

1. Install the mods you intend to use.
2. Install their required patches.
3. Sort the plugins with LOOT.
4. Resolve missing requirements and compatibility problems.
5. Make sure your tree, grass, landscape and texture mods are enabled.

Do not generate DynDOLOD while you are still changing the major environment mods.

Step 2 — Run TexGen

1. Add TexGenx64.exe to MO2 as an executable.
2. Run TexGen through MO2.
3. Choose an output folder outside the game and mod folders.
4. Use the recommended settings for your setup.
5. Start the generation process.
6. Wait until TexGen completes successfully.
7. Install the generated output as a new mod in MO2.
8. Enable it in the left panel.

In my setup, this generated mod is named:

TexGen Output New

Step 3 — Run DynDOLOD

1. Add DynDOLODx64.exe to MO2 as an executable.
2. Run it through MO2.
3. Select the appropriate options for your load order.
4. Start generation.
5. Wait for the process to finish successfully.
6. Install the generated output as a new mod.
7. Enable it in MO2.

In my setup, this generated mod is named:

DynDOLOD_Output New

The generated output is specific to your installed mods. Do not download someone else’s output and expect it to match your setup.

Step 4 — Check the result

After generation:

* Confirm that the generated mods are enabled.
* Confirm that DynDOLOD plugins are enabled.
* Check for errors in the generation logs.
* Launch the game and inspect distant mountains, trees, buildings and landscape transitions.

Official generation instructions: https://dyndolod.info/Generation-Instructions

⸻

15. DLSS and Frame Generation

My setup also uses Theo’s Render Pipeline for DLSS and Frame Generation.

The two mods used are:

* Theo’s Render Pipeline - DLSS - FrameGen
* Theo’s Render Pipeline - DLSS - Frame Gen - Neural Rendering

In my MO2 left panel, the Standard version is above the Universal Neural Rendering version. The lower Universal entry takes priority where files conflict.

Follow the current installation instructions from the mod author. Do not assume that the same settings or files work with every GPU or Skyrim runtime.

Community Shaders and Theo’s Render Pipeline

The configuration used in my setup:

* Community Shaders upscaling remains enabled.
* Community Shaders Frame Generation is disabled.
* Community Shaders NVIDIA Reflex is disabled.
* Theo’s Render Pipeline handles Frame Generation and Reflex.

Do not enable two competing Frame Generation systems at the same time.

Use the configuration menu and hotkey supplied by the installed version of the mod. The menu shortcut can differ between releases or configurations.

My observed performance with DLSS enabled is around 90–110 FPS on an RTX 4050 Laptop GPU with 16 GB RAM. Your result will depend on resolution, graphics settings, location, CPU, GPU power limits and the rest of your modlist.

⸻

16. First launch and testing

Do not install the entire list and immediately start a long playthrough without testing.

Use this order:

1. Launch Skyrim through SKSE in MO2.
2. Confirm that the main menu loads.
3. Start a test game or load a safe test save.
4. Check character appearance and animations.
5. Visit an exterior location and inspect grass, trees, mountains and water.
6. Enter a city and inspect JK’s Skyrim locations.
7. Enter an interior and check lighting and audio.
8. Test combat effects, spell impacts and creature visuals.
9. Check distant objects and LOD.
10. Monitor performance and look for crashes or missing textures.

If something breaks, disable recently added mods in small groups and test again. Do not randomly remove core requirements.

Avoid uninstalling large gameplay or location mods in the middle of an important save. Make backups before major changes.

⸻

17. Troubleshooting

The game does not start

* Check that SKSE matches your Skyrim runtime.
* Check that Address Library is installed and appropriate for your runtime.
* Check for outdated SKSE plugins.
* Read the error message rather than reinstalling everything immediately.

A mod does not appear in the game

* Make sure it is enabled in MO2.
* Check whether it has a plugin that must also be enabled.
* Check its requirements.
* Check whether another mod overwrites its files.

Textures or meshes look wrong

* Open MO2’s conflict information.
* Check which mod wins the file conflict.
* Make sure the intended texture or mesh replacer has the correct priority.
* Check whether a patch is required.

A location crashes or looks broken

* Check compatibility between mods editing that location.
* Make sure the correct JK’s patches are installed.
* Check LOOT warnings and the mod descriptions.

DynDOLOD has errors

* Read the generation log.
* Check that the required resources and DLL are installed.
* Check that the current load order is finalized.
* Do not enable an incomplete or failed output.

⸻

18. Final notes

This setup aims to make Skyrim look and sound better without losing the atmosphere that made the original game special.

The main idea is simple:

* Keep the original gameplay.
* Preserve Skyrim’s visual identity.
* Improve the environment and atmosphere.
* Use animations that feel natural rather than exaggerated.
* Improve sound without changing the identity of the game.
* Generate LOD for the actual installed load order.
* Avoid unnecessary gameplay overhauls.

The modlist is based on my own working setup, but modding is version-sensitive. Always check requirements, compatibility notes and updates before installing.

Enjoy your journey through Skyrim.