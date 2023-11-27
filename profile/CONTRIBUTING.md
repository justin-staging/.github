# Contributing

How MCSR mod development works

## Contributing code
Generally, if you want to contribute to a mod, the first step would be to make a pull request to an active maintainer. If you don't where to find an active repo, you can ask in the official discord or look in the commit history of the archive. If no maintainers are currently active and your pull request has gone without response, the next step would be to directly contact the mod team. In both cases, the next step for the update would be legalization.

## Legalization
For a mod update to be made legalized, a tech advisor has to review the code and the moderators have to give the go ahead. A new mod requires two reviews. Once the requisite approvals have been given, a tech advisor pushes the code to an archive repo and puts the new jars in the legal-mods repostory. After that, the mod is legal to use in runs.

# Specifications

## legal-mods repository

The legal-mods repository stores the most up-to-date versions of every internally managed legal mod. It is in the folder structure
```
<modid>/
  <legal-version-range>/
    <mod-file>.jar
```
so, for example, the current (as of writing this) 1.16 version of starlight would located at `starlight/1.16-1.16.5/starlight-1.16.1-v7.jar`. The range will be formatted as `<version>` or `<minimum version>-<maximum version>`

## Archive repositories

From now on, each newly legalized mod or update will have a copy of it's code stored on a MCSR Organization repository. These repositories will be under the name `<modid>-archive` and each branch will denote the legal versions. Using the last example, it's code will be stored at `starlight-archive` branch `1.16-1.16.5`.

## Internal and external mods
Internal mods are the mods which are checked every updated by the MCSR team and developed within the community. External mods are the opposite and are maintained by people outside of the MCSR community, for example the CaffeineMC mods (Sodium, Lithium, Krypton, Phosphor). The MCSR community has occassionally forked these mods and added fixes or made backports, these are also legal and are treated as internal mods. External mods are legal for any version range they are available for (except otherwise stated), but internal mods override this for the versions they support.

## Organization development repositories
If multiple people are contributing to a mod, it may make sense for the development to be centralized, and for this purpose an organization repo can be created, with the participants given write access. For this to happen, simply make a ticket in the discord with the request.
