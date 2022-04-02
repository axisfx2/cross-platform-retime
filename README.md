# Cross Platform Retime

* Description: Export time remap values from After Effects and import them into other application(s)
* Copyright: AXISFX LTD
* Author: Ewan Davidson
* Email: ewan@axisfx.design
* Release Date: 02.04.2022
* Current Version: 1.0.0

## Installation

* Click the green 'Code' button
* Click 'Download ZIP'
* Copy 'export_retime_data.jsx' to your After Effects installs '/Support Files/Scripts/ScriptUI Panels' folder
* Copy 'afx_retime' to houdinixx.x/otls (Houdini user preferences folder)
* Data is also supported in the Cinema 4D [Alembic Retime](https://github.com/axisfx2/abc_retime) plugin

## Troubleshooting

* Make sure your frame rates are consistant across each application

## Adding support for other DCCs

The data saved from After Effects is just a plain text list of frame numbers ie [0, 1, 2.5, 3].<br>
You could easily add support for other DCC's. Simplest method would be to use Json, then convert the string data into a list object:<br>
Python: json.loads(data)<br>
Extend Script/ Java: json.parse(data);

## Changes

### 1.0.0   |  02.04.2022  |   ED

* Initial release