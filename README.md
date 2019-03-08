# RichEditBoxFontTest
Simple app to repro how UWP responds to new system fonts, installed during runtime.

## Repro steps

1. Install the included font: `./great-vibes/GreatVibes-Regular.otf`
1. Load the solution in Visual Studio. F5 to build and deploy.
1. Write text to the RichEditBox and use the `Save` button to save a copy.
1. Close the app.
1. Uninstall the font from step 1.
1. Relaunch the app and use the `Open` button to restore the document from step 3.
1. Observe that the GreatVibes font is not present.
1. Repeat step 1 to reinstall the font.
1. Observe that the GreatVibes font is still not present.
1. Click the 'Reload in new view' button.
1. Observe that the GreatVibes font is now present in the new window instance.
