# MoneyManager EX Themes

MMEX supports themes that can change the HTML layout and icons used within the application. The application is
shipped with a number of 'system' themes, the content of which can be viewed within the [system-themes](system-themes/) folder

Feel free to share your themes here in the [User Themes](other-themes/) area.

## Theme contents

A theme consists of the following files which must be present in the theme. The theme itself should have an **.mmextheme** extension and by built as a zip file. Within the file any folder hierachy can be used.

- Theme Meta Data
    - _theme.json (see below for valid JSON)
    - _theme.png (A 300x150 image that showcases the theme and will be displayed against the theme in the application Theme Manager)
- A master.css file used for HTML formatting, accompanyimng files for the master.css file may also be included (e.g. background.png files)
- Icons that make up the theme (see [Default Theme](system-themes/default/) for detail on the full list of icons)

## JSON content

### Example JSON

```json
{
    "theme": { 
        "name": "MMEX Default Theme",
        "author": "MMEX Team",
        "description": "This is the default MMEX theme and uses the MMEX colour scheme. It is a simple 'duo color' theme",
        "url": "https://github.com/moneymanagerex/moneymanagerex/blob/master/resources/themes/default/readme.md"
    },
    "colors": {
        "navigationPanel": "#F0F0F0",
        "listFutureDate": "#FF0000",
        "reports": {
            "credit": "#00FF00",
            "debit": "#FF0000"
        }
    }
}
```

### JSON Options supported

entry | Mandatory? | Default | Usage
--- | --- | --- | ---
/theme/name | Y | | The full theme name
theme/author | N | Empty | The name of the team or individual responsible for theme creation
theme/description | Y | | A short description of the theme
theme/url | N | Empty | A URL that links to more detail about the theme
/colors/navigationPanel | N | Empty |Color for the navigation panel background
/colors/listPanel | N | Empty | Color for the list panel background
/colors/listAlternative1 | N | #F0F5EB | Color for the list alternative row color (used in all but "All Transactions" view)
/colors/listAlternative2 | N | #E0E7F0 | Color for the list alternative row color (used in "All Transactions" view)
/colors/listTotal | N | #7486A8 | Color for total rows in list views
/colors/listBorder | N | #000000 | Color for list borders
/colors/listFutureDate | N | #7486A8 | Color for future transactions
/colors/reports/credit | N | #50B381 | Color for representing income/credits in reports
/colors/reports/debit | N | #F75E51 | Color for representing expense/debits in reports
/colors/reports/delta | N | #008FFB | Color for representing difference between income and expense in reports
/colors/reports/palette | N | #008FFB #00E396 #FEB019 #FF4560 #775DD0 #3F51B5 #03A9F4 #4cAF50 #F9CE1D #FF9800 #33B2DF #546E7A #D4526E #13D8AA #A5978B #4ECDC4 #81D4FA #546E7A #FD6A6A #2B908F #F9A3A4 #90EE7E #FA4443 #69D2E7 #449DD1 #F86624 | The range of colors used when drawing graphs in the reports
