# AndroidTestActivityIsKilled

### Note
- We can tested activity is killed by enable mode `Don't keep activity` inside Developer Setting

- If have a variable and it don't initialize inside onCreated we may got some NullPointerException. For example,
in case we leave this Activity and this Activity is destroyed by system, when we go back to this Activity, Activity will recreate
but our variable is null (because it not initialize in onCreate) so we may have NullPointerException. If we always use dependencies injection,
 we can prevent it