
-- Instances:

local ScreenGui = Instance.new("ScreenGui")
local OthersFrame = Instance.new("Frame")
local UIGradient = Instance.new("UIGradient")
local UICorner = Instance.new("UICorner")
local MainFrame2Title = Instance.new("TextLabel")
local Frame = Instance.new("Frame")
local Script1 = Instance.new("TextButton")
local Script2 = Instance.new("TextButton")
local Script3 = Instance.new("TextButton")
local CloseOthers = Instance.new("TextButton")
local UICorner_2 = Instance.new("UICorner")
local Shadow = Instance.new("Frame")
local UICorner_3 = Instance.new("UICorner")
local TextLabel = Instance.new("TextLabel")

--Properties:

ScreenGui.Parent = game.CoreGui

OthersFrame.Name = "OthersFrame"
OthersFrame.Parent = ScreenGui
OthersFrame.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
OthersFrame.BorderColor3 = Color3.fromRGB(27, 42, 53)
OthersFrame.BorderSizePixel = 0
OthersFrame.Position = UDim2.new(0.333002001, 0, 0.282537073, 0)
OthersFrame.Size = UDim2.new(0, 335, 0, 263)
OthersFrame.Active = true
OthersFrame.Draggable = true

UIGradient.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(45, 168, 182)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(64, 96, 161))}
UIGradient.Parent = OthersFrame

UICorner.CornerRadius = UDim.new(0, 4)
UICorner.Parent = OthersFrame

MainFrame2Title.Name = "MainFrame2Title"
MainFrame2Title.Parent = OthersFrame
MainFrame2Title.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
MainFrame2Title.Position = UDim2.new(0.226865664, 0, 0.0304182507, 0)
MainFrame2Title.Size = UDim2.new(0, 184, 0, 44)
MainFrame2Title.Font = Enum.Font.SourceSansBold
MainFrame2Title.Text = "Others"
MainFrame2Title.TextColor3 = Color3.fromRGB(255, 255, 255)
MainFrame2Title.TextSize = 31.000

Frame.Parent = OthersFrame
Frame.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
Frame.Position = UDim2.new(0.0746268705, 0, 0.24714829, 0)
Frame.Size = UDim2.new(0, 286, 0, 184)
Frame.Active = true
Frame.Draggable = false

Script1.Name = "Script1"
Script1.Parent = Frame
Script1.BackgroundColor3 = Color3.fromRGB(0, 170, 255)
Script1.Position = UDim2.new(0.230769232, 0, 0.048913043, 0)
Script1.Size = UDim2.new(0, 153, 0, 50)
Script1.Font = Enum.Font.SciFi
Script1.Text = "FAST TP"
Script1.TextColor3 = Color3.fromRGB(0, 0, 0)
Script1.TextSize = 27.000
Script1.MouseButton1Down:connect(function()
	loadstring(game:HttpGet(('https://raw.githubusercontent.com/MainHackScripts/FASTRBTP/main/README.md'),true))()
end)

Script2.Name = "Script2"
Script2.Parent = Frame
Script2.BackgroundColor3 = Color3.fromRGB(0, 170, 255)
Script2.Position = UDim2.new(0.230769232, 0, 0.364130437, 0)
Script2.Size = UDim2.new(0, 153, 0, 50)
Script2.Font = Enum.Font.SourceSans
Script2.Text = "MASCOTS"
Script2.TextColor3 = Color3.fromRGB(0, 0, 0)
Script2.TextSize = 27.000
Script2.MouseButton1Down:connect(function()
	game:GetService("StarterGui"):SetCore("SendNotification", {Title = "Mascot RBW2", Text = "Comming Soon!"})
end)

Script3.Name = "Script3"
Script3.Parent = Frame
Script3.BackgroundColor3 = Color3.fromRGB(0, 170, 255)
Script3.Position = UDim2.new(0.230769232, 0, 0.684782624, 0)
Script3.Size = UDim2.new(0, 153, 0, 50)
Script3.Font = Enum.Font.SourceSans
Script3.Text = "CREDITS:"
Script3.TextColor3 = Color3.fromRGB(0, 0, 0)
Script3.TextSize = 27.000
Script3.MouseButton1Down:connect(function()
	game:GetService("StarterGui"):SetCore("SendNotification", {Title = "GUI BY:", Text = "NitroHub#5026"})
	game:GetService("StarterGui"):SetCore("SendNotification", {Title = "Gui DSFX", Text = "NitroHub#5026"})
	game:GetService("StarterGui"):SetCore("SendNotification", {Title = "CODING BY:", Text = "NitroHub#5026"})
	game:GetService("StarterGui"):SetCore("SendNotification", {Title = "Thank you", Text = "Thanks for using NitroHUB!"})
end)

CloseOthers.Name = "CloseOthers"
CloseOthers.Parent = OthersFrame
CloseOthers.BackgroundColor3 = Color3.fromRGB(77, 100, 150)
CloseOthers.BorderSizePixel = 0
CloseOthers.Position = UDim2.new(0.813328981, 0, 0.0295569599, 0)
CloseOthers.Size = UDim2.new(0, 55, 0, 44)
CloseOthers.ZIndex = 2
CloseOthers.Font = Enum.Font.GothamSemibold
CloseOthers.Text = ""
CloseOthers.TextColor3 = Color3.fromRGB(255, 255, 255)
CloseOthers.TextScaled = true
CloseOthers.TextSize = 14.000
CloseOthers.TextWrapped = true
CloseOthers.MouseButton1Down:connect(function()
	OthersFrame.Visible = false
end)

UICorner_2.Parent = CloseOthers

Shadow.Name = "Shadow"
Shadow.Parent = CloseOthers
Shadow.BackgroundColor3 = Color3.fromRGB(53, 69, 103)
Shadow.BorderSizePixel = 0
Shadow.Size = UDim2.new(1, 0, 1, 4)

UICorner_3.Parent = Shadow

TextLabel.Parent = CloseOthers
TextLabel.AnchorPoint = Vector2.new(0.5, 0.5)
TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextLabel.BackgroundTransparency = 1.000
TextLabel.BorderColor3 = Color3.fromRGB(27, 42, 53)
TextLabel.BorderSizePixel = 0
TextLabel.Position = UDim2.new(0.5, 0, 0.5, 0)
TextLabel.Size = UDim2.new(1, -20, 1, -20)
TextLabel.ZIndex = 2
TextLabel.Font = Enum.Font.GothamSemibold
TextLabel.Text = "X"
TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
TextLabel.TextScaled = true
TextLabel.TextSize = 14.000
TextLabel.TextWrapped = true
