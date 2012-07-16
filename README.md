alfred-count
============

## Count characters and words with Alfred.app

### With Alfred

Invoke Alfred, type the keyword *count* followed by the string of text you want to measure and hit *return*

### Anywhere else
For example in TextEdit select a line of text and hit *control + space*.

Both ways will show the result in a Growl notification.

## Known Issues
If your string contains any of these characters <strike>the whole thing comes crashing down.</strike> Well, let’s say the results are off.

- ' (single quote) doesn't work at all, Growl will not show a notification.
- # (pound/number sign) counts as 2 characters
- ¥ counts as 2 characters
- sometimes does not work on text with multiple lines. This may have to do with the characters listed above
- spaces at start or end are not included when invoked in Alfred. They are included if invoked in an other app like TextEdit. (Whyyyy?)

Also note that if Growl isn’t running, this will not work. Nothing happens. Obviously. Thing is, I tried adding a check to see if Growl is running and if not show an AppleScript dialog showing either the result or saying you need Growl, but I could not get it to work – yet.
