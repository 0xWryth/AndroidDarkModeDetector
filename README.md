# AndroidDarkModeDetector

Steps to reproduce (on Android Studio)
- Create a new value value ressources file nammed "colors" in the "values" folder (select the night mode qualifier and set it to "night")
- Use the following code to detect the UI mode
```java
switch (getResources().getConfiguration().uiMode & Configuration.UI_MODE_NIGHT_MASK) {
	case Configuration.UI_MODE_NIGHT_YES:
		// Dark mode
		break;
	case Configuration.UI_MODE_NIGHT_NO:
		// Light mode
		break;
}
```
