# tilo


## Settings:

- `preventDoubleActive` (1/0) - Warning if want to add new active and there already is one active
- `linkLabels` (1/0) - Link the label to the ticket. Use together with `linkTemplate` and `labelsToLink`
- `linkTemplate` (url with placeholder) - URL to the ticket, placeholder `{label}` for the ticket number
- `labelsToLink` (oblejct with key: value pairs) - the ticket's project identifier. Key could be an abbreviation, but is the one used for the label in tilo. Value should be the correct project identifier, it's used for the actual link. 

## User instructions:
- Type "-" for an active item to reset the active time

## Bugs found:

- ...


## ToDo:

- Copy/paste of a long Jira issue key should transform to the shorter version
- Change tab index of linked Jira issue keys. Place first, so tabbing the time inputs is easier
- Hover item changes background or something
- Smaller favicons should only include the o✓
- Preliminary total time: If there is an active item, show the total if ended at current time
- List default items - add to tilo with a click
- Button to flash current total time when an item is still active. Round up to 5
- Format input: no, uppercase, lowercase
- A larger check above the list when all time is logged
- Drag-and-drop reordering the items
- Disable/hide update input when item is logged? Setting for that?
- Add new time to the update input for the item having the same label
- Automatically end active item if new active is added. Additional confirmation? Setting
- Type "-n:nn" to detract that amount of time from the item
- Sort items alphabetiacally. Sort Jira projects last?
- Checkboxes to toggle settings directly on the page
- Move logged items to the bottom of the list?
- Show latest reported time, i.e. active (if any) or latest end/interval
- Validation/Warning if want to add time > 8h, code to ignore already there
- Support for saving data for n days, e.g. mm-dd as index for all time data
- Move logged time (only amount? or abbr with text from .prev in title?) to other span to avoid counting it again, but still include it in the total amount
- Padding for rounding to closest 15 min
- Support for different separators instead of :
- Add comment feature, so notes can be added to an item after it was created
- Wrap times in separate buttons, so they are clickable and can be deleted
- Move settings to parameters in TILO.init()
- Bookmarklet to Chrome, so when a ticket is open in Jira, tilo opens with the ticket number prefilled (if not already in the list) or focused in update input (if exists) - is this even possible??
- Change messages to famous quotes about time
