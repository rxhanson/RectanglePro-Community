# Rectangle Pro Community

Rectangle Pro is a closed source superset of the Rectangle macOS app for window management. 

Since Rectangle Pro is a separate app with much more functionality, this repository is for issues and discussions specifically related to Rectangle Pro.

The [terminal commands for hidden settings in Rectangle](https://github.com/rxhanson/Rectangle/blob/master/TerminalCommands.md) can also be applied to Rectangle Pro, but you have to change "com.knollsoft.Rectangle" to "com.knollsoft.Hookshot".

[FAQ/Discussions](https://github.com/rxhanson/RectanglePro-Community/discussions)

## Programmatically triggering window sizes & positions

You can programmatically trigger any of the Rectangle Pro actions using urls. 

Here are some examples:

For options that already exist, like left half: 

`open -g "rectangle-pro://execute-action?name=left-half"`

For application layouts you've created, use the name you gave it

`open -g "rectangle-pro://execute-layout?name=applayout1"` 

For custom shortcuts you've created, also use the name you gave it

`open -g "rectangle-pro://execute-custom?name=custom1"`
