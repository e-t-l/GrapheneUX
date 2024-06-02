# Enable hidden Pattern lockscreen

1. Connect ADB from a computer, or by using an [on-device ADB shell](https://github.com/e-t-l/GrapheneUX/blob/main/On-device%20ADB.md)
2. Decide on your new lock pattern, where the grid of nine dots corresponds to numbers 1-9 on a phone dialpad (see below)
3. In an ADB shell, execute: `locksettings set-pattern --old {old pin/password} {new pattern}
4. Note: The pattern unlock option will still be hidden under Settings app > Security > Screen lock. If you want to change it back to a pin or password, you can use the Settings app, but to change the pattern you must repeat this ADB command.

### Reference for pattern dot grid:
```
1  2  3
4  5  6
7  8  9
```

### Example
If your current PIN is "12345" and you want your new lock pattern to be "start in upper right corner, trace counterclockwise around perimiter of grid, ending on the dot underneath the starting dot", you would enter...

`locksettings set-pattern --old 12345 32147896`
