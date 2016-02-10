#Gradient Swatches
This script calculates intervals between two RGB colors, creates swatches for those colors, and builds a table gradient.  A few things of note:

##In the dialog:
- The user chooses a gradient name.
- The user may choose how many steps they wish to calculate between the colors.
- Both text boxes and sliders are available the color’s RGB and HSL. The HSL calculations are made as the RGB is manipulated (sliders and text input updated), and vice versa with HSL changes.
- A preview of the chosen swatch color appears on the right and is updated immediately as numbers are entered or sliders are moved.
- If the user enters an invalid number in the RGB or HSL text boxes (e.g. the user enters more than three numbers or a number greater than 255 in the RGB box), the box will turn red.
- The user chooses the height of the table.
- The user may choose to enter in a particular table width OR allow the script to calculate the page width (allowing for the page margins) and create a table that fills that width.

![Gradient Table Dialog Screenshot](https://cloud.githubusercontent.com/assets/13002217/12951646/521e51b4-cfe1-11e5-97ca-66362fb58df1.png)

##Features of the table:
- A swatch for each calculated color is created and given the name of its RGB calculation (R/G/B).
Duplicate swatches are automatically detected and deleted.
- If a swatch already exists in the swatches panel, the script will apply that swatch and will not create a duplicate.
- The script creates the gradient by making the appropriate number of table cells for each calculated step (plus one for a "title cell"). Every cell in the table gradient has a color swatch applied as a background and its name (the RGB recipe) created as its content.
- Text color of the R/G/B depends on the color’s brightness. If it is less than 130, the text will be white; otherwise, the text will be black.
- The “title cell”, the left-most column, is not given a background color. It includes the user’s chosen name for the gradient AND the date the gradient was created.
- The text frame is automatically fitted to the table.

Yes, there are lots of little steps, so the script features an UNDO function as well! 

Hope this is useful, and let me know if you have any suggestions or edits.

![Gradient Table ScreenShot1](https://cloud.githubusercontent.com/assets/13002217/12951630/36fea636-cfe1-11e5-9eb9-6f20ec95d2d3.png)

![Gradient Table ScreenShot1](https://cloud.githubusercontent.com/assets/13002217/12951649/5a253404-cfe1-11e5-874f-ac4bc7e0c7e7.png)
