EasyStorage
=====

EasyStorage is a library for making it quicker and easier for XNA Game Studio developers to manage the StorageDevice without all the details. EasyStorage uses a simple API to enable you to add file saving to your game.

EasyStorage uses two simple interfaces called ISaveDevice and IAsycnSaveDevice to define "save devices" which are any object that can handle file operations. By default, EasyStorage comes with three ready-to-go save devices that implement both interfaces:

PlayerSaveDevice - a save device that uses the XNA storage APIs to manage a StorageDevice that is for a specific player
SharedSaveDevice - a save device that uses the XNA storage APIs to manage a StorageDevice that is shared for all players
IsolatedStorageSaveDevice - a save device that uses IsolatedStorage, intended for use on Windows Phone where StorageDevice is not available.

You can choose to use one of the above or build your own save devices from the code included in the library. Building new save device implementations gives you an easy way to interact with other code using EasyStorage while creating an implementation that meets your needs.

To download EasyStorage, head to the Source Code tab and download the version you want. There's an easy link in the top right for downloading the latest source.

The latest versions of EasyStorage have added resx files including localized strings to make it easier for developers to have localized dialogs in their games. However some developers may not want to include these strings as doing so requires the game to claim the particular language during peer review. You can now use the EasyStorageSettings class to set your supported languages, thereby limiting what languages your game must be reviewed under.
