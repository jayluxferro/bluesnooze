![Bluesnooze logo](images/icon.png)

# Bluesn00ze
This is a fork of the **Bluesnooze** application.

[Download the latest release][download-latest]


## About

**Bluesnooze prevents your sleeping Mac from connecting to Bluetooth accessories.**

If you pair Bluetooth headphones or speakers with both your phone & Mac it can be frustrating when your sleeping Mac connects intermittently and disrupts the audio.

With Bluesnooze the Bluetooth connection is switched off when your Mac sleeps, and switched on when your Mac wakes.

![Screenshot showing Bluesnooze in the status bar](images/screenshot.png)


## Installation

1. Download `Bluesnooze.zip` from the [latest release][download-latest]
1. In Finder, open `Bluesnooze.zip` in your `Downloads` directory
1. Drag `Bluesn00ze.app` to your `Applications` directory
1. *Optional*: Configure 'Launch at login'

## Caveats

- Please note this app is not compatible with the “Allow your Apple Watch to unlock your Mac” feature.
- Unfortunately this app can't be distributed via the App Store because it uses a private API to switch Bluetooth on/off (but the release version is notarized by Apple).

## Settings

The application settings can be modified using the `defaults` command. 

```shell
# read settings:
defaults read org.sperixlabs.Bluesnooze hideIcon

# update settings:
defaults write org.sperixlabs.Bluesnooze hideIcon -bool true

# delete settings: (this resets everything to defaults)
defaults delete org.sperixlabs.Bluesnooze
```


[download-latest]: https://github.com/jayluxferro/bluesnooze/releases/latest

## Acknowledgements
- https://github.com/odlp/bluesnooze
