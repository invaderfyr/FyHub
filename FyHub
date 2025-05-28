local Rayfield = loadstring(game:HttpGet('https://sirius.menu/rayfield'))()

local Window = Rayfield:CreateWindow({
   Name = "FY SCRIPTS",
   Icon = 0, -- Icon in Topbar. Can use Lucide Icons (string) or Roblox Image (number). 0 to use no icon (default).
   LoadingTitle = "FY SCRIPTS",
   LoadingSubtitle = "by Imvader_fyr",
   Theme = "Default", -- Check https://[Log in to view URL]

   ToggleUIKeybind = "K", -- The keybind to toggle the UI visibility (string like "K" or Enum.KeyCode)

   DisableRayfieldPrompts = false,
   DisableBuildWarnings = false, -- Prevents Rayfield from warning when the script has a version mismatch with the interface

   ConfigurationSaving = {
      Enabled = true,
      FolderName = nil, -- Create a custom folder for your hub/game
      FileName = "Fy Hub"
   },

   Discord = {
      Enabled = false, -- Prompt the user to join your Discord server if their executor supports it
      Invite = "noinvitelink", -- The Discord invite code, do not include discord.gg/. E.g. discord.gg/ ABCD would be ABCD
      RememberJoins = true -- Set this to false to make them join the discord every time they load it up
   },

   KeySystem = true, -- Set this to true to use our key system
   KeySettings = {
      Title = "Fy Key System",
      Subtitle = "Key System",
      Note = "Get the key in my avatar info", -- Use this to tell the user how to get a key
      FileName = "Fy_Key", -- It is recommended to use something unique as other scripts using Rayfield may overwrite your key file
      SaveKey = true, -- The user's key will be saved, but if you change the key, they will be unable to use your script
      GrabKeyFromSite = true, -- If this is true, set Key below to the RAW site you would like Rayfield to get the key from
      Key = {"Invader_noob"} -- List of kviewthat will be accepted by the system, can be RAW file links (pastebin, github etc) or simple strings ("hello","key22")
   }
})

local MainTab = Window:CreateTab("Main", nil) -- Title, Image
local Section = MainTab:CreateSection("Games")

Rayfield:Notify({
   Title = "welcome user",
   Content = "This script cannot be shared",
   Duration = 5,
   Image = nil,
})

local Button = MainTab:CreateButton({
   Name = "7 days to live",
   Callback = function()
               loadstring(game:HttpGet("https://rawscripts.net/raw/7-Days-To-Live-7-days-to-live-38787"))()
end,})

local playerTab = Window:CreateTab("Player", nil) -- Title, Image

local Slider = playerTab:CreateSlider({
   Name = "Walkspeed",
   Range = {0, 500},
   Increment = 1,
   Suffix = "walk",
   CurrentValue = 16,
   Flag = "Slider1", -- A flag is the identifier for the configuration file, make sure every element has a different flag if you're using configuration saving to ensure no overlaps
   Callback = function(Value)
            game.Players.localPlayer.character.Humanoid.WalkSpeed = (Value)
   end,
})

local Slider = playerTab:CreateSlider({
   Name = "jumppower",
   Range = {0, 500},
   Increment = 10,
   Suffix = "jump",
   CurrentValue = 10,
   Flag = "Slider2", -- A flag is the identifier for the configuration file, make sure every element has a different flag if you're using configuration saving to ensure no overlaps
   Callback = function(Value)
            game.Players.localPlayer.character.Humanoid.JumpPower = (Value)
   end,
})

local otherTab = Window:CreateTab("Other", nil) -- Title, Image

local Button = otherTab:CreateButton({
   Name = "Cool kid",
   Callback = function() 
            loadstring(game:HttpGet("https://raw.githubusercontent.com/MiRw3b/c00lgui-v3rx/main/c00lguiv3rx.lua"))()
end,})

local Button = otherTab:CreateButton({
   Name = "Nameless admin",
   Callback = function()
            loadstring(game:HttpGet("https://rawscripts.net/raw/Universal-Script-nameless-admin-so-good-38584"))()
   end,
})

local creditTab = Window:CreateTab("Credits", nil) -- Title, Image

local Input = creditTab:CreateInput({
   Name = "By Invader_fyr",
   CurrentValue = "Hi",
   PlaceholderText = "Input Placeholder",
   RemoveTextAfterFocusLost = false,
   Flag = "Input1",
   Callback = function(Text)
   end,
})
