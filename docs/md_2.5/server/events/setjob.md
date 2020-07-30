# ESX.CreatePickup

```lua
AddEventHandler('esx.setjob', function(source, job, lastjob)

end)
```

Gets called when a players job gets updated

#### `data` Table Information

| child          | type    | explanation                                                                                        |
|----------------|---------|----------------------------------------------------------------------------------------------------|
| source         | number  | The client id of the player                                                                        |
| job            | table   | new job of player                                                                                  |
| lastjob        | table   | old job of player                                                                                  |
