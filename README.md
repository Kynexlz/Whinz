# Whinz Hub

```lua
local Hub = loadstring(game:HttpGet("https://raw.githubusercontent.com/Kynexlz/Whinz/refs/heads/main/Whinz"))()

local Window = Hub:CreateWindow({
    Title = "My Hub"
})
```

Create a Tab
```lua
local MainTab = Window:CreateTab({
    Name = "Main"
})
```

Create a Section
```lua
local Section = MainTab:CreateSection({
    Name = "Example"
})
```

Create a Label - Display text/information.
```lua
Tab:CreateLabel({
    Text = "Label"
})
```

Create a Button - Runs an action when clicked.
```lua
Tab:CreateButton({
    Name = "Button",
    Callback = function()
        print("Clicked!")
    end
})
```

Create a Toggle - On/off switch.
```lua
Tab:CreateToggle({
    Name = "Toggle",
    CurrentValue = false,
    Callback = function(Value)
        print(Value)
    end
})
```

Create a Slider - Select a number within a range.
```lua
Tab:CreateSlider({
    Name = "Speed",
    Range = {1, 100},
    Increment = 1,
    CurrentValue = 16,
    Callback = function(Value)
        print(Value)
    end
})
```

