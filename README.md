local lib = loadstring(game:HttpGet("https://raw.githubusercontent.com/rainhitgrassed/Slixx-ui-library/refs/heads/main/source"))();

lib:SetTitle("Shadow.cc") -- name <string>

local tab1 = lib:NewTab("Main") -- name <string> description <string>
tab1:NewToggle("Auto Win",false,function(bool) -- name <string> default <bool> callback <function>

end)
tab1:NewDropdown("Dropdown",{"1","2","3","4","5"},"hi",function(selected) -- name <string> list <table> default <string> callback <function>
	print(selected)
end)
tab1:NewTextBox("WalkSpeed","Enter WalkSpeed",function(value) -- name <string> placeholdertext <string> callback <function>
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = value
end)
tab1:NewSlider("WalkSpeed",16,500,16,function(value) -- name <string> minimum <number> maximium <number> default <number> callback <function>
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = value
end)
tab1:NewButton("Change Jump Height to 110",function()-- name <string> callback <function>
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = 110
end)
