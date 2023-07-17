local Rayfield = loadstring(game:HttpGet('https://sirius.menu/rayfield'))()

local Window = Rayfield:CreateWindow({
   Name = "                         🚗 Car Driving Indonesia 🚗",
   LoadingTitle = "Nah Hub",
   LoadingSubtitle = "by IPelZ",
   ConfigurationSaving = {
      Enabled = false,
      FolderName = nil, -- Create a custom folder for your hub/game
      FileName = "Nah Hub"
   },
   Discord = {
      Enabled = true    ,
      Invite = "zZNr9TSHFr", -- The Discord invite code, do not include discord.gg/. E.g. discord.gg/ABCD would be ABCD
      RememberJoins = true -- Set this to false to make them join the discord every time they load it up
   },
   KeySystem = true, -- Set this to true to use our key system
   KeySettings = {
      Title = "Car Driving Indonesia | Key",
      Subtitle = "Key at Discord Server",
      Note = "https://discord.gg/RH6PXH5Qpk",
      FileName = "nahhubkey", -- It is recommended to use something unique as other scripts using Rayfield may overwrite your key file
      SaveKey = false, -- The user's key will be saved, but if you change the key, they will be unable to use your script
      GrabKeyFromSite = true, -- If this is true, set Key below to the RAW site you would like Rayfield to get the key from
      Key = {"https://pastebin.com/raw/szWbpBYU"} -- List of keys that will be accepted by the system, can be RAW file links (pastebin, github etc) or simple strings ("hello","key22")
   }
})

local MainTab = Window:CreateTab("🏠 Home", nil) -- Title, Image
local MainSection = MainTab:CreateSection("Main")

Rayfield:Notify({
   Title = "You executed the script!",
   Content = "Good Luck and Have Fun,",
   Duration = 5,
   Image = nil,
   Actions = { -- Notification Buttons
      Ignore = {
         Name = "Okay!",
         Callback = function()
         print("The user tapped Okay!")
      end
   },
},
})

Rayfield:Notify({
   Title = "OWN RISK",
   Content = "Best Script by IPelZ,",
   Duration = 10,
   Image = nil,
   Actions = { -- Notification Buttons
      Ignore = {
         Name = "Okay!",
         Callback = function()
         print("The user tapped Okay!")
      end
   },
},
})

local Toggle = MainTab:CreateToggle({
   Name = "Auto Farm",
   CurrentValue = false,
   Flag = "Toggle", -- A flag is the identifier for the configuration file, make sure every element has a different flag if you're using configuration saving to ensure no overlaps
   Callback = function(Value)
        print('hello')
   end,
})

local Dropdown = MainTab:CreateDropdown({
   Name = "Select Farm",
   Options = {"Cafe | Slow","Truck Farm"},
   CurrentOption = {"Job"},
   MultipleOptions = false,
   Flag = "teleport", -- A flag is the identifier for the configuration file, make sure every element has a different flag if you're using configuration saving to ensure no overlaps
   Callback = function(Option)
        print(Option)
   end,
})

local Button = MainTab:CreateButton({
   Name = "ANTI AFK",
   Callback = function()
        wait(0.5)local ba=Instance.new("ScreenGui")
local ca=Instance.new("TextLabel")local da=Instance.new("Frame")
local _b=Instance.new("TextLabel")local ab=Instance.new("TextLabel")ba.Parent=game.CoreGui
ba.ZIndexBehavior=Enum.ZIndexBehavior.Sibling;ca.Parent=ba;ca.Active=true
ca.BackgroundColor3=Color3.new(0.176471,0.176471,0.176471)ca.Draggable=true
ca.Position=UDim2.new(0.698610067,0,0.098096624,0)ca.Size=UDim2.new(0,304,0,52)
ca.Font=Enum.Font.SourceSansSemibold;ca.Text="Anti Afk Kick Script"ca.TextColor3=Color3.new(0,1,1)
ca.TextSize=22;da.Parent=ca
da.BackgroundColor3=Color3.new(0.196078,0.196078,0.196078)da.Position=UDim2.new(0,0,1.0192306,0)
da.Size=UDim2.new(0,304,0,107)_b.Parent=da
_b.BackgroundColor3=Color3.new(0.176471,0.176471,0.176471)_b.Position=UDim2.new(0,0,0.800455689,0)
_b.Size=UDim2.new(0,304,0,21)_b.Font=Enum.Font.Arial;_b.Text="Made by Nah💤"
_b.TextColor3=Color3.new(1,1,1)_b.TextSize=20;ab.Parent=da
ab.BackgroundColor3=Color3.new(0.176471,0.176471,0.176471)ab.Position=UDim2.new(0,0,0.158377379,0)
ab.Size=UDim2.new(0,304,0,44)ab.Font=Enum.Font.ArialBold;ab.Text="Status: Script Started"
ab.TextColor3=Color3.new(1,1,1)ab.TextSize=20;local bb=game:service'VirtualUser'
game:service'Players'.LocalPlayer.Idled:connect(function()
bb:CaptureController()bb:ClickButton2(Vector2.new())
ab.Text="You went idle and ROBLOX tried to kick you but we reflected it!"wait(2)ab.Text="Script Re-Enabled"end)
   end,
})

local TeleportTab = Window:CreateTab("✈ Teleports", nil) -- Title, Image
local Section = TeleportTab:CreateSection("Jawa Tengah")

local Button = TeleportTab:CreateButton({
   Name = "Spawn",
   Callback = function()
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(30.3196926, 936.80481, 61686.5898, 0.0996260867, 4.79245443e-08, -0.99502492, 1.15507959e-08, 1, 4.93206791e-08, 0.99502492, -1.64069558e-08, 0.0996260867)
   end,
})

local Button = TeleportTab:CreateButton({
   Name = "Cirebon",
   Callback = function()
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-21691.9102, 1040.56006, -26898.959, -0.119459286, 3.81142051e-08, 0.992839098, -2.42230804e-08, 1, -4.13036467e-08, -0.992839098, -2.89837256e-08, -0.119459286)
   end,
})

local Button = TeleportTab:CreateButton({
   Name = "Palimanan",
   Callback = function()
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-12969.5439, 1053.45911, -16391.582, -0.88787663, 3.17715703e-08, -0.460081607, 4.74615591e-09, 1, 5.98971326e-08, 0.460081607, 5.09976488e-08, -0.88787663)
   end,
})

local Button = TeleportTab:CreateButton({
   Name = "Pekalongan",
   Callback = function()
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-38678.2812, 1014.59015, -62482.1484, 0.959999979, -2.55267594e-08, 0.280000001, 2.16932374e-08, 1, 1.67901888e-08, -0.280000001, -1.00444746e-08, 0.959999979)
   end,
})

local Button = TeleportTab:CreateButton({
   Name = "Semarang",
   Callback = function()
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-50943.3203, 1012.66724, -86413.625, -0.864348352, 1.59815905e-09, -0.502893567, -1.41378531e-09, 1, 5.60787061e-09, 0.502893567, 5.55813706e-09, -0.864348352)
   end,
})

local Button = TeleportTab:CreateButton({
   Name = "Tegal",
   Callback = function()
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-31533.4355, 1046.60974, -46711.5703, -0.842999756, 3.44499256e-08, -0.537913918, 1.38103484e-08, 1, 4.24004725e-08, 0.537913918, 2.83148101e-08, -0.842999756)
   end,
})

local MiscTab = Window:CreateTab("🎲Misc", nil) -- Title, Image
local Section = MiscTab:CreateSection("Misc")

local Toggle = MiscTab:CreateToggle({
   Name = "No Clip",
   CurrentValue = false,
   Flag = "Toggle1", -- A flag is the identifier for the configuration file, make sure every element has a different flag if you're using configuration saving to ensure no overlaps
   Callback = function(Value)
        print(Noclip)
   end,
})

local Input = MiscTab:CreateInput({
   Name = "Jump Power",
   PlaceholderText = "1-200",
   RemoveTextAfterFocusLost = true,
   Callback = function(Text)
        game.Players.LocalPlayer.Character.Humanoid.JumpPower = (Text)
   end,
})

local Button = MiscTab:CreateButton({
   Name = "Infinite Jump",
   Callback = function()
        --Toggles the infinite jump between on or off on every script run
_G.infinjump = not _G.infinjump

if _G.infinJumpStarted == nil then
	--Ensures this only runs once to save resources
	_G.infinJumpStarted = true
	
	--Notifies readiness
	game.StarterGui:SetCore("SendNotification", {Title="Youtube Hub"; Text="Infinite Jump Activated!"; Duration=5;})

	--The actual infinite jump
	local plr = game:GetService('Players').LocalPlayer
	local m = plr:GetMouse()
	m.KeyDown:connect(function(k)
		if _G.infinjump then
			if k:byte() == 32 then
			humanoid = game:GetService'Players'.LocalPlayer.Character:FindFirstChildOfClass('Humanoid')
			humanoid:ChangeState('Jumping')
			wait()
			humanoid:ChangeState('Seated')
			end
		end
	end)
end
   end,
})

local Slider = MiscTab:CreateSlider({
   Name = "Walkspeed Slider",
   Range = {0, 300},
   Increment = 10,
   Suffix = "Speed",
   CurrentValue = 16,
   Flag = "Slider1", -- A flag is the identifier for the configuration file, make sure every element has a different flag if you're using configuration saving to ensure no overlaps
   Callback = function(Value)
        game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = (Value)
   end,
})

local Slider = MiscTab:CreateSlider({
   Name = "Fly Speed",
   Range = {0, 100},
   Increment = 10,
   Suffix = "Speed",
   CurrentValue = 0,
   Flag = "Slider2", -- A flag is the identifier for the configuration file, make sure every element has a different flag if you're using configuration saving to ensure no overlaps
   Callback = function(Value)
        game.Players.LocalPlayer.Character.Humanoid.Fly = (Value)
   end,
})
