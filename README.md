# Srijan BuildPacks

Builder: Detect -> Build -> Push

BuildPack: 

BuildPackages: Consists of multiple buildpacks

Stack

## Create Builder
pack create-builder viz-builder:bionic --builder-config ./builder.toml

## Create App
pack build viz-app --builder my-builder:bionic

```

pack set-default-builder heroku/buildpacks:18

```