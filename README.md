# MoneyManager EX Themes

MMEX supports themes that can change the HTML layout and icons used within the application. The application is
shipped with a number of 'system' themes, the content of which can be viewed within the [system-themes](system-themes/) folder

Feel free to share your themes here in the [User Themes](other-themes/) area.

## Theme contents

A theme consists of the following files which must be present in the theme. The theme itself should be a zip file with an extensions .mmextheme. The folder hierachy within the theme is optional.

- Theme Meta Data
    - _theme.json (see below for valid JSON)
    - _theme.png (A 300x150 image that showcases the theme and will be displayed against the theme in the application Theme Manager)
- A master.css file used for HTML formatting, accompanyimng files for the master.css file may also be included (e.g. background.png files)
- Icons that make up the theme (see [Default Theme](system-themes/default/) for detail on teh full list of icons)

## JSON content

### Example JSON

```json
{ "name": "MMEX Default Theme",
    "author": "MMEX Team",
    "description": "This is the default MMEX theme and uses the MMEX colour scheme. It is a simple 'duo color' theme",
    "url": "https://github.com/moneymanagerex/moneymanagerex/blob/master/resources/themes/default/readme.md"
}
```

- name = The full theme name
- author = The name of the team or individual responsible for theme creation
- description = A short description of the theme
- url = A URL that links to more detail about the theme

