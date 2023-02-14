--[[
 
	Made By ImHackingForFun2 On Roblox.
 
--]]
local SynapseX = Instance.new("ScreenGui")
local SynapseXFrame = Instance.new("Frame")
local Clear = Instance.new("TextButton")
local Code = Instance.new("TextBox")
local Execute = Instance.new("TextButton")
local Inject = Instance.new("TextButton")
local Synapse_Text = Instance.new("TextLabel")
local X_Text = Instance.new("TextLabel")
local Logs = Instance.new("TextLabel")
 
-- Things
 
SynapseX.Name = "SynapseX"
SynapseX.Parent = game.CoreGui
 
SynapseXFrame.Name = "SynapseXFrame"
SynapseXFrame.Parent = SynapseX
SynapseXFrame.Active = true
SynapseXFrame.BackgroundColor3 = Color3.new(0.192157, 0.192157, 0.192157)
SynapseXFrame.BorderSizePixel = 0
SynapseXFrame.Position = UDim2.new(0, 0, 0.67414242, 0)
SynapseXFrame.Size = UDim2.new(0, 446, 0, 247)
SynapseXFrame.Draggable = true
 
Clear.Name = "Clear"
Clear.Parent = SynapseXFrame
Clear.BackgroundColor3 = Color3.new(0.192157, 0.192157, 0.192157)
Clear.BorderSizePixel = 0
Clear.Position = UDim2.new(0.356502235, 0, 0.872381032, 0)
Clear.Size = UDim2.new(0, 127, 0, 31)
Clear.Font = Enum.Font.ArialBold
Clear.Text = "Clear"
Clear.TextColor3 = Color3.new(1, 1, 1)
Clear.TextSize = 17
 
Code.Name = "Code"
Code.Parent = SynapseXFrame
Code.BackgroundColor3 = Color3.new(0.266667, 0.266667, 0.266667)
Code.BorderSizePixel = 0
Code.Position = UDim2.new(0, 0, 0.122686706, 0)
Code.Size = UDim2.new(0, 446, 0, 185)
Code.Font = Enum.Font.SourceSans
Code.Text = ""
Code.TextColor3 = Color3.new(0, 0, 0)
Code.TextSize = 14
Code.TextXAlignment = Enum.TextXAlignment.Left
Code.TextYAlignment = Enum.TextYAlignment.Top
 
Execute.Name = "Execute"
Execute.Parent = SynapseXFrame
Execute.BackgroundColor3 = Color3.new(0.192157, 0.192157, 0.192157)
Execute.BorderSizePixel = 0
Execute.Position = UDim2.new(0, 0, 0.872381032, 0)
Execute.Size = UDim2.new(0, 127, 0, 31)
Execute.Font = Enum.Font.ArialBold
Execute.Text = "Execute"
Execute.TextColor3 = Color3.new(1, 1, 1)
Execute.TextSize = 17
 
Inject.Name = "Inject"
Inject.Parent = SynapseXFrame
Inject.BackgroundColor3 = Color3.new(0.192157, 0.192157, 0.192157)
Inject.BorderSizePixel = 0
Inject.Position = UDim2.new(0.715246618, 0, 0.872381032, 0)
Inject.Size = UDim2.new(0, 127, 0, 31)
Inject.Font = Enum.Font.ArialBold
Inject.Text = "Inject"
Inject.TextColor3 = Color3.new(1, 1, 1)
Inject.TextSize = 18
Inject.TextWrapped = true
 
Synapse_Text.Name = "Synapse_Text"
Synapse_Text.Parent = SynapseXFrame
Synapse_Text.BackgroundColor3 = Color3.new(0.192157, 0.192157, 0.192157)
Synapse_Text.BorderSizePixel = 0
Synapse_Text.Size = UDim2.new(0, 105, 0, 30)
Synapse_Text.Font = Enum.Font.Code
Synapse_Text.Text = "Synapse"
Synapse_Text.TextColor3 = Color3.new(1, 1, 1)
Synapse_Text.TextSize = 23
Synapse_Text.TextWrapped = true
Synapse_Text.TextYAlignment = Enum.TextYAlignment.Top
 
X_Text.Name = "X_Text"
X_Text.Parent = SynapseXFrame
X_Text.BackgroundColor3 = Color3.new(0.192157, 0.192157, 0.192157)
X_Text.BorderSizePixel = 0
X_Text.Position = UDim2.new(0.2130045, 0, 0, 0)
X_Text.Size = UDim2.new(0, 22, 0, 19)
X_Text.Font = Enum.Font.Code
X_Text.Text = "X"
X_Text.TextColor3 = Color3.new(1, 0.666667, 0)
X_Text.TextSize = 19
X_Text.TextWrapped = true
X_Text.TextYAlignment = Enum.TextYAlignment.Top
 
Logs.Name = "Logs"
Logs.Parent = SynapseXFrame
Logs.BackgroundColor3 = Color3.new(0.192157, 0.192157, 0.192157)
Logs.BorderSizePixel = 0
Logs.Position = UDim2.new(0.284753352, 0, 0.0121457493, 0)
Logs.Size = UDim2.new(0, 149, 0, 23)
Logs.Font = Enum.Font.Code
Logs.Text = ""
Logs.TextColor3 = Color3.new(1, 1, 1)
Logs.TextSize = 20
Logs.TextYAlignment = Enum.TextYAlignment.Top
 
-- Making It Work
 
Clear.MouseButton1Down:connect(function()
Code.Text = ("Cleared!")
wait(2)
Code.Text = ("")
end)
 
Execute.MouseButton1Down:connect(function()
loadstring(Code.Text)
end)
 
Inject.MouseButton1Down:connect(function()
Logs.Text = ("Injecting...")
wait(7)
Logs.Text = ("Injected!")
wait(4)
Logs.Text = ("Ready To Use!")
wait(3)
Logs.Text = ("")
end)
