# Disable requiring a lock PIN for the Work Profile

1. In the Settings app > Security & Privacy > More Security & Privacy, disable "Work profile: Use one lock." (This will require you to set a separate PIN or password for the work profile; it doesn't matter since you will be disabling it immediately, so a PIN of `0000` is fine, for example.)
2. Connect ADB from a computer, or by using an [on-device ADB shell](https://github.com/e-t-l/GrapheneUX/blob/main/On-device%20ADB.md)
3. Double-check the User ID of your Work Profile. (It's usually `10`, but you can check by running the ADB command `pm list users`).
3. In an ADB shell, execute: `locksettings clear --old {old pin/password} --user {work profile user ID}`.
4. Note: The pattern unlock option will still be hidden under Settings app > Security > Screen lock. If you want to change it back to a pin or password, you can use the Settings app, but to change the pattern you must repeat this ADB command.

### Example
If your work profile's user ID is `10` and you set its PIN to `0000`, you would enter...

`locksettings clear --old 0000 --user 10`
