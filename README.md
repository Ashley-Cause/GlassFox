# GlassFox
GlassFox is my custom Firefox Theme for macOS which attempts to make the browser fully transparency, or take advantage of macOS' vibrancy.
In progress-ish in that its not a perfect overhaul, but I probably won't really add to it much as I've not got time to maintain it really.

<img width="1710" alt="image" src="https://github.com/user-attachments/assets/f776e6d4-4d23-44e2-8892-0f5211200c56">

<img width="1710" alt="image" src="https://github.com/user-attachments/assets/07648cda-1c5f-4711-872a-4f2c5204dc30">


## PLEASE NOTE: I'VE ONLY TESTED THIS THEME ON MACOS

# What is what?
Within this repository, there are two files: `userChrome.css` and `userContent.css`.
`userChrome.css` is the file which provodes the transparency to the Firefox browser itself.
`userContent.css` provides some styling to a select few websites which I have thus far been bothered to style, to also make them transparent. As well as generally all of the built-in Firefox web pages such as the newtab page, the addons manager, and the settings page (`about:newtab`, `about:addons`, `about:preferences`).


## Getting Started
### To install the theme:
1. Open a new tab and navigate to `about:profiles`.
2. Click the button to "Show in Finder" under the profile you are currently on.
3. Within that profile folder (e.g. `Profiles/*.default/`), create a `chrome` folder if it doesn't already exist
4. Download the `userChrome.css`, and optionally the `userContent.css` file from this repository, and place them inside the `chrome` folder in your profile's directory.

### To activate the styling.
1. Open a new tab and navigate to `about:config`.
2. If you get a warning, click `Accept the Risk and Continue`.
3. Search for and enable (set to `true`):
  1. `toolkit.legacyUserProfileCustomizations.stylesheets`.
  2. `widget.macos.titlebar-blend-mode.behind-window`
  3. If you downloaded `userContent.css`: `browser.tabs.allow_transparent_browser`

### Extensions that I use with this theme
#### [UnloadTabs](https://addons.mozilla.org/en-US/firefox/addon/unload-tabs/)
Self explanatory, lets you unload tabs at will via the tab context menu or a keyboard shortcut.

#### [Tab Session Manager](https://addons.mozilla.org/en-US/firefox/addon/tab-session-manager/)
Saves the tabs you have open when you close a window, so that you can reopen them later if you want to.
Sometimes Firefox glitches and clears my tabs, or I accidentally open a different window and lose my pinned tabs.
Tab Session Manager means its less painful to get them back.
Also useful if you're trying to keep track of different projects, you can rename sessions to make them easy to find.

#### [Stylus](https://addons.mozilla.org/en-US/firefox/addon/styl-us/)
I'm not a big fan of scrollbars on the main body of web pages, and sometimes the scrollbar also clips into the edge of the website content,
so I use Stylus to hide the scrollbars.
Pretty simple to use, but all you have to do to hide the scrollbars is create a new style, and paste the following into the stylesheet.
```css
html, body {
    scrollbar-width: none;
}
```

**More on Stylus**
Stylus is probably where I will add more support for transparency on other websites, instead of updating this repository.
And so I've created a style on Stylus called `GlassFox`, which contains all of the styles that are in `userContent.css`, except for the styles
for built-in Firefox pages such as any page with the url prefix `about:`.
So if you don't mind the lack of transparency on the newtab page for example, but still want some transparency, install the `GlassFox` style on Stylus.
