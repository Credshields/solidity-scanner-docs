# SolidityScan Visual Studio Code Extension

We also provide Visual Studio Code extension that has scanning capabilities for Solidity smart contracts. It allows you to scan a single .sol file or an entire workspace and gives a security profile for your contract with a security score, vulnerability distribution according to criticality levels & highlights the lines of code containing the vulnerabilities.

#### Features

- Scan Current File: Allows you to scan the open Solidity file for vulnerabilities.
- Scan Entire Workspace: Allows you to scan the all the solidity files in the existing workspace for a comprehensive security profile.
- Vulnerability distribution: Displays all types of vulnerabilities detected in the file distributed according to criticality levels.
- Detailed results: Shows descriptions & remediations for the detected vulnerabilities along with highlighting the piece of code where they are present.
- Gas optimizations: Gives you possible ways of optimising your Solidity files for gas.

Please see the following example to get an understanding on how to use the extension.

![VSCode Demo](./assets/images/vscode-demo.gif)

#### Prerequisites

Visual Studio Code version 1.54.0 or later.

#### Installation

Install the extension from the Visual Studio Code Marketplace.
Reload or restart Visual Studio Code.

#### Configuration

To use SolidityScan, you may configure an API Access Token for authentication.

1. Open Visual Studio Code settings (File > Preferences > Settings or `Ctrl + ,)`.
2. Search for "SolidityScan" and set the `solidityscan.apiToken` property with your API Access Token.

#### Usage

##### Commands

- Scan Current File: Ctrl+K Ctrl+S (macOS: Cmd+K Cmd+S)
- Scan Entire Workspace: Ctrl+K Ctrl+Alt+S (macOS: Cmd+K Cmd+Option+S)

##### Explorer View

SolidityScan provides an explorer view in the activity bar with the 'Analysis' view. When an API token is provided, it displays a breakdown of vulnerabilities:

- Critical
- High
- Medium
- Low
- Informational
- Gas
