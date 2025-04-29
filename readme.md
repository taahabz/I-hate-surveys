# Qalam Survey Auto-Fill Scripts

A set of Tampermonkey scripts for automatically detecting and filling out feedback surveys in the Qalam NUST student portal.

## Features

- **Auto-Detection**: Automatically detects unsubmitted surveys on your dashboard
- **Auto-Fill**: Fills all radio button questions with the first option (can be customized)
- **Auto-Comment**: Adds a default comment of "Good" (can be customized)
- **Auto-Submit**: Submits the survey after filling
- **Auto-Navigation**: Returns to the feedback page to process the next survey

## Installation

### 1. Install Tampermonkey

First, you need to install the Tampermonkey browser extension:

- [Chrome Web Store](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo)
- [Firefox Add-ons](https://addons.mozilla.org/en-US/firefox/addon/tampermonkey/)
- [Microsoft Edge Add-ons](https://microsoftedge.microsoft.com/addons/detail/tampermonkey/iikmkjmpaadaobahmlepeloendndfphd)



### 2. Install the Scripts

1. Click on the Tampermonkey icon in your browser and select "Create a new script"
2. Delete all the template code 
3. Copy and paste the first script (Survey Detection) into the editor
4. Save the script (Ctrl+S or File > Save)
5. Repeat steps 1-4 for the second script (Survey Auto-Fill)

## How to Use

1. Log in to your Qalam NUST account
2. Navigate to the feedback page: `https://qalam.nust.edu.pk/student/qa/feedback`
3. The scripts will automatically:
   - Detect unsubmitted surveys
   - Open the first one
   - Fill in all required fields
   - Submit the survey
   - Return to the feedback page to process the next one
4. Wait for all surveys to be completed

## Customization

### Changing the Rating (Radio Button Selection)

By default, the script selects the first option for all radio button questions. To change this behavior, edit the following section in the Survey Auto-Fill script:

```javascript
// Find this section in the second script
for (const [index, row] of rows.entries()) {
    const radios = row.querySelectorAll('input[type="radio"]');
    if (radios.length > 0) {
        radios[0].checked = true;  // Change the index [0] to select different options
        // For example: radios[4].checked = true; // This would select the last (5th) option
        radios[0].dispatchEvent(new Event('change', { bubbles: true }));
        console.log(`✅ Selected first option for row ${index + 1}`);
    } else {
        console.warn(`⚠️ No radio buttons found in row ${index + 1}`);
    }
}
```

To select different rating options:
- `radios[0]` = First option (leftmost radio button)
- `radios[1]` = Second option
- `radios[2]` = Third option
- And so on...

### Changing the Comment

To change the default comment from "Good" to something else, modify this line in the Survey Auto-Fill script:

```javascript
// Find this line in the second script
commentField.value = "Good";  // Change "Good" to your preferred comment
```

## Troubleshooting

If the scripts are not working as expected:

1. **Check Console Logs**: Both scripts have detailed logging. Press F12 to open browser developer tools and check the console for error messages.

2. **Survey Structure Changed**: If Qalam updates their survey structure, the scripts may need to be updated.

3. **Script Conflicts**: Make sure you don't have other scripts that might interfere with these.

4. **Manual Intervention**: Some surveys may have unique structures that require manual intervention.

## Important Notes

- These scripts are for educational purposes and to save time on repetitive tasks
- Use them responsibly and ethically
- The scripts work as of April 2025, but may need updates if Qalam changes their interface

## License

This project is released under the MIT License - see the LICENSE file for details.

## Acknowledgements

- Created with assistance from GPT
