# ReleaseNotifications

Release Notification content is in JSON file. It must be provided separately for each Magento version, edition, and locale. For each version, a default.json file should be provided. The files must be placed under the following file structure.
```text
root
  \version (2.2.2|2.3.0)
      \edition (Community|Enterprise)
		 \locale.json (en_US.json|fr_Fr.json)
      \default.json
```
* "**version**" = The Magento version that the client has installed (ex. 2.2.2). Detected via the Magento installation's Product Metadata.
* "**edition**" = The Magento edition that the client has installed (ex. Community/Enterprise/B2B). Detected via the Magento installation's Product Metadata.
* "**locale**" = The chosen locale of the admin user (ex. en_US). Detected via the admin user's Interface Locale setting via the admin user's login Session.
