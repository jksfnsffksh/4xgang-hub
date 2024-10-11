\\x-- Script 4x Hub para Blox Fruits
local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()

-- Função para auto farming
local function autoFarm()
    while true do
        -- Código para auto farming
        wait(1) -- Ajuste o tempo conforme necessário
    end
end

-- Função para auto boss fights
local function autoBoss()
    while true do
        -- Código para auto boss fights
        wait(1) -- Ajuste o tempo conforme necessário
    end
end

-- Função para teletransporte
local function teletransportar(x, y, z)
    character.HumanoidRootPart.CFrame = CFrame.new(x, y, z)
end

-- Função para ESP
local function ativarESP()
    -- Código para ESP
end

-- Atalhos para ativar as funções
local UserInputService = game:GetService("UserInputService")

UserInputService.InputBegan:Connect(function(input)
    if input.KeyCode == Enum.KeyCode.F then
        autoFarm()
    elseif input.KeyCode == Enum.KeyCode.B then
        autoBoss()
    elseif input.KeyCode == Enum.KeyCode.T then
        teletransportar(100, 50, 100) -- Coordenadas de exemplo
    elseif input.KeyCode == Enum.KeyCode.E then
        ativarESP()
    end
end)

print("Script 4x Hub carregado com sucesso!")
