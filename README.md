# Cloudy Downloads

Public release artifacts for Cloudy apps, served by GitHub Pages from this
repo. One folder per app; every URL inside a folder is stable forever, so
marketing sites and shipped builds never change when a release goes out.

## Layout

    indecs/Indecs.dmg        # always the latest Indecs for Mac DMG
    indecs/appcast.xml       # Sparkle feed (SUFeedURL in the app's Info.plist)
    tokematic/               # (migration pending: tokematic issue)

## Releasing

A release is a PR to this repo that replaces the DMG and appcast in the app's
folder. The marketing site links the stable folder URLs; GitHub Pages serves
them at:

    https://cloudyindustries.github.io/cloudy-downloads/<app>/<file>
