-- W1MN - Rock Fruit Auto Script
-- Created by Deegiigdy

if game.PlaceId ~= 15502339000 then
    warn("This script is -- W1MN - Rock Fruit Auto Script
-- Created by Deegiigdy

if game.PlaceId ~= 15502339000 then
    warn("This script is intended for Rock Fruit only.")
    return
end

-- Anti-AFK
local vu = game:GetService("VirtualUser")
game:GetService("Players").LocalPlayer.Idled:Connect(function()
    vu:Button2Down(Vector2.new(0,0), workspace.CurrentCamera.CFrame)
    task.wait(1)
    vu:Button2Up(Vector2.new(0,0), workspace.CurrentCamera.CFrame)
end)

-- Basic UI Loader (placeholder)
local ScreenGui = Instance.new("ScreenGui", game.CoreGui)
ScreenGui.Name = "W1MN_UI"
local TextLabel = Instance.new("TextLabel", ScreenGui)
TextLabel.Size = UDim2.new(0, 250, 0, 50)
TextLabel.Position = UDim2.new(0.5, -125, 0, 50)
TextLabel.Text = "W1MN Script Loaded!"
TextLabel.TextScaled = true
TextLabel.BackgroundColor3 = Color3.new(0.2, 0.2, 0.2)
TextLabel.TextColor3 = Color3.new(1, 1, 1)
TextLabel.BorderSizePixel = 0

-- Future features will be added here:
-- Auto Farm
-- Skill Selector
-- Weapon Selector
-- Cross-Sea NPC System
-- Auto Stats

print("W1MN script loaded successfully.")
