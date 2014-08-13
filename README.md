TestRail Custom Passed Status
============================

A TestRail UI Script to account for custom passed tests status when calculating percentages for completion.

Install
-------

1. As an administrator, navigate to Administration -> Site Settings -> API and check the 'Enable session authentication API' check box.

2. Click 'Save Settings'

3. As an administrator, navigate to Administration -> Customizations.

4. Scroll down to UI Script and click Add UI Script.

5. Copy the contents of the testrail_custom_passed_status_ui_script file into the UI script.

6. Edit the configuration to include all Status' that should be considered a passed state.

7. Save the changes.

Notes
-----

- This script runs all requests asynchrounsly so that page load times are less affected. If could take a few seconds to full update some pages if there are a lot of callous to make. If you do not care about page load times, you can edit the configuration to set `async_requests=false`.

- This script was tested on Chrome using TestRail Version 3.1.3.3146.