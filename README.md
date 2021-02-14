
Hello, welcome to my website! Feel free to take a random kick script! (Credits to a random developer forum user.)

```lua
local bannedPlayers = {
	912587768
}

function playerEntered(player)
	if (table.find(bannedPlayers, player.UserId)) then
		player:Kick("You have been banned.")
	end
end

game.Players.PlayerAdded:Connect(playerEntered)
```


