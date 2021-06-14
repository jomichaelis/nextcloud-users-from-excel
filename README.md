# Nextcloud-Users-From-Excel

This is a short python-script for converting an excel-sheet to api-calls for creating nextcloud-users.

User information include
- userID
- password
- email
- displayName
- groups (only if already existing)
- quota
- language

## Install
It is recommended to use venv to create an environment just for this project, but to necessary.

```sh
pip install requirements.txt
```

## Using your Nexctloud

Create a .env-file inside the root-folder of this project and set it up like env.sample.
You need to provide your username, the URL of your Nextcloud-Installation and an app-password.
Create one by navigating to "Settings" -> "Security".

## Using the Excel-sheet

Open your Excel-Sheet and make your changes. Watch out though! Excel creates a temporary ~$users.xlsx-file and uses this one while the excel-window is opened. Only when you close it, changes will be written to the actual file users.xlsx and thus be visible for the python-script.

## License
MIT
