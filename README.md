-- Criação de uma GUI flutuante no Roblox (segura)
local ScreenGui = Instance.new("ScreenGui")
local Frame = Instance.new("Frame")
local Title = Instance.new("TextLabel")
local AutoWinBtn = Instance.new("TextButton")
local AutoBondBtn = Instance.new("TextButton")

-- GUI principal
ScreenGui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
ScreenGui.Name = "NatHub"

Frame.Parent = ScreenGui
Frame.Size = UDim2.new(0, 300, 0, 220)
Frame.Position = UDim2.new(0.5, -150, 0.5, -110)
Frame.BackgroundColor3 = Color3.fromRGB(30, 30, 30)
Frame.Active = true
Frame.Draggable = true

Title.Parent = Frame
Title.Size = UDim2.new(1, 0, 0, 40)
Title.BackgroundColor3 = Color3.fromRGB(50, 50, 50)
Title.Text = "NatHub | Dead Rails"
Title.TextColor3 = Color3.new(1, 1, 1)
Title.Font = Enum.Font.SourceSansBold
Title.TextSize = 20

-- Botão Auto Win
AutoWinBtn.Parent = Frame
AutoWinBtn.Position = UDim2.new(0, 20, 0, 60)
AutoWinBtn.Size = UDim2.new(0, 260, 0, 40)
AutoWinBtn.Text = "Auto Win"
AutoWinBtn.BackgroundColor3 = Color3.fromRGB(70, 70, 70)
AutoWinBtn.TextColor3 = Color3.new(1, 1, 1)
AutoWinBtn.MouseButton1Click:Connect(function()
    print("Executando ação: Auto Win")
    -- Aqui você adicionaria código válido permitido pelo jogo, ex: dar recompensa se for permitido
end)

-- Botão Auto Bond
AutoBondBtn.Parent = Frame
AutoBondBtn.Position = UDim2.new(0, 20, 0, 110)
AutoBondBtn.Size = UDim2.new(0, 260, 0, 40)
AutoBondBtn.Text = "Auto Bond"
AutoBondBtn.BackgroundColor3 = Color3.fromRGB(70, 70, 70)
AutoBondBtn.TextColor3 = Color3.new(1, 1, 1)
AutoBondBtn.MouseButton1Click:Connect(function()
    print("Executando ação: Auto Bond")
    -- Aqui poderia ativar ações como coleta automatizada dentro das regras
end)
