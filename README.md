local ScreenGui = Instance.new("ScreenGui")
ScreenGui.Name = "Blox Fruits GUI"
ScreenGui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")

local MainFrame = Instance.new("Frame")
MainFrame.Name = "Main Frame"
MainFrame.Size = UDim2.new(0.5, 0, 0.5, 0)
MainFrame.Position = UDim2.new(0.25, 0, 0.25, 0)
MainFrame.BackgroundColor3 = Color3.fromRGB(40, 40, 40)
MainFrame.BorderSizePixel = 0
MainFrame.Parent = ScreenGui

local TitleLabel = Instance.new("TextLabel")
TitleLabel.Name = "Title Label"
TitleLabel.Text = "BLOX FRUITS"
TitleLabel.Size = UDim2.new(1, 0, 0.1, 0)
TitleLabel.Position = UDim2.new(0, 0, 0, 0)
TitleLabel.BackgroundColor3 = Color3.fromRGB(255, 0, 0)
TitleLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
TitleLabel.Font = Enum.Font.SourceSansBold
TitleLabel.TextSize = 24
TitleLabel.Parent = MainFrame

local TabsFrame = Instance.new("Frame")
TabsFrame.Name = "Tabs Frame"
TabsFrame.Size = UDim2.new(1, 0, 0.1, 0)
TabsFrame.Position = UDim2.new(0, 0, 0.1, 0)
TabsFrame.BackgroundColor3 = Color3.fromRGB(50, 50, 50)
TabsFrame.Parent = MainFrame

local DiscordButton = Instance.new("TextButton")
DiscordButton.Name = "Discord Button"
DiscordButton.Size = UDim2.new(0.2, 0, 1, 0)
DiscordButton.Position = UDim2.new(0, 0, 0, 0)
DiscordButton.BackgroundColor3 = Color3.fromRGB(70, 70, 70)
DiscordButton.TextColor3 = Color3.fromRGB(255, 255, 255)
DiscordButton.Font = Enum.Font.SourceSans
DiscordButton.TextSize = 16
DiscordButton.Text = "Discord"
DiscordButton.Parent = TabsFrame

local FarmButton = Instance.new("TextButton")
FarmButton.Name = "Farm Button"
FarmButton.Size = UDim2.new(0.2, 0, 1, 0)
FarmButton.Position = UDim2.new(0.2, 0, 0, 0)
FarmButton.BackgroundColor3 = Color3.fromRGB(70, 70, 70)
FarmButton.TextColor3 = Color3.fromRGB(255, 255, 255)
FarmButton.Font = Enum.Font.SourceSans
FarmButton.TextSize = 16
FarmButton.Text = "Farm"
FarmButton.Parent = TabsFrame

local SeaButton = Instance.new("TextButton")
SeaButton.Name = "Sea Button"
SeaButton.Size = UDim2.new(0.2, 0, 1, 0)
SeaButton.Position = UDim2.new(0.4, 0, 0, 0)
SeaButton.BackgroundColor3 = Color3.fromRGB(70, 70, 70)
SeaButton.TextColor3 = Color3.fromRGB(255, 255, 255)
SeaButton.Font = Enum.Font.SourceSans
SeaButton.TextSize = 16
SeaButton.Text = "Sea"
SeaButton.Parent = TabsFrame

local QuestsButton = Instance.new("TextButton")
QuestsButton.Name = "Quests Button"
QuestsButton.Size = UDim2.new(0.2, 0, 1, 0)
QuestsButton.Position = UDim2.new(0.6, 0, 0, 0)
QuestsButton.BackgroundColor3 = Color3.fromRGB(70, 70, 70)
QuestsButton.TextColor3 = Color3.fromRGB(255, 255, 255)
QuestsButton.Font = Enum.Font.SourceSans
QuestsButton.TextSize = 16
QuestsButton.Text = "Quests/Items"
QuestsButton.Parent = TabsFrame

local SportButton = Instance.new("TextButton")
SportButton.Name = "Sport Button"
SportButton.Size = UDim2.new(0.2, 0, 1, 0)
SportButton.Position = UDim2.new(0.8, 0, 0, 0)
SportButton.BackgroundColor3 = Color3.fromRGB(70, 70, 70)
SportButton.TextColor3 = Color3.fromRGB(255, 255, 255)
SportButton.Font = Enum.Font.SourceSans
SportButton.TextSize = 16
SportButton.Text = "Sport"
SportButton.Parent = TabsFrame

local ContentFrame = Instance.new("Frame")
ContentFrame.Name = "Content Frame"
ContentFrame.Size = UDim2.new(1, 0, 0.8, 0)
ContentFrame.Position = UDim2.new(0, 0, 0.2, 0)
ContentFrame.BackgroundColor3 = Color3.fromRGB(60, 60, 60)
ContentFrame.Parent = MainFrame

-- Discord Tab
local DiscordLabel = Instance.new("TextLabel")
DiscordLabel.Name = "Discord Label"
DiscordLabel.Size = UDim2.new(1, 0, 1, 0)
DiscordLabel.Position = UDim2.new(0, 0, 0, 0)
DiscordLabel.BackgroundColor3 = Color3.fromRGB(60, 60, 60)
DiscordLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
DiscordLabel.Font = Enum.Font.SourceSans
DiscordLabel.TextSize = 20
DiscordLabel.Text = "Join our Discord Server!"
DiscordLabel.Parent = ContentFrame

-- Farm Tab
local FarmLabel = Instance.new("TextLabel")
FarmLabel.Name = "Farm Label"
FarmLabel.Size = UDim2.new(1, 0, 1, 0)
FarmLabel.Position = UDim2.new(0, 0, 0, 0)
FarmLabel.BackgroundColor3 = Color3.fromRGB(60, 60, 60)
FarmLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
FarmLabel.Font = Enum.Font.SourceSans
FarmLabel.TextSize = 20
FarmLabel.Text = "Start farming now!"
FarmLabel.Visible = false
FarmLabel.Parent = ContentFrame

-- Sea Tab
local SeaLabel = Instance.new("TextLabel")
SeaLabel.Name = "Sea Label"
SeaLabel.Size = UDim2.new(1, 0, 1, 0)
SeaLabel.Position = UDim2.new(0, 0, 0, 0)
SeaLabel.BackgroundColor3 = Color3.fromRGB(60, 60, 60)
SeaLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
SeaLabel.Font = Enum.Font.SourceSans
SeaLabel.TextSize = 20
SeaLabel.Text = "Explore the vast sea!"
SeaLabel.Visible = false
SeaLabel.Parent = ContentFrame

-- Quests/Items Tab
local QuestsLabel = Instance.new("TextLabel")
QuestsLabel.Name = "Quests Label"
QuestsLabel.Size = UDim2.new(1, 0, 1, 0)
QuestsLabel.Position = UDim2.new(0, 0, 0, 0)
QuestsLabel.BackgroundColor3 = Color3.fromRGB(60, 60, 60)
QuestsLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
QuestsLabel.Font = Enum.Font.SourceSans
QuestsLabel.TextSize = 20
QuestsLabel.Text = "Complete quests and collect items!"
QuestsLabel.Visible = false
QuestsLabel.Parent = ContentFrame

-- Sport Tab
local SportLabel = Instance.new("TextLabel")
SportLabel.Name = "Sport Label"
SportLabel.Size = UDim2.new(1, 0, 1, 0)
SportLabel.Position = UDim2.new(0, 0, 0, 0)
SportLabel.BackgroundColor3 = Color3.fromRGB(60, 60, 60)
SportLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
SportLabel.Font = Enum.Font.SourceSans
SportLabel.TextSize = 20
SportLabel.Text = "Participate in sports events!"
SportLabel.Visible = false
SportLabel.Parent = ContentFrame

-- Tab Switching
DiscordButton.MouseButton1Click:Connect(function()
    DiscordLabel.Visible = true
    FarmLabel.Visible = false
    SeaLabel.Visible = false
    QuestsLabel.Visible = false
    SportLabel.Visible = false
end)

FarmButton.MouseButton1Click:Connect(function()
    DiscordLabel.Visible = false
    FarmLabel.Visible = true
    SeaLabel.Visible = false
    QuestsLabel.Visible = false
    SportLabel.Visible = false
end)

SeaButton.MouseButton1Click:Connect(function()
    DiscordLabel.Visible = false
    FarmLabel.Visible = false
    SeaLabel.Visible = true
    QuestsLabel.Visible = false
    SportLabel.Visible = false
end)

QuestsButton.MouseButton1Click:Connect(function()
    DiscordLabel.Visible = false
    FarmLabel.Visible = false
    SeaLabel.Visible = false
    QuestsLabel.Visible = true
    SportLabel.Visible = false
end)

SportButton.MouseButton1Click:Connect(function()
    DiscordLabel.Visible = false
    FarmLabel.Visible = false
    SeaLabel.Visible = false
    QuestsLabel.Visible = false
    SportLabel.Visible = true
end)
