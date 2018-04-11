# Instructions to configure your mac keyboard correctly for British keyboards.

## Instructions for keyboard layouts

>I’m used to proper British keyboards, and I expect my ‘#’, ‘"’ and ‘@’ to be in their usual places. Apple seems to think differently about the matter, with their bastardised excuse of a ‘British’ keyboard.

Here are a couple of keyboard layout files you can simply unzip, and move to the /Library/Keyboard Layouts folder. (Create the folder if it’s not there already.) You’ll need to log out and back in for the new layouts to become available. In certain situations you might find the ‘`’ and ‘\’ keys to be swapped, in which case the alternative layout is the one for you.

These instructions and files are taken from [the rather eccentric sicte of Liyang Hu.](http://liyang.hu/#osx-survival,osx-british,index)

I am documenting them here for posterity.

## Instructions to configure correct Home and End key behaviour

- Copy the KeyBindings folder into your ~/Library folder.
- Restart your mac.

### DefaultKeyBinding.dict

```c
{
/* Remap Home / End keys */
/* Home Button*/
"\UF729" = "moveToBeginningOfLine:"; 
/* End Button */
"\UF72B" = "moveToEndOfLine:"; 
/* Shift + Home Button */
"$\UF729" = "moveToBeginningOfLineAndModifySelection:"; 
/* Shift + End Button */
"$\UF72B" = "moveToEndOfLineAndModifySelection:"; 
/* Ctrl + Home Button */
"^\UF729" = "moveToBeginningOfDocument:"; 
/* Ctrl + End Button */
"^\UF72B" = "moveToEndOfDocument:"; 
 /* Shift + Ctrl + Home Button */
"$^\UF729" = "moveToBeginningOfDocumentAndModifySelection:";
/* Shift + Ctrl + End Button*/
"$^\UF72B" = "moveToEndOfDocumentAndModifySelection:"; 
}
```