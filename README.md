# FreadomBubblePicker
We imported the original library of BubblePicker (https://github.com/igalata/Bubble-Picker) as a module to customise the original library according to our design and animation needs. Please refer to origin library in case of any queries or amendments.


Note: If our project uses slf4j-logging library and causes problem while compiling, follow the steps below.

1. Exclude it in the gradle.
```implementation('com.github.Grappus:FreadomBubblePicker:1.0.1') {
        exclude module: 'slf4j-log4j12'
    }
```

 2. View the project structure in "Project" mode. Check the `External Libraries` and search for `com.github.Grappus:FreadomBubblePicker:1.0.1` (the bubble picker library) and delete the `slf4j-log4j12` from it.

3. Clean project, rebuild it and voila! It should work.
