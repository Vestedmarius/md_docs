# esx:setjob

```lua
AddEventHandler('esx:setjob', function(source, job, lastjob)

end)
```

Gets called when a players job gets updated

#### `parms` Table Information

| child          | type    | explanation                                                                                        |
|----------------|---------|----------------------------------------------------------------------------------------------------|
| source         | number  | The client id of the player                                                                        |
| job            | table   | new job of player returns [job table](https://vestedmarius.github.io/md_docs/md_2.5/server/xplayer/data/job)                                                                                 |
| lastjob        | table   | old job of player returns [job table](https://vestedmarius.github.io/md_docs/md_2.5/server/xplayer/data/job)                                                                                 |



#### Example Server-Side Usage

```lua
RegisterServerEvent('esx:setjob')
AddEventHandler('esx:setjob', function(source, job, lastjob)
	xPlayer = ESX.GetPlayerFromId(source)

	print(xPlayer.getName() .. ' old job name: ' .. lastjob.name .. ' new job name: ' .. job.name)
end)
```