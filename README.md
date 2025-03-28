# Tennis Activities Filter

A client-side web application for filtering tennis activities based on various criteria. This application provides a natural language interface for filtering activities by court type, group size, age group, skill level, and other attributes.

## Live Demo

Access the live application at [https://dncfwtec.github.io/fwtec-activities/](https://dncfwtec.github.io/fwtec-activities/)

## Features

- **Natural Language Filtering**: Intuitive sentence-based filtering interface
- **Multi-select Options**: Select multiple criteria for ball type, technical focus, etc.
- **Interactive Activity Cards**: Results display detailed information in card format
- **Responsive Design**: Works on mobile, tablet, and desktop devices
- **Data Management Tools**: Includes pages for adding and editing activities

## Pages

- **index.html**: Main filtering interface
- **tennis-activities-add.html**: Form for adding new activities
- **tennis-activities-edit.html**: Form for editing existing activities

## Data Structure

The application uses a separate JSON file (`tennis-activities-data.json`) that contains all the activities and their attributes. Each activity has the following structure:

```json
{
    "Activity Name": "Name of activity",
    "Description": "Description of activity",
    "Purpose": "Purpose of the activity",
    "Duration": "15-20 minutes",
    "Variations": "Possible variations",
    "Court Setup": "one court or multiple courts",
    "Group Size": "4-10 or 10-16",
    "Court Type": "mini or standard",
    "Student Grade Level": "Elementary, Middle, or High",
    "Skill Level": "beginners only, mixed skills, or returners only",
    "Ball Red": true or false,
    "Ball Orange": true or false,
    "Ball Green/Yellow": true or false,
    "FH Focus": true or false,
    "BH Focus": true or false,
    "Rally Building": true or false,
    "Volley": true or false,
    "Overhead": true or false,
    "Serve": true or false,
    "Point Play": true or false,
    "Consistency": true or false,
    "Footwork": true or false,
    "Sportsmanship": true or false,
    "Teamwork": true or false,
    "Problem-solving": true or false,
    "Positive Reinforcement": true or false
}
```

## How to Use

### Filtering Activities

1. Visit the main page
2. Use the dropdown menus to select court type, group size, etc.
3. Select any additional criteria using the multi-select options
4. Click "Find Tennis Activities" to filter the results
5. View matching activities in the cards below

### Adding New Activities

1. Navigate to the "Add Activity" page
2. Fill out all required fields
3. Click "Generate JSON" to create the JSON for the new activity
4. Copy the generated JSON and add it to the `tennis-activities-data.json` file

### Editing Activities

1. Navigate to the "Edit Activity" page
2. Select an activity from the dropdown or paste existing JSON
3. Modify any fields as needed
4. Click "Update JSON" to generate the updated JSON
5. Copy the updated JSON and replace the corresponding entry in the data file

## Development

### Modifying the Interface

The application uses plain HTML, CSS, and JavaScript. To modify the interface:

1. Edit the HTML files to change structure
2. Modify the CSS in the `<style>` section to change appearance
3. Update the JavaScript in the `<script>` section to alter behavior

### Adding New Filter Categories

To add new filter categories:

1. Add new properties to the activity objects in the JSON file
2. Add corresponding filter UI elements to the HTML
3. Update the filtering logic in the JavaScript

## License

This project is available for use with proper attribution.

## Acknowledgements

Created for Fred Wells Tennis & Education Center to help coaches find appropriate tennis activities for different teaching scenarios.
