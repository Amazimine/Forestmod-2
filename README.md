# Forest Mod — Fabric 1.21.1

A Minecraft horror mod featuring a mysterious forest entity with creepy idle and walk animations.

## How to get the .jar (no coding required)

1. Go to **github.com** and create a free account if you don't have one
2. Click the **+** button in the top right → **New repository**
3. Name it anything (e.g. `forestmod`), make it **Public**, click **Create repository**
4. On the next page click **uploading an existing file**
5. Drag and drop **all the files and folders** from this zip into the upload box
6. Click **Commit changes**
7. Click the **Actions** tab at the top of your repo
8. You should see a workflow run in progress — wait ~3 minutes for it to finish (green tick)
9. Click the finished run, then scroll down to **Artifacts** and download **forestmod-jar**
10. Unzip it — inside is `forestmod-1.0.0.jar`

## Installing the mod

1. Install [Fabric Loader 0.16.5](https://fabricmc.net/use/) for Minecraft 1.21.1
2. Download [Fabric API for 1.21.1](https://modrinth.com/mod/fabric-api) and put it in your mods folder
3. Put `forestmod-1.0.0.jar` in your `.minecraft/mods` folder
4. Launch Minecraft with the Fabric profile

## Spawning the entity in-game

```
/summon forestmod:forest_entity
```

## Adding your own texture

Replace `src/main/resources/assets/forestmod/textures/entity/forest_entity.png`
with your own 64×64 PNG texture before committing to GitHub.
