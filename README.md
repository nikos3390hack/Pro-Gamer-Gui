# Pro-Gamer-Gui

This is a script loader i made because i was bored

To make this script i used Orion library
https://github.com/shlexware/Orion

local games = {
    [{6839171747}] = "https://raw.githubusercontent.com/nikos3390hack/Pro-Gamer-Gui/main/scripts/Doors.lua",
}

for ids, url in next, games do
    if table.find(ids, game.PlaceId) then
        loadstring(game:HttpGet(url))()
        break
    end
end
