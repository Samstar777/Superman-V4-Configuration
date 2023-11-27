# Superman-V4-Configuration

Explore the power of S.U.P.E.R.M.A.N. Version 4 with the configuration repository! This repository houses the JSON configuration file containing preference settings for the Software Update Policy Enforcement tool designed for Mac administration.

## Overview
Welcome to the Superman V4 Configuration repository! This repository contains the preference settings for S.U.P.E.R.M.A.N. Version 4, a powerful Software Update Policy Enforcement tool designed for Mac administration by Kevin M White

**Disclaimer:** Be cautious when modifying configuration settings, especially in production environments. Always refer to the [official documentation](https://github.com/Macjutsu/super/wiki) for detailed information on each setting.

## Contents

- [Configuration File](#configuration-file)
- [Usage](#usage)
- [License](#license)

## Configuration File

The main configuration file is `superman_v4_config.json`. This file includes various settings that govern the behavior of S.U.P.E.R.M.A.N., such as authentication details, deferral timers, deadline counts, display options, and more.

## Usage

Follow these steps to create a custom schema configuration profile:

 1. Access Configuration Profiles:

    - Launch Jamf Pro and navigate to the "Computers" section in the sidebar.
    - Click on "Configuration Profiles" within the sidebar.
    - Select the "New" button to initiate the creation of a new configuration profile.

 2. Choose Payload Type:

    - In the "New Configuration Profile" window, provide a name for your profile, such as "Custom Schema Configuration."
    - Click the "Add" button located under the "Payloads" section.
    - Select "Application & Custom Settings" from the "Payload Type" drop-down menu.
    - Click the "Select" button to proceed.

 3. Configure Application & Custom Settings:

    - In the "Application & Custom Settings" payload configuration window, select external application and Add and select the custom schema.
    - Download the "superman_v4_config.json" from github
    - "Custom Schema": paste the JSON schema code into the provided text box and populate the preference domain info from the json file.
    - Click "Save" to finalize the configuration.

 4. Define Custom Settings:

    - Expand the "Custom Settings" section and locate the desired setting to configure.
    - Click the associated checkbox to enable the setting.
    - Provide the desired value for the setting.
    - Repeat these steps for any additional settings you want to configure.
    - for more info, refer [Youtube Vudeo](https://youtu.be/fkb-IhcCgoo?si=YKJY7P4QoMMSK1yv)

 5. Scope the Profile:

    - Switch to the "Scope" tab of the configuration profile window.
    - Select the desired scope for the profile, such as a specific computer group or all computers.
    - Click "Save" to finalize the configuration profile.

 6. Deploy the Profile:

    - Click the "Deploy" button in the configuration profile window.
    - Select the desired deployment method, such as "Smart Distribution" or "Manual Install."
    - Click "Deploy" to distribute the profile to the specified targets.


### Once the configuration profile is deployed, the defined custom settings will be applied to the specified application for the targeted devices.

