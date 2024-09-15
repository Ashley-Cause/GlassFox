# GlassFox
Firefox Theme for macOS which makes the browser fully transparent through some questionable styling choices.

## PLEASE NOTE: I'VE ONLY TESTED THIS THEME ON MACOS

# What is what?
Within this repository, there are two files: `userChrome.css` and `userContent.css`.
`userChrome.css` is the file which provodes the transparency to the Firefox browser itself.
`userContent.css` provides some styling to a select few websites which I have thus far been bothered to style, to also make them transparent. As well as generally all of the built-in Firefox web pages such as the newtab page, the addons manager, and the settings page (`about:newtab`, `about:addons`, `about:preferences`).


## Getting Started
### To install the theme:
1. Open a new tab and navigate to `about:profiles`.
2. Click the button to "Show in Finder" under the profile you are currently on.
3. Within that profile folder (e.g. `Profiles/*.default/`), create a `chrome` folder, if it doesn't exist
4. Download the `userChrome.css`, and optionally the `userContent.css` file from this repository, and place them inside the `chrome` folder in your profile's directory.

### To activate the styling.
1. Open a new tab and navigate to `about:config`.
2. If you get a warning, click `Accept the Risk and Continue`.
3. Search for `stylesheets`, and enable `toolkit.legacyUserProfileCustomizations.stylesheets`.
4. If you also downloaded `userContent.css`, search for and enable `browser.tabs.allow_transparent_browser`

### To make it look good(ish i think)
