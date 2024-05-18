local lib = loadstring(game:HttpGet("https://raw.githubusercontent.com/AZYsGithub/Arceus-X-UI-Library/main/source.lua"))()
lib:SetTitle("Arcues  x script (Basic)")
lib:SetIcon("http://www.roblox.com/asset/?id=9178187770")
local a = workspace.Gravity

lib:SetTheme("Default")
lib:AddButton("Reset", function()
    game.Players.LocalPlayer.Character.Head:Destroy()
end)

lib:AddToggle("fakelv", function(state)
    if state then
        loadstring(game:HttpGet('https://raw.githubusercontent.com/SHAREHACK/allscript/main/level'))()
    else
        workspace.Gravity = a
    end
end, false)
