# VRChat User Verification/Control System

Welcome to the VRChat User Verification/Control System, a Unity-based solution which work using the VRChat Udon Graph Node Programming Language designed to manage user access in VRChat worlds.
This system consists of three modules: WhiteList Module, BlackList Module, and Combined Module (Alpha Version, can be buggy).

## WhiteList Module

The WhiteList Module allows world creators to control access based on a predefined list of trusted users. Utilizing the following variables:

- **WhiteList (String):** VRChat Trusted URL for the whitelist TXT file.
- **Enable Objects (GameObject Array):** Array of objects to reveal to verified users.
- **Hide Objects (GameObject Array):** Array of objects to hide from verified users.

## BlackList Module

The BlackList Module allows world creators to restrict access for users on a predefined ban list. Key variables include:

- **BlackList (String):** VRChat Trusted URL for the blacklist TXT file.
- **Hide Objects (GameObject Array):** Array of objects to hide from users on the blacklist.
- **VRC World (VRC World Object):** Sets the player respawn location to be the same as BanLocation.
- **BanLocation (GameObject):** Location to teleport the user on a ban event.

## Combined Module (Alpha Version, can be buggy)

The Combined Module integrates both the WhiteList and BlackList modules into a unified system, providing a comprehensive solution for managing user access in VRChat worlds. Key variables include:

- **WhiteList (String):** VRChat Trusted URL for the whitelist TXT file.
- **BlackList (String):** VRChat Trusted URL for the blacklist TXT file.
- **ObjectsToShowOnVerify (GameObject Array):** Array of objects to reveal to verified users.
- **ObjectsToHideOnVerify (GameObject Array):** Array of objects to hide from verified users.
- **ObjectsToHideOnBan (GameObject Array):** Array of objects to hide when a user is banned.
- **BanLocation (GameObject):** Location to teleport the user on a ban event.
- **VrcWorldObject (GameObject):** Sets the player respawn location to be the same as BanLocation.

## VRChat Trusted URL

Ensure that the VRChat Trusted URL for the whitelist and banlist TXT files is correctly specified. Supported formats include:

- [GitHub](*.github.io)
- [Pastebin](pastebin.com)
- [Github Gist](gist.githubusercontent.com)
- [Raw GitHub](raw.githubusercontent.com)

- Make sure the URL is an absolute URL and not a blob or URL to a page containing TXT File.

## File Format

- **WhiteList TXT File Format:** "white-list,username1,username2,username3" (no new lines).
- **BanList TXT File Format:** "block-list,username1,username2,username3" (no new lines).
- Supports formats: [GitHub](*.github.io), [Pastebin](pastebin.com), [Github Gist](gist.githubusercontent.com).
- File format: "white-list,username1,username2,username3," (no new lines).

## Dependencies

- VRChat SDK
- UDON Graph

## Installation

1. Clone the repository or download the ZIP file or Unity Package.
2. Import the provided Folder into your unity project under assets or right click on assets then click on import custom package and select the provided Untiy Package.
3. Select the module that suits your needs, and draga and drop it into your World Heirarchy.
4. Provide the information that is required by the Udon Behaviour Component in the module/prefab and you are done.

### Usage of Modules

Choose the module that suits your requirements or use multiple modules for a comprehensive solution:

#### WhiteList Module

- **Import the Prefab:** Drag and drop the provided `WhiteListModule` into your scene.
- **Add Component to Existing GameObject:** Click on an existing GameObject in your scene, then click on "Add Component." Search for the Udon Behaviour, and drag & drop the `WhiteListModule` script into the component to add it. (Only if the imported prefab doesn't contain the UDON Behaviour)
- **Create New Empty Object:** Create a new empty GameObject in your scene, then click on "Add Component." Search for the Udon Behaviour, and drag & drop the `WhiteListModule` script into the component to add it. (Only if the imported prefab doesn't contain the UDON Behaviour)

#### BlackList Module

- **Import the Prefab:** Drag and drop the provided `BlackListModule` into your scene.
- **Add Component to Existing GameObject:** Click on an existing GameObject in your scene, then click on "Add Component." Search for the Udon Behaviour, and drag & drop the `BlackListModule` script into the component to add it. (Only if the imported prefab doesn't contain the UDON Behaviour)
- **Create New Empty Object:** Create a new empty GameObject in your scene, then click on "Add Component." Search for the Udon Behaviour, and drag & drop the `BlackListModule` script into the component to add it. (Only if the imported prefab doesn't contain the UDON Behaviour)

#### Combined Module (Alpha Version)

- **Import the Prefab:** Drag and drop the provided `CombinedModulePrefab` into your scene.
- **Add Component to Existing GameObject:** Click on an existing GameObject in your scene, then click on "Add Component." Search for the Udon Behaviour, and drag & drop the `CombinedModule` script into the component to add it. (Only if the imported prefab doesn't contain the UDON Behaviour)
- **Create New Empty Object:** Create a new empty GameObject in your scene, then click on "Add Component." Search for the Udon Behaviour, and drag & drop the `CombinedModule` script into the component to add it. (Only if the imported prefab doesn't contain the UDON Behaviour)

Customize the system parameters for each module according to your specific world's requirements. Enjoy flexible user access control with the VRChat User Verification/Control System!

## Credits

If you find this VRChat Ban & Whitelist System useful in your project, please consider giving credit:

- Author: Kunal Kashyap, Discord: @nommiiee, VRChat: {NomNom}
- GitHub: [Nommiiee](https://github.com/Nommiiee/)

Your acknowledgment is greatly appreciated! Thank you for using the VRChat User Verification/Control System. Or you can simply put the Credits Prefab included in the package/zip in your world.

## Credits Prefab

Included in this package is a Credits Prefab featuring a photo frame for easy integration into your VRChat world. This prefab provides a visually appealing way to display credits for the VRChat User Verification/Control System.

### Installation

1. Drag and drop the provided `CreditsPrefab` into your scene.

### Usage

Place the Credits Prefab in a visible location within your world to acknowledge the contributors and authors of the VRChat User Verification/Control System. You are also free to edit the Credits Prefab to customise it to your world theme. But please don't change the image, keep it as it is, you can customise the Frame, Colour, Design and other aspects of it.

## Contributing

We welcome contributions! Feel free to submit issues, pull requests, or feature suggestions.

## License

This project is licensed under the [MIT License](LICENSE).

## Author

[Kunal Kashyap/Nommiiee/{NomNom}]
