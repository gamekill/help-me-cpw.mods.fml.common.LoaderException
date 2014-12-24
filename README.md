help-me-cpw.mods.fml.common.LoaderException
==========================================

---- Minecraft Crash Report ----
// Don't be sad, have a hug! <3

Time: 2014.12.24. 18:24
Description: Exception in server tick loop

cpw.mods.fml.common.LoaderException: java.lang.ClassNotFoundException: Better Title Screen is a client-side only mod
	at cpw.mods.fml.common.ProxyInjector.inject(ProxyInjector.java:76)
	at cpw.mods.fml.common.FMLModContainer.constructMod(FMLModContainer.java:492)
	at sun.reflect.GeneratedMethodAccessor5.invoke(Unknown Source)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(Unknown Source)
	at java.lang.reflect.Method.invoke(Unknown Source)
	at com.google.common.eventbus.EventSubscriber.handleEvent(EventSubscriber.java:74)
	at com.google.common.eventbus.SynchronizedEventSubscriber.handleEvent(SynchronizedEventSubscriber.java:47)
	at com.google.common.eventbus.EventBus.dispatch(EventBus.java:322)
	at com.google.common.eventbus.EventBus.dispatchQueuedEvents(EventBus.java:304)
	at com.google.common.eventbus.EventBus.post(EventBus.java:275)
	at cpw.mods.fml.common.LoadController.sendEventToModContainer(LoadController.java:208)
	at cpw.mods.fml.common.LoadController.propogateStateMessage(LoadController.java:187)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(Unknown Source)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(Unknown Source)
	at java.lang.reflect.Method.invoke(Unknown Source)
	at com.google.common.eventbus.EventSubscriber.handleEvent(EventSubscriber.java:74)
	at com.google.common.eventbus.SynchronizedEventSubscriber.handleEvent(SynchronizedEventSubscriber.java:47)
	at com.google.common.eventbus.EventBus.dispatch(EventBus.java:322)
	at com.google.common.eventbus.EventBus.dispatchQueuedEvents(EventBus.java:304)
	at com.google.common.eventbus.EventBus.post(EventBus.java:275)
	at cpw.mods.fml.common.LoadController.distributeStateMessage(LoadController.java:118)
	at cpw.mods.fml.common.Loader.loadMods(Loader.java:492)
	at cpw.mods.fml.server.FMLServerHandler.beginServerLoading(FMLServerHandler.java:87)
	at cpw.mods.fml.common.FMLCommonHandler.onServerStart(FMLCommonHandler.java:314)
	at net.minecraft.server.dedicated.DedicatedServer.func_71197_b(DedicatedServer.java:117)
	at net.minecraft.server.MinecraftServer.run(MinecraftServer.java:387)
	at net.minecraft.server.MinecraftServer$2.run(MinecraftServer.java:685)
Caused by: java.lang.ClassNotFoundException: Better Title Screen is a client-side only mod
	at net.minecraft.launchwrapper.LaunchClassLoader.findClass(LaunchClassLoader.java:191)
	at java.lang.ClassLoader.loadClass(Unknown Source)
	at java.lang.ClassLoader.loadClass(Unknown Source)
	at cpw.mods.fml.common.ModClassLoader.loadClass(ModClassLoader.java:58)
	at java.lang.Class.forName0(Native Method)
	at java.lang.Class.forName(Unknown Source)
	at cpw.mods.fml.common.ProxyInjector.inject(ProxyInjector.java:59)
	... 27 more
Caused by: java.lang.NullPointerException
	at net.minecraft.launchwrapper.LaunchClassLoader.findClass(LaunchClassLoader.java:182)
	... 33 more


A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------

-- System Details --
Details:
	Minecraft Version: 1.7.10
	Operating System: Windows 7 (amd64) version 6.1
	Java Version: 1.8.0_25, Oracle Corporation
	Java VM Version: Java HotSpot(TM) 64-Bit Server VM (mixed mode), Oracle Corporation
	Memory: 788781880 bytes (752 MB) / 1632108544 bytes (1556 MB) up to 2863661056 bytes (2731 MB)
	JVM Flags: 3 total; -Xms1024m -Xmx3072m -XX:PermSize=256m
	AABB Pool Size: 0 (0 bytes; 0 MB) allocated, 0 (0 bytes; 0 MB) used
	IntCache: cache: 0, tcache: 0, allocated: 0, tallocated: 0
	FML: MCP v9.05 FML v7.10.85.1272 Minecraft Forge 10.13.2.1272 166 mods loaded, 166 mods active
	mcp{9.05} [Minecraft Coder Pack] (minecraft.jar) Unloaded->Constructed
	FML{7.10.85.1272} [Forge Mod Loader] (forge-1.7.10-10.13.2.1272-universal.jar) Unloaded->Constructed
	Forge{10.13.2.1272} [Minecraft Forge] (forge-1.7.10-10.13.2.1272-universal.jar) Unloaded->Constructed
	appliedenergistics2-core{rv2-beta-1} [AppliedEnergistics2 Core] (minecraft.jar) Unloaded->Constructed
	Aroma1997Core{1.0.2.13} [Aroma1997Core] (Aroma1997Core-1.7.10-1.0.2.13.jar) Unloaded->Constructed
	CodeChickenCore{1.0.4.29} [CodeChicken Core] (minecraft.jar) Unloaded->Constructed
	<CoFH ASM>{000} [CoFH ASM Data Initialization] (minecraft.jar) Unloaded->Constructed
	NotEnoughItems{1.0.3.77} [Not Enough Items] (NotEnoughItems-1.7.10-1.0.3.77-universal.jar) Unloaded->Constructed
	ThaumicTinkerer-preloader{0.1} [Thaumic Tinkerer Core] (minecraft.jar) Unloaded->Constructed
	OpenModsCore{0.6} [OpenModsCore] (minecraft.jar) Unloaded->Constructed
	CoFHCore{1.7.10R3.0.0B9} [CoFH Core] (CoFHCore-[1.7.10]3.0.0B9-46.jar) Unloaded->Constructed
	BuildCraft|Core{6.2.6} [BuildCraft] (buildcraft-6.2.6.jar) Unloaded->Constructed
	BuildCraft|Transport{6.2.6} [BC Transport] (buildcraft-6.2.6.jar) Unloaded->Constructed
	BuildCraft|Silicon{6.2.6} [BC Silicon] (buildcraft-6.2.6.jar) Unloaded->Constructed
	BuildCraft|Factory{6.2.6} [BC Factory] (buildcraft-6.2.6.jar) Unloaded->Constructed
	additionalpipes{3.2} [Additional Pipes] (additionalpipes-3.2.jar) Unloaded->Constructed
	IC2{2.2.654-experimental} [IndustrialCraft 2] (industrialcraft-2-2.2.654-experimental.jar) Unloaded->Constructed
	AdvancedMachines{1.1.2} [IC2 Advanced Machines Addon] (AdvancedMachinesAS-1.7.10.jar) Unloaded->Constructed
	AdvancedSolarPanel{1.7.10-3.5.1} [Advanced Solar Panels] (AdvancedSolarPanel-1.7.10-3.5.1.jar) Unloaded->Constructed
	AppleCore{1.0.1} [AppleCore] (AppleCore-mc1.7.10-1.0.1.jar) Unloaded->Constructed
	appliedenergistics2{rv2-beta-1} [Applied Energistics 2] (appliedenergistics2-rv2-beta-1.jar) Unloaded->Constructed
	Aroma1997CoreHelper{1.0.2.13} [Aroma1997Core|Helper] (Aroma1997Core-1.7.10-1.0.2.13.jar) Unloaded->Constructed
	Aroma1997sDimension{1.0} [Aroma1997's Dimensional World] (Aroma1997s-Dimensional-World-1.7.10-1.1.0.1.jar) Unloaded->Constructed
	AromaBackup{0.0.0.5} [AromaBackup] (AromaBackup-1.7.10-0.0.0.5.jar) Unloaded->Constructed
	Backpack{2.0.1} [Backpack] (backpack-2.0.1-1.7.x.jar) Unloaded->Constructed
	bdlib{1.5.1.32} [BD Lib] (bdlib-mc1710-1.5.1.32.jar) Unloaded->Constructed
	BetterTitleScreen{1.7.10-1.1} [Better Title Screen] (BetterTitleScreen-1.7.10-1.1.jar) Unloaded->Errored
	BiblioCraft{1.9.1} [BiblioCraft] (BiblioCraft[v1.9.1][MC1.7.10].jar) Unloaded->Constructed
	ExtrabiomesXL{3.16.0} [ExtrabiomesXL] (extrabiomesxl_1.7.10-3.16.0.jar) Unloaded->Constructed
	BiblioWoodsEBXL{1.4} [BiblioWoods ExtraBiomesXL Edition] (BiblioWoods[ExtraBiomesXL][v1.4].jar) Unloaded->Constructed
	Forestry{3.3.0.334-unstable} [Forestry for Minecraft] (forestry_1.7.10-3.3.0.334-unstable.jar) Unloaded->Constructed
	BiblioWoodsForestry{1.7} [BiblioWoods Forestry Edition] (BiblioWoods[Forestry][v1.7].jar) Unloaded->Constructed
	Mantle{1.7.10-0.3.2.jenkins184} [Mantle] (Mantle-1.7.10-0.3.2.jar) Unloaded->Constructed
	Natura{2.2.0} [Natura] (natura-1.7.10-2.2.0.1.jar) Unloaded->Constructed
	BiblioWoodsNatura{1.5} [BiblioWoods Natura Edition] (BiblioWoods[Natura][v1.5].jar) Unloaded->Constructed
	BinnieCore{2.0-dev5} [Binnie Core] (binnie-mods-2.0-dev5.jar) Unloaded->Constructed
	ExtraTrees{2.0-dev5} [Extra Trees] (binnie-mods-2.0-dev5.jar) Unloaded->Constructed
	binnie-fix-dev5{1.0} [BinnieFixDev5] (binnie-fix-dev5-1.7.10-1.0.jar) Unloaded->Constructed
	Botany{2.0-dev5} [Botany] (binnie-mods-2.0-dev5.jar) Unloaded->Constructed
	ExtraBees{2.0-dev5} [Extra Bees] (binnie-mods-2.0-dev5.jar) Unloaded->Constructed
	Genetics{2.0-dev5} [Genetics] (binnie-mods-2.0-dev5.jar) Unloaded->Constructed
	AWWayofTime{v1.3.0Beta} [Blood Magic: Alchemical Wizardry] (BloodMagic-1.7.10-1.3.0Beta-6.jar) Unloaded->Constructed
	bluepower{0.1.766} [Blue Power] (BluePower-1.7.10-0.1.766-universal.jar) Unloaded->Constructed
	Baubles{1.0.1.10} [Baubles] (Baubles-1.7.10-1.0.1.10.jar) Unloaded->Constructed
	Thaumcraft{4.2.2.1} [Thaumcraft] (Thaumcraft-1.7.10-4.2.2.1.jar) Unloaded->Constructed
	Botania{r1.3-145} [Botania] (Botania r1.3-145.jar) Unloaded->Constructed
	BuildCraft|Builders{6.2.6} [BC Builders] (buildcraft-6.2.6.jar) Unloaded->Constructed
	BuildCraft|Energy{6.2.6} [BC Energy] (buildcraft-6.2.6.jar) Unloaded->Constructed
	CarpentersBlocks{3.3.3} [Carpenter's Blocks] (Carpenter's Blocks v3.3.3 - MC 1.7.10.jar) Unloaded->Constructed
	ChickenChunks{1.3.4.15} [ChickenChunks] (ChickenChunks-1.7.10-1.3.4.15-universal.jar) Unloaded->Constructed
	ForgeMultipart{1.1.0.314} [Forge Multipart] (ForgeMultipart-1.7.10-1.1.0.314-universal.jar) Unloaded->Constructed
	chisel{2.1.3} [Chisel] (Chisel 2-2.1.3.jar) Unloaded->Constructed
	CompactSolars{4.4.39.315} [Compact Solar Arrays] (CompactSolars-1.7.10-4.4.39.315-universal.jar) Unloaded->Constructed
	ComputerCraft{1.65} [ComputerCraft] (ComputerCraft1.65.jar) Unloaded->Constructed
	cookiecore{1.3.0} [Cookie Core] (cookiecore-1.3.0.jar) Unloaded->Constructed
	Enchiridion{1.1} [Enchiridion] (Enchiridion-1.7.X-1.2b.jar) Unloaded->Constructed
	MineFactoryReloaded{1.7.10R2.8.0RC6} [MineFactory Reloaded] (MineFactoryReloaded-[1.7.10]2.8.0RC6-5.jar) Unloaded->Constructed
	EnderIO{1.7.10-2.2.5.311} [Ender IO] (EnderIO-1.7.10-2.2.5.311.jar) Unloaded->Constructed
	EnderStorage{1.4.5.27} [EnderStorage] (EnderStorage-1.7.10-1.4.5.27-universal.jar) Unloaded->Constructed
	ThermalFoundation{1.7.10R1.0.0RC1} [Thermal Foundation] (ThermalFoundation-[1.7.10]1.0.0RC1-13.jar) Unloaded->Constructed
	ThermalExpansion{1.7.10R4.0.0B8} [Thermal Expansion] (ThermalExpansion-[1.7.10]4.0.0B8-23.jar) Unloaded->Constructed
	EnderTech{1.7.10-0.3.0.358} [EnderTech] (EnderTech-1.7.10-0.3.0.358.jar) Unloaded->Constructed
	extracarts{b0.6.1} [Extra Carts] (ExtraCarts-1.7.10-b0.7.0.jar) Unloaded->Constructed
	Waila{1.5.6a} [Waila] (Waila-1.5.6a_1.7.10.jar) Unloaded->Constructed
	extracells{2.2.21} [ExtraCells] (ExtraCells-1.7.10-2.2.21b40.jar) Unloaded->Constructed
	ExtraUtilities{1.1.0k} [Extra Utilities] (extrautilities-1.1.0k.jar) Unloaded->Constructed
	fastleafdecay{1.0} [Fast Leaf Decay] (FastLeafDecay-1.7.10-1.0.jar) Unloaded->Constructed
	ThaumicTinkerer{unspecified} [Thaumic Tinkerer] (ThaumicTinkerer-2.5-1.7.10-162.jar) Unloaded->Constructed
	ForbiddenMagic{1.7.10-0.551} [Forbidden Magic] (Forbidden Magic-1.7.10-0.551.jar) Unloaded->Constructed
	Railcraft{9.4.0.0} [Railcraft] (Railcraft_1.7.10-9.4.0.0.jar) Unloaded->Constructed
	TConstruct{1.7.10-1.8.0.build804} [Tinkers' Construct] (TConstruct-1.7.10-1.8.0.jar) Unloaded->Constructed
	MagicBees{1.7.10-2.1.22} [Magic Bees] (magicbees-1.7.10-2.1.22.jar) Unloaded->Constructed
	gendustry{1.4.3.5} [GenDustry] (gendustry-fu-mc1710-1.4.3.5.jar) Unloaded->Constructed
	GraviSuite{1.7.10-2.0.3} [Graviation Suite] (GraviSuite-1.7.10-2.0.3.jar) Unloaded->Constructed
	iChunUtil{4.0.0} [iChunUtil] (iChunUtil-4.0.0.jar) Unloaded->Constructed
	Hats{4.0.1} [Hats] (Hats-4.0.1.jar) Unloaded->Constructed
	HatStand{4.0.0} [HatStand] (HatStand-4.0.0.jar) Unloaded->Constructed
	IC2NuclearControl{2.0.8c} [Nuclear Control 2] (IC2NuclearControl-2.0.8c.jar) Unloaded->Constructed
	inpure|core{1.7.10R1.0.0B7} [INpureCore] (INpureCore-[1.7.10]1.0.0B7-19.jar) Unloaded->Constructed
	inventorytweaks{1.58-147-645ca10} [Inventory Tweaks] (InventoryTweaks-1.58-147.jar) Unloaded->Constructed
	iridiummod{0.7} [Iridium Mod] (iridiummod-1.7-0.7.jar) Unloaded->Constructed
	IronChest{6.0.43.730} [Iron Chest] (ironchest-1.7.10-6.0.43.730-universal.jar) Unloaded->Constructed
	JABBA{1.2.0a} [JABBA] (Jabba-1.2.0a_1.7.10.jar) Unloaded->Constructed
	LatCoreMC{1.6.1} [LatCoreMC] (LatCoreMC-1.7.10-1.6.1.jar) Unloaded->Constructed
	LatBlocks{1.6.1} [LatBlocks Mod] (LatBlocks-1.7.10-1.6.1.jar) Unloaded->Constructed
	LogisticsPipes{0.8.2.89} [Logistics Pipes] (logisticspipes-0.8.2.89.jar) Unloaded->Constructed
	MineFactoryReloaded|CompatAppliedEnergistics{1.7.10R2.8.0RC6} [MFR Compat: Applied Energistics] (MineFactoryReloaded-[1.7.10]2.8.0RC6-5.jar) Unloaded->Constructed
	MineFactoryReloaded|CompatAtum{1.7.10R2.8.0RC6} [MFR Compat: Atum] (MineFactoryReloaded-[1.7.10]2.8.0RC6-5.jar) Unloaded->Constructed
	MineFactoryReloaded|CompatBackTools{1.7.10R2.8.0RC6} [MFR Compat: BackTools] (MineFactoryReloaded-[1.7.10]2.8.0RC6-5.jar) Unloaded->Constructed
	MineFactoryReloaded|CompatBuildCraft{1.7.10R2.8.0RC6} [MFR Compat: BuildCraft] (MineFactoryReloaded-[1.7.10]2.8.0RC6-5.jar) Unloaded->Constructed
	MineFactoryReloaded|CompatChococraft{1.7.10R2.8.0RC6} [MFR Compat: Chococraft] (MineFactoryReloaded-[1.7.10]2.8.0RC6-5.jar) Unloaded->Constructed
	MineFactoryReloaded|CompatExtraBiomes{1.7.10R2.8.0RC6} [MFR Compat: ExtraBiomes] (MineFactoryReloaded-[1.7.10]2.8.0RC6-5.jar) Unloaded->Constructed
	MineFactoryReloaded|CompatForestry{1.7.10R2.8.0RC6} [MFR Compat: Forestry] (MineFactoryReloaded-[1.7.10]2.8.0RC6-5.jar) Unloaded->Constructed
	MineFactoryReloaded|CompatForgeMicroblock{1.7.10R2.8.0RC6} [MFR Compat: ForgeMicroblock] (MineFactoryReloaded-[1.7.10]2.8.0RC6-5.jar) Unloaded->Constructed
	MineFactoryReloaded|CompatIC2{1.7.10R2.8.0RC6} [MFR Compat: IC2] (MineFactoryReloaded-[1.7.10]2.8.0RC6-5.jar) Unloaded->Constructed
	MineFactoryReloaded|CompatMystcraft{1.7.10R2.8.0RC6} [MFR Compat: Mystcraft] (MineFactoryReloaded-[1.7.10]2.8.0RC6-5.jar) Unloaded->Constructed
	MrTJPCoreMod{1.0} [MrTJPCoreMod] (MrTJPCore-1.7.10-1.0.3.5-universal.jar) Unloaded->Constructed
	ProjRed|Core{4.5.8.59} [ProjectRed] (ProjectRed-1.7.10-4.5.8.59-Base.jar) Unloaded->Constructed
	ProjRed|Exploration{4.5.8.59} [ProjectRed-Exploration] (ProjectRed-1.7.10-4.5.8.59-World.jar) Unloaded->Constructed
	MineFactoryReloaded|CompatProjRed{1.7.10R2.8.0RC6} [MFR Compat ProjectRed] (MineFactoryReloaded-[1.7.10]2.8.0RC6-5.jar) Unloaded->Constructed
	MineFactoryReloaded|CompatRailcraft{1.7.10R2.8.0RC6} [MFR Compat: Railcraft] (MineFactoryReloaded-[1.7.10]2.8.0RC6-5.jar) Unloaded->Constructed
	MineFactoryReloaded|CompatRP2{1.7.10R2.8.0RC6} [MFR Compat: RP2] (MineFactoryReloaded-[1.7.10]2.8.0RC6-5.jar) Unloaded->Constructed
	MineFactoryReloaded|CompatSufficientBiomes{1.7.10R2.8.0RC6} [MFR Compat: Sufficient Biomes] (MineFactoryReloaded-[1.7.10]2.8.0RC6-5.jar) Unloaded->Constructed
	MineFactoryReloaded|CompatThaumcraft{1.7.10R2.8.0RC6} [MFR Compat: Thaumcraft] (MineFactoryReloaded-[1.7.10]2.8.0RC6-5.jar) Unloaded->Constructed
	MineFactoryReloaded|CompatThermalExpansion{1.7.10R2.8.0RC6} [MFR Compat: Thermal Expansion] (MineFactoryReloaded-[1.7.10]2.8.0RC6-5.jar) Unloaded->Constructed
	MineFactoryReloaded|CompatTConstruct{1.7.10R2.8.0RC6} [MFR Compat: Tinkers' Construct] (MineFactoryReloaded-[1.7.10]2.8.0RC6-5.jar) Unloaded->Constructed
	TwilightForest{2.3.2} [The Twilight Forest] (twilightforest-1.7.10-2.3.2.jar) Unloaded->Constructed
	MineFactoryReloaded|CompatTwilightForest{1.7.10R2.8.0RC6} [MFR Compat: TwilightForest] (MineFactoryReloaded-[1.7.10]2.8.0RC6-5.jar) Unloaded->Constructed
	MineFactoryReloaded|CompatVanilla{1.7.10R2.8.0RC6} [MFR Compat: Vanilla] (MineFactoryReloaded-[1.7.10]2.8.0RC6-5.jar) Unloaded->Constructed
	MineTweaker3{3.0.9B} [MineTweaker 3] (MineTweaker3-1.7.10-3.0.9C.jar) Unloaded->Constructed
	MobAmputation{4.0.0} [MobAmputation] (MobAmputation-4.0.0.jar) Unloaded->Constructed
	MobDismemberment{4.0.0} [MobDismemberment] (MobDismemberment-4.0.0.jar) Unloaded->Constructed
	ModTweaker{0.5c} [ModTweaker] (ModTweaker-1.7.X-0.5d.jar) Unloaded->Constructed
	cfm{3.4.2} [§9MrCrayfish's Furniture Mod] (MrCrayfishFurnitureModv3.4.2(1.7.10).jar) Unloaded->Constructed
	NearbyMobFinder{1.7.10-1.1.1} [Nearby Mob Finder] (NearbyMobFinder-1.7.10-1.1.1.jar) Unloaded->Constructed
	NEIAddons{1.12.3.11} [NEI Addons] (neiaddons-mc1710-1.12.3.11.jar) Unloaded->Constructed
	NEIAddons|Botany{1.12.3.11} [NEI Addons: Botany] (neiaddons-mc1710-1.12.3.11.jar) Unloaded->Constructed
	NEIAddons|Forestry{1.12.3.11} [NEI Addons: Forestry] (neiaddons-mc1710-1.12.3.11.jar) Unloaded->Constructed
	NEIAddons|CraftingTables{1.12.3.11} [NEI Addons: Crafting Tables] (neiaddons-mc1710-1.12.3.11.jar) Unloaded->Constructed
	NEIAddons|ExNihilo{1.12.3.11} [NEI Addons: Ex Nihilo] (neiaddons-mc1710-1.12.3.11.jar) Unloaded->Constructed
	neiintegration{1.0.3} [NEI Integration] (NEIIntegration-MC1.7.10-1.0.3.jar) Unloaded->Constructed
	ObsidiPlates{3.0.0.18} [ObsidiPlates] (ObsidiPlates-1.7.10-universal-3.0.0.18.jar) Unloaded->Constructed
	OpenMods{0.6} [OpenMods] (OpenModsLib-1.7.10-0.6-snapshot-268.jar) Unloaded->Constructed
	OpenBlocks{1.3} [OpenBlocks] (OpenBlocks-1.7.10-1.3-snapshot-513.jar) Unloaded->Constructed
	harvestcraft{1.7.10b} [Pam's HarvestCraft] (Pam's HarvestCraft 1.7.10c.jar) Unloaded->Constructed
	planetguyLib{1.2} [planetguyLib] (PlanetguyLib-1.2.jar) Unloaded->Constructed
	PneumaticCraft{1.4.4-47} [PneumaticCraft] (PneumaticCraft-1.7.10-1.4.4-47-universal.jar) Unloaded->Constructed
	PowerConverters{1.7.10-3.0.0.30} [Power Converters] (PowerConverters-1.7.10-3.0.0.30.jar) Unloaded->Constructed
	ProjRed|Transmission{4.5.8.59} [ProjectRed-Transmission] (ProjectRed-1.7.10-4.5.8.59-Integration.jar) Unloaded->Constructed
	ProjRed|Transportation{4.5.8.59} [ProjectRed-Transportation] (ProjectRed-1.7.10-4.5.8.59-Mechanical_beta.jar) Unloaded->Constructed
	ProjRed|Compatibility{4.5.8.59} [ProjectRed-Compatibility] (ProjectRed-1.7.10-4.5.8.59-Compat.jar) Unloaded->Constructed
	ProjRed|Integration{4.5.8.59} [ProjectRed-Integration] (ProjectRed-1.7.10-4.5.8.59-Integration.jar) Unloaded->Constructed
	ProjRed|Illumination{4.5.8.59} [ProjectRed-Illumination] (ProjectRed-1.7.10-4.5.8.59-Lighting.jar) Unloaded->Constructed
	ProjRed|Expansion{4.5.8.59} [ProjectRed-Expansion] (ProjectRed-1.7.10-4.5.8.59-Mechanical_beta.jar) Unloaded->Constructed
	RedstoneArsenal{1.7.10R1.1.0RC1} [Redstone Arsenal] (RedstoneArsenal-[1.7.10]1.1.0RC1-19.jar) Unloaded->Constructed
	JAKJ_RedstoneInMotion{2.3.0} [Remain In Motion] (RemainInMotion-2.3.0.jar) Unloaded->Constructed
	JAKJ_RedstoneInMotion_HollowCarriages{1.0} [JAKJ_RedstoneInMotion_HollowCarriages] (RemainInMotion-2.3.0.jar) Unloaded->Constructed
	secretroomsmod{4.7.1} [The SecretRoomsMod] (secretroomsmod-1.7.10-4.7.1.375.jar) Unloaded->Constructed
	simplyjetpacks{1.3.1} [Simply Jetpacks] (SimplyJetpacks-MC1.7.10-1.3.1.jar) Unloaded->Constructed
	SolarExpansion{1.2c} [Solar Expansion] (SolarExpansion-Basic-1.2c.jar) Unloaded->Constructed
	SolarFlux{1.7.10-0.4c} [Solar Flux] (SolarFlux-1.7.10-0.4c.jar) Unloaded->Constructed
	SSR{rc3} [Soul Shards Reborn] (SSR-rc3.jar) Unloaded->Constructed
	StevesCarts{2.0.0.b18} [Steve's Carts 2] (StevesCarts2.0.0.b18.jar) Unloaded->Constructed
	StevesFactoryManager{A93} [Steve's Factory Manager] (StevesFactoryManagerA93.jar) Unloaded->Constructed
	ThaumcraftMobAspects{1.7.2-2A} [Thaumcraft Mob Aspects] (ThaumcraftMobAspects-1.7.2-2A.jar) Unloaded->Constructed
	thaumcraftneiplugin{1.7.10-1.6a} [Thaumcraft NEI Plugin] (thaumcraftneiplugin-1.7.10-1.6a.jar) Unloaded->Constructed
	thaumicenergistics{0.8.7.2a-rv2} [Thaumic Energistics] (thaumicenergistics-0.8.7.2a-rv2.jar) Unloaded->Constructed
	ThaumicExploration{0.6.0} [Thaumic Exploration] (ThaumicExploration-1.7.10-1.1-34.jar) Unloaded->Constructed
	thaumicinfusion{3.8.1} [Thaumic Infusion] (ThaumicInfusion-1.7.10-3.83.jar) Unloaded->Constructed
	TFoxMod{1.6.1} [TFox's Mod] (TheTFoxMod-1.7.10-1.6.1.jar) Unloaded->Constructed
	TSteelworks{1.7.10-1.0.6} [Tinkers' Steelworks] (TSteelworks-1.7.10-1.0.6.jar) Unloaded->Constructed
	TiCTooltips{1.1.11b} [TiC Tooltips] (TiCTooltips-mc1.7.10-1.1.11b.jar) Unloaded->Constructed
	TMechworks{1.7.10-86.e500b88} [Tinkers' Mechworks] (TMechworks-1.7.10-0.2.10.jar) Unloaded->Constructed
	Translocator{1.1.1.14} [Translocator] (Translocator-1.7.10-1.1.1.14-universal.jar) Unloaded->Constructed
	ttCore{MC1.7.10-0.1.0-48} [ttCore] (ttCore-MC1.7.10-0.1.0-48.jar) Unloaded->Constructed
	TWarden{1.1.1} [Thaumic Warden] (TWarden-1.1.1.jar) Unloaded->Constructed
	WailaHarvestability{1.0.4} [Waila Harvestability] (WailaHarvestability-mc1.7.x-1.0.4.jar) Unloaded->Constructed
	wailaplugins{MC1.7.10-0.0.1-10} [WAILA Plugins] (WAILAPlugins-MC1.7.10-0.0.1-10.jar) Unloaded->Constructed
	wawla{1.0.9} [What Are We Looking At] (Wawla-1.0.9_1.7.10.jar) Unloaded->Constructed
	witchery{0.21.0} [Witchery] (witchery-1.7.10-0.21.0.jar) Unloaded->Constructed
	WR-CBE|Core{1.4.1.9} [WR-CBE Core] (WR-CBE-1.7.10-1.4.1.9-universal.jar) Unloaded->Constructed
	WR-CBE|Addons{1.4.1.9} [WR-CBE Addons] (WR-CBE-1.7.10-1.4.1.9-universal.jar) Unloaded
