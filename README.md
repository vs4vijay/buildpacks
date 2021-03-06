# Srijan BuildPacks

**Builder**: Checks specified buildpacks

**BuildPack**: Detect -> Build -> Push

**BuildPackages**: Package distribution of multiple buildpacks

**Stack**: provides run-time and build-time environments

---

## Create Builder
```
pack create-builder viz-builder:latest --config builder.toml
```

## Create Package
```
pack package-buildpack viz-buildpack --config package.toml
```

## Create App
```
pack build viz-app --builder viz-builder:latest
```

---

### Development Notes

```

pack suggest-stacks

pack set-default-builder heroku/buildpacks:18

pack package-buildpack my-buildpack.cnb --package-config ./package.toml --format file


# Suggested Stacks

Stack ID: heroku-18
Description: The official Heroku stack based on Ubuntu 18.04
Maintainer: Heroku
Build Image: heroku/pack:18-build
Run Image: heroku/pack:18

Stack ID: io.buildpacks.stacks.bionic
Description: A minimal Cloud Foundry stack based on Ubuntu 18.04
Maintainer: Cloud Foundry
Build Image: cloudfoundry/build:base-cnb
Run Image: cloudfoundry/run:base-cnb

Stack ID: org.cloudfoundry.stacks.cflinuxfs3
Description: A large Cloud Foundry stack based on Ubuntu 18.04
Maintainer: Cloud Foundry
Build Image: cloudfoundry/build:full-cnb
Run Image: cloudfoundry/run:full-cnb

Stack ID: org.cloudfoundry.stacks.tiny
Description: A tiny Cloud Foundry stack based on Ubuntu 18.04, similar to distroless
Maintainer: Cloud Foundry
Build Image: cloudfoundry/build:tiny-cnb
Run Image: cloudfoundry/run:tiny-cnb

```