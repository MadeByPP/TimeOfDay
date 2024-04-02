This is a fork of the TimeOfDay plugin on uMod.

[https://umod.org/plugins/time-of-day](https://umod.org/plugins/time-of-day)

## Differences from uMod version
- A TimeOffset option is provided in the configuration to change the night start time and day start time.

## FAQ

#### Do I need to reset my config to use this fork?

No, existing configs will work.

#### The offset time does not seem to be correct.

This phenomenon occurs because when time is a condition, it is checked in hourly increments and when the time changes, it changes immediately.

For example, 'Change to morning at 19:45.' is a condition
and 'If night is skipped, change morning to 7:25.' is a time change.

That's because of limitations in the way this plugin works.
