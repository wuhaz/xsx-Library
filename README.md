# xsx Lib

xsx is a open sourced Roblox UI library

## Booting Library
```lua
local library = loadstring(game:HttpGet("https://raw.githubusercontent.com/wuhaz/xsx-Library/main/Arsenal%20s"))()
```

## Features:
- Buttons
- Sliders
- Textbox
- Toggles
- Labels
- Notifications
- Ranks
- Dropdowns
- Keybinds
- TexBoxes


## Documentation
Documentation Made By Wuhazu

# Creating a Rank
```lua
library.rank = "nigga"
local Wm = library:Watermark("xsx example | v" .. library.version ..  " | " .. library:GetUsername() .. " | rank: " .. library.rank)
local FpsWm = Wm:AddWatermark("fps: " .. library.fps)
coroutine.wrap(function()
    while wait(.75) do
        FpsWm:Text("fps: " .. library.fps)
    end
end)()
```

# Creating A Window
```lua
library.title = "Wuhazu"

library:Introduction()
wait(1)
local Init = library:Init()
```

# Creating a Notification
```lua
local Notif = library:InitNotifications()

for i = 20,0,-1 do 
    task.wait(0.05)
    local LoadingXSX = Notif:Notify("Loading xsx lib v2, please be patient.", 3, "information") -- notification, alert, error, success, information
end 

```

# Creating a Tab
```lua
local Tab1 = Init:NewTab("Example tab")
```

# Creating a Section
```lua
local Section1 = Tab1:NewSection("Example Components")
```

# Creating a Label
```lua
local Label1 = Tab1:NewLabel("Example label", "left")--"left", "center", "right"
```

# Creating a Toggle (With Keybind)
```lua
local Toggle1 = Tab1:NewToggle("Example toggle", false, function(value)
    local vers = value and "on" or "off"
    print("one " .. vers)
end):AddKeybind(Enum.KeyCode.RightControl)
```

# Creating a Button
```lua
local Button1 = Tab1:NewButton("Button", function()
    print("one")
end)
```

# Creating a Keybind
```lua
local Keybind1 = Tab1:NewKeybind("Keybind 1", Enum.KeyCode.RightAlt, function(key)
    Init:UpdateKeybind(Enum.KeyCode[key])
end)
```

# Creating a Textbox
```lua 
local Textbox1 = Tab1:NewTextbox("Text box 1 [auto scales // small]", "", "1", "all", "small", true, false, function(val)
    print(val)
end)
```

# Creating a Small Textbox
```lua
local Textbox1 = Tab1:NewTextbox("Text box 1 [auto scales // small]", "", "1", "all", "small", true, false, function(val)
    print(val)
end)
```

# Creating a Medium Textbox
```lua
 local Textbox2 = Tab1:NewTextbox("Text box 2 [medium]", "", "2", "all", "medium", true, false, function(val)
    print(val)
end)
```

# Creating a Large Textbox
```lua
local Textbox3 = Tab1:NewTextbox("Text box 3 [large]", "", "3", "all", "large", true, false, function(val)
    print(val)
end)
```

# Creating a Selector/Dropdown
```lua
 local Selector1 = Tab1:NewSelector("Selector 1", "bungie", {"fg", "fge", "fg", "fg"}, function(d)
    print(d)
end):AddOption("fge")
```

# Creating a Slider
```lua
local Slider1 = Tab1:NewSlider("Slider 1", "", true, "/", {min = 1, max = 100, default = 20}, function(value)
    print(value)
end)
```

# Paste This In The Bottom Of Your Script
```lua
local FinishedLoading = Notif:Notify("Loaded midnight.cc", 4, "success")
```
You Have To Include This Or your dick will blow off
