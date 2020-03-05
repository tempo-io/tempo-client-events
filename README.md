# Tempo Plugin Client Side Events
## How to Use These Events
These events are emitted using the [trigger](https://docs.atlassian.com/aui/7.7.6/docs/trigger.html) element from the `aui-kit`.
​
You can listen for the following events by using
​
```javascript
    AJS.bind('EVENT STRING', function() {
        // What you want to do when this event is triggered
    })
```
## Current List of Available Events
### Log Work Form
- `logWorkOpened`
    - This event is triggered when the log work form is opened.
    - Note that this is triggered before all the inner elements has rendered in.
- `editLogWorkOpened`
    - This event is triggered when opening the log work for an already existing worklog.
    - If needed the worklog ID will be added to the `#worklogForm` element as a data-attribute named `data-worklog-id`.
    - Note that this is triggered before all the inner elements has rendered in.
