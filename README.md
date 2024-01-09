# UDON-User-Verification
## VRChat Ban & Whitelist System for UDON Graph

## Overview

This project implements a Ban & Whitelist system using VRChat's UDON Graph Programming Language. The system enables world creators to control access to their worlds by preventing banned users from interacting and moving while allowing whitelisted users unrestricted access.

## Features

- **Ban System:** Automatically denies access to users on the ban list.
- **Whitelist System:** Grants specific users full access to the world and designated objects.
- **User Movement Control:** Restricts movement for banned users, ensuring compliance with world rules.

## Configuration Variables

- **WhiteList (String):** VRChat Trusted URL for the whitelist TXT file. Format: [GitHub](*.github.io), [Pastebin](pastebin.com), [Github Gist](gist.githubusercontent.com). File format: "white-list,username1,username2,username3," (no new lines).

- **BanList (String):** VRChat Trusted URL for the banlist TXT file. Format: [GitHub](*.github.io), [Pastebin](pastebin.com), [Github Gist](gist.githubusercontent.com). File format: "block-list,username1,username2,username3," (no new lines).

- **ObjectsToShowOnVerify (GameObject Array):** Array of objects to reveal to verified users.
- **ObjectsToHideOnVerify (GameObject Array):** Array of objects to hide from unverified users.
- **ObjectsToHideOnBan (GameObject Array):** Array of objects to hide when a user is banned.
- **BanLocation (GameObject):** Location to teleport the user on a ban event.

## Usage

1. Import the provided UDON Graph into your VRChat world.
2. Custom the ban list and whitelist by providing link to the WhiteList and BanList.
3. Configure object visibility and location parameters according to your world's requirements.
4. Deploy the system to manage user access in your world.

## VRChat Trusted URL

Ensure that the VRChat Trusted URL for the whitelist and banlist TXT files is correctly specified. Supported formats include GitHub (*.github.io), Pastebin (pastebin.com), and Github Gist (gist.githubusercontent.com).

## File Format

- **WhiteList TXT File Format:** "white-list,username1,username2,username3" (no new lines).
- **BanList TXT File Format:** "block-list,username1,username2,username3" (no new lines).

## Dependencies

- VRChat SDK
- UDON Graph

## Installation

1. Clone the repository or download the ZIP file.
2. Import the provided UDON Graph into your VRChat project.
3. Customize the system parameters as needed.

## Contributing

We welcome contributions! Feel free to submit issues, pull requests, or feature suggestions.

## License

This project is licensed under the [MIT License](LICENSE).

## Author

[Your Name]
