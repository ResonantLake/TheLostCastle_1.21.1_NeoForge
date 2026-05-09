# TheLostCastel-1.21.1-NeoForge

## [TheLostCastle](https://github.com/Jack-Bagel/The-Lost-Castle) 모드의 1.21.1 버전 NeoForge 모드로더 포팅 버전입니다

![Lost Castle Banner](https://i.imgur.com/2hvM43r.png) <span style="font-family: helvetica, arial, sans-serif; font-size: 14px;">&nbsp;<br></span>

<span style="font-family: helvetica, arial, sans-serif; font-size: 14px;"><strong>Former structure of End Remastered, The Lost Castle introduces an enormous castle that you'll be able to find with the help of a map given by a journeyman cartographer. Inside resides infinite fortune and mysteries from a long forgotten civilization that disappeared a long time ago and is now eagerly guarded by illagers that won't give up on their fortune even if it means the end of them, or the end of you...<br></strong></span>

 

<span style="font-family: helvetica, arial, sans-serif; font-size: 14px;"><strong>*Note that the castle is pretty rare and can spawn multiple thousands of blocks away from spawn.</strong></span>

<span style="font-family: helvetica, arial, sans-serif; font-size: 14px;">Supported Versions: 1.18.2, 1.19.X, 1.20.X!</span>

 <span style="font-size: 24px;">&nbsp;<img src="https://i.imgur.com/BwHHtEH.png" alt="" width="1125" height="313"></span>

 

<div class="spoiler">&nbsp;<img src="https://i.imgur.com/iU2lZ7Y.png" alt="" width="1113" height="696"></div>


<div class="spoiler"><p><img src="https://i.imgur.com/gkMuTuB.png" alt="" width="1113" height="696"></p></div>

 

<div class="spoiler"><p><img src="https://i.imgur.com/y8cEs4F.png" alt="" width="1113" height="696"></p></div>

 

![](https://i.imgur.com/uIGZuYH.png)

<span style="font-size: 14px;">We always try to be aware of issues in our mods, if you experience a bug while playing, please report it in the comments or the "Issues" section to help us keep the experience fun and enjoyable for all players.<strong><br></strong></span>

 <span style="font-size: 14px;"><span style="color: #3366ff;" data-darkreader-inline-color=""><strong>&nbsp;<a style="color: #3366ff;" href="https://discord.gg/D9cxayDNSP" data-darkreader-inline-color="">CLICK HERE</a> </strong></span><strong>to&nbsp;</strong><strong>join our discord server to speak, chat, report problems o</strong><strong>r talk with us :)</strong></span>

## Credits & License

This is a backport of [The Lost Castle](https://github.com/Jack-Bagel/The-Lost-Castle)
by Jack Bagel / Team Remastered (originally targeting Minecraft 1.21.5).

- **Original mod**: https://github.com/Jack-Bagel/The-Lost-Castle
- **Original author**: [@Jack-Bagel](https://github.com/Jack-Bagel)
- **License**: GNU Lesser General Public License v3.0 only (LGPL-3.0-only) — see [LICENSE](LICENSE)

### Port changes (1.21.5 → 1.21.1 NeoForge)

- Downgraded NeoForge / NeoForm / Parchment versions in `gradle.properties`
- Disabled the Fabric subproject in `settings.gradle`
- Adjusted `FoundationProcessor` for 1.21.1 API (`getMinBuildHeight`/`getMaxBuildHeight`,
  3-argument `ChunkAccess.setBlockState`)
- Updated stronghold-disabling mixin signature to match 1.21.1
  `ChunkGenerator.tryGenerateStructure` (9 parameters)
- Moved the mixin from the `server` array to `mixins` so it applies in single player
- Replaced a corrupted `castle_ml.nbt` with the equivalent file from the 1.20.X release of the same mod
EOF
