# Steam Discount v1.0

## Installation
Install from iCloud link: [https://www.icloud.com/shortcuts/4950398c8a4f4a618aa0f255c0a2a3ff](https://www.icloud.com/shortcuts/4950398c8a4f4a618aa0f255c0a2a3ff)

**Note**: If you are on iOS 14 or lower, you must allow untrusted shortcuts in order to import this shortcut. To find out how, see [https://support.apple.com/guide/shortcuts/enable-shared-shortcuts-apdfeb05586f/4.0/ios/14.0](https://support.apple.com/guide/shortcuts/enable-shared-shortcuts-apdfeb05586f/4.0/ios/14.0). 

Install manually by saving `Steam Discount.shortcut`. Then, import it by opening the file. 

## Usage
The purpose of this shortcut is to notify you if certain Steam games of your choosing are currently on sale. For each discounted game, it will display the discount percentage along with the price before and after the discount. *No log in required.* 

Before use, please configure the shortcut. The setup screen should pop up after importing, but if it does not, it can be found in `Details` > `Setup`. You may also manually configure the shortcut by modifying the following variables: `AppList`, `CC`, and `Currency`.  
- `AppList` is a list of the AppIDs of the Steam products you would like to track for discounts. A Steam AppID can be found in its corresponding Steam URL. For example, in "https://store.steampowered.com/app/730/" the AppID is 730. You may use my shorcut [Copy Steam AppID from URL](https://github.com/MalihaTarafdar/ios-shortcuts/tree/main/copy-steam-appid-from-url) to copy the AppID from the share sheet of the Steam product page. Alternatively, you may find the AppID of a Steam product on [SteamDB](https://steamdb.info/instantsearch/). 
- `CC` is the region in which you would like to check prices, specified as a two-letter country code as defined in [ISO 3166-1](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2#Officially_assigned_code_elements). 
- `Currency` is the currency in which you would like to view prices, specified as a three-letter currency code as defined in [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217#List_of_ISO_4217_currency_codes). 

Furthermore, though not required, this shortcut is intended to be used in an iOS Automation as manually checking for discounts defeats the purpose of being notified. A new Personal Automation may be created by the following steps in the Shortcuts app:
1. Click the `Automation` tab. 
2. Click the `+` button in top right corner of the screen. 
3. Click the `Time of Day` option. 
4. Set `When` to the time of day you would like this shortcut to check for discounts and notify you. 
5. Set `Repeat` to how frequently you would like to be notified. 
6. Select the `Run Immediately` option at the bottom. 
7. Click `Next`. 
8. Find this shortcut and select it. 

If you would like to check for discounts at different intervals than a single automation allows, you must create multiple automations. For example, checking hourly would require a different automation for every hour of the day. Since Steam rarely has unreasonably short sales, checking once or twice a day at most is sufficient. 

## Limitations
Please note that if none of the specified games are on sale, the shortcut will produce no output. Also, the shortcut will continue to notify you if a game is on sale even if it already has unless you manually remove it from the list. This requires you to modify the `AppList` variable in the shorcut as specified below. In the future, I may utilize persistent data storage to eliminate the need to manually modify the shortcut and solve the problem of being re-notified about the same exact discount. 

## Use Cases
You may be wondering why use this shortcut if Steam notifies you on sales for items on your wishlist. The following are some use cases for this shortcut. 

1. You wish to track sales for products that you do not wish to put on your Steam wishlist (e.g. gifts). 
2. You wish to track sales for products you already own on your Steam account, so you cannot put them on your Steam wishlist. 
3. Your Steam wishlist is too long and notifications from Steam about sales are no longer specific and require you to open the app to view them. 
4. You do not wish to install the Steam app on your device and would like a lightweight discount tracker. 

## Support Me
This shortcut along with others I have made are open source and can be found at [https://github.com/MalihaTarafdar/ios-shortcuts](https://github.com/MalihaTarafdar/ios-shortcuts). If you found this shortcut useful, please consider supporting me at [coindrop.to/malihatarafdar](https://coindrop.to/malihatarafdar)!
