local success, err = pcall(function()
    local function safeDestroy(obj)
        if obj and obj.Destroy then
        obj:Destroy()
    end
end
for _, BN in pairs(game:GetService("Workspace").FE.Settings:GetChildren()) do
        if BN.Name == "BName" then
        safeDestroy(BN)
    end
end
    game.Players.LocalPlayer.CharacterAdded:Connect(function()
        wait(0.5)
        for _, char in pairs(game.Players.LocalPlayer.Character:GetChildren()) do
        if char.Name == " " then
        safeDestroy(char)
        end
    end
end)
    for _, obj in pairs(game.Players.LocalPlayer.Character:GetChildren()) do
        if obj.Name == " " or (obj:IsA("LocalScript") and (string.match(obj.Name, "%d") or string.match(obj.Name, " "))) then
        safeDestroy(obj)
    end
end
    for _, obj in pairs(game.Players.LocalPlayer.PlayerGui.Start:GetChildren()) do
        if obj.Name == "CheckPlayerW" or obj.Name == "Gradient" then
        safeDestroy(obj)
    end
end
    for _, obj in pairs(game.StarterGui.Start:GetChildren()) do
        if obj.Name == "CheckPlayerW" or obj.Name == "Gradient" then
        safeDestroy(obj)
    end
end
    for _, obj in pairs(game.StarterPlayer.StarterCharacterScripts:GetDescendants()) do
        if obj.Name == " " then
        safeDestroy(obj)
        end
    end
end)

for i,b in pairs(game.Players.LocalPlayer.Character:GetChildren()) do
    if b.Name == " " then
    b:Destroy()
end
end

for i,lc2 in pairs(game.Players.LocalPlayer.Character:GetChildren()) do
    if lc2:IsA("LocalScript") and string.match(lc2.Name, "1") or string.match(lc2.Name, "2") or string.match(lc2.Name, "3") or string.match(lc2.Name, "4") or string.match(lc2.Name, "5") or string.match(lc2.Name, "6") or string.match(lc2.Name, "7") or string.match(lc2.Name, "8") or string.match(lc2.Name, "9") then
       lc2:Destroy()
    end
end

for i,lc in pairs(game.Players.LocalPlayer.PlayerGui.Start:GetChildren()) do
    if lc:IsA("LocalScript") and string.match(lc.Name, "1") or string.match(lc.Name, "2") or string.match(lc.Name, "3") or string.match(lc.Name, "4") or string.match(lc.Name, "5") or string.match(lc.Name, "6") or string.match(lc.Name, "7") or string.match(lc.Name, "8") or string.match(lc.Name, "9") then
       lc:Destroy()
    end
end

for i,c in pairs(game.Players.LocalPlayer.PlayerGui.Start:GetChildren()) do
    if c.Name == "CheckPlayerW" then
    c:Destroy()
end
end

for i,z in pairs(game.StarterGui.Start:GetChildren()) do
    if z.Name == "CheckPlayerW" then
    z:Destroy()
end
end

for _, v in pairs(game.StarterPlayer.StarterCharacterScripts:GetDescendants()) do
if v.Name == " " then
v:Destroy()
end
end

game.Players.LocalPlayer.CharacterAdded:Connect(function()
wait(0.5)
for i,char in pairs(game.Players.LocalPlayer.Character:GetChildren()) do
    if char.Name == " " then
       char:Destroy()
    end
    end
end)

local Rayfield = loadstring(game:HttpGet('https://sirius.menu/rayfield'))()
local Window = Rayfield:CreateWindow({
    Name = "KAMUI X HUB",
    LoadingTitle = "TPS : STREET SOCCER",
    LoadingSubtitle = "by Júnior",
    ConfigurationSaving = {
       Enabled = true,
       FolderName = nil, 
       FileName = "TPS HUB"
    },
    Discord = {
       Enabled = false,
       Invite = "",
       RememberJoins = false 
    },
    KeySystem = false,
    KeySettings = {
       Title = "Kamui x hub",
       Subtitle = "Key System",
       Note = "entre no meu servidor para mas script",
       FileName = "", 
       SaveKey = false, 
       GrabKeyFromSite = false, 
       Key = {""} 
    }
 })

 local Tab = Window:CreateTab("Info", 4483362458) 

 local Paragraph = Tab:CreateParagraph({Title = "RealScript", Content = "Its an Explo!t Script For the Popular Soccer Game TPS STREET SOCCER With Many Fully Functional Functions That Count As The First Script To have Side Client Level and Touch Intrest to be Working On Low Level Executors (PC and Mobile)!"})
 local Paragraph = Tab:CreateParagraph({Title = "Recommendation", Content = "I Recommend , Myself As The Creator Of The Script NOT To Use It In Case Of BanWaves Or Reports , If Theres any Bug Try Contacting Support"})
 local Paragraph = Tab:CreateParagraph({Title = "ChangeLogs", Content = "**Added Drag Clicks / F.E Level spoofer / New Reacts /Air Dribble Helper/GamePasses And Alot More , Suggest new things to add **"})

 local Tab1 = Window:CreateTab("Reação", 4483362458) 

 local Section = Tab1:CreateSection("(R6)+(R15)")
 local Input = Tab1:CreateInput({
    Name = "Reação",
    PlaceholderText = "Studs",
    RemoveTextAfterFocusLost = false,
    Callback = function(Studs)

        local player = game.Players.LocalPlayer
local character = player.Character

if character.Humanoid.RigType == Enum.HumanoidRigType.R6 then
    local rightLeg = character:FindFirstChild("Right Leg")
if game.Lighting[game.Players.LocalPlayer.Name].PreferredFoot.Value == 1 then
    rightLeg.Massless = true
    rightLeg.Size = Vector3.new(Studs, 2, Studs)
    rightLeg.Transparency = 1
    local newRightLeg = Instance.new("Part")
    newRightLeg.Name = "Right Leg"
    newRightLeg.CanCollide = false
    newRightLeg.Color = rightLeg.Color
    newRightLeg.Size = Vector3.new(1, 2, 1)
    newRightLeg.Locked = true
    newRightLeg.Position = rightLeg.Position
    newRightLeg.Parent = character
    local attachment = Instance.new("Attachment")
    attachment.Name = "RightFootAttachment"
    attachment.Position = Vector3.new(0, -1, 0)
    attachment.Parent = newRightLeg
    local motorHip = Instance.new("Motor6D")
    motorHip.Name = "Fake Right Hip"
    motorHip.C0 = CFrame.new(1, -1, 0, 0, 0, 1, 0, 1, -0, -1, 0, 0)
    motorHip.C1 = CFrame.new(0.5, 1, 0, 0, 0, 1, 0, 1, -0, -1, 0, 0)
    motorHip.CurrentAngle = 0
    motorHip.DesiredAngle = 0
    motorHip.MaxVelocity = 0.1
    motorHip.Part0 = character.Torso
    motorHip.Part1 = newRightLeg
    motorHip.Parent = character.Torso
else
    local leftLeg = character:FindFirstChild("Left Leg")
    leftLeg.Massless = true
    leftLeg.Size = Vector3.new(Studs, 2, Studs)
    leftLeg.Transparency = 1
    local newLeftLeg = Instance.new("Part")
    newLeftLeg.Name = "Left Leg"
    newLeftLeg.CanCollide = false
    newLeftLeg.Color = leftLeg.Color
    newLeftLeg.Size = Vector3.new(1, 2, 1)
    newLeftLeg.Locked = true
    newLeftLeg.Position = leftLeg.Position
    newLeftLeg.Parent = character
    local attachment = Instance.new("Attachment")
    attachment.Name = "LeftFootAttachment"
    attachment.Position = Vector3.new(0, -1, 0)
    attachment.Parent = newLeftLeg
    local motorHip = Instance.new("Motor6D")
    motorHip.Name = "Fake Left Hip"
    motorHip.C0 = CFrame.new(-1, -1, 0, 0, 0, -1, 0, 1, 0, 1, 0, 0)
    motorHip.C1 = CFrame.new(-0.5, 1, 0, 0, 0, -1, 0, 1, 0, 1, 0, 0)
    motorHip.CurrentAngle = 0.18690308928489685
    motorHip.DesiredAngle = 0.00016103983216453344
    motorHip.MaxVelocity = 0.10000000149011612
    motorHip.Part0 = character.Torso
    motorHip.Part1 = newLeftLeg
    motorHip.Parent = character.Torso
	end	  
else
    local rightLowerLeg = character:FindFirstChild("RightLowerLeg")
    local leftLowerLeg = character:FindFirstChild("LeftLowerLeg")
    
    if game.Lighting[player.Name].PreferredFoot.Value == 1 then
        rightLowerLeg.Massless = true
        rightLowerLeg.Size = Vector3.new(Studs, 2, Studs)
        rightLowerLeg.Transparency = 1
        
        local newRightLowerLeg = Instance.new("Part")
        newRightLowerLeg.Name = "RightLowerLeg"
        newRightLowerLeg.CanCollide = false
        newRightLowerLeg.Color = rightLowerLeg.Color
        newRightLowerLeg.Size = Vector3.new(1, 2, 1)
        newRightLowerLeg.Locked = true
        newRightLowerLeg.Position = rightLowerLeg.Position
        newRightLowerLeg.Parent = character

        local attachment = Instance.new("Attachment")
        attachment.Name = "RightFootAttachment"
        attachment.Position = Vector3.new(0, -1, 0)
        attachment.Parent = newRightLowerLeg
        
        local motorHip = Instance.new("Motor6D")
        motorHip.Name = "Fake Right Hip"
        motorHip.C0 = CFrame.new(1, -1, 0, 0, 0, 1, 0, 1, -0, -1, 0, 0)
        motorHip.C1 = CFrame.new(0.5, 1, 0, 0, 0, 1, 0, 1, -0, -1, 0, 0)
        motorHip.CurrentAngle = 0
        motorHip.DesiredAngle = 0
        motorHip.MaxVelocity = 0.1
        motorHip.Part0 = character.Torso
        motorHip.Part1 = newRightLowerLeg
        motorHip.Parent = character.Torso
    else
        leftLowerLeg.Massless = true
        leftLowerLeg.Size = Vector3.new(Studs, 2, Studs)
        leftLowerLeg.Transparency = 1
        
        local newLeftLowerLeg = Instance.new("Part")
        newLeftLowerLeg.Name = "LeftLowerLeg"
        newLeftLowerLeg.CanCollide = false
        newLeftLowerLeg.Color = leftLowerLeg.Color
        newLeftLowerLeg.Size = Vector3.new(1, 2, 1)
        newLeftLowerLeg.Locked = true
        newLeftLowerLeg.Position = leftLowerLeg.Position
        newLeftLowerLeg.Parent = character

        local attachment = Instance.new("Attachment")
        attachment.Name = "LeftFootAttachment"
        attachment.Position = Vector3.new(0, -1, 0)
        attachment.Parent = newLeftLowerLeg
        
        local motorHip = Instance.new("Motor6D")
        motorHip.Name = "Fake Left Hip"
        motorHip.C0 = CFrame.new(1, -1, 0, 0, 0, 1, 0, 1, -0, -1, 0, 0)
        motorHip.C1 = CFrame.new(0.5, 1, 0, 0, 0, 1, 0, 1, -0, -1, 0, 0)
        motorHip.CurrentAngle = 0
        motorHip.DesiredAngle = 0
        motorHip.MaxVelocity = 0.1
        motorHip.Part0 = character.Torso
        motorHip.Part1 = newLeftLowerLeg
        motorHip.Parent = character.Torso
    end
end


        
    end,
 })


 local Tab2 = Window:CreateTab("Reações", 4483362458) 

 local Section = Tab2:CreateSection("4 Reações Mehoods")

 local Button = Tab2:CreateButton({
    Name = "St Reação",
    Callback = function()
        game.Workspace.TPSSystem.TPS.Velocity = Vector3.new(100, 100, 100)
    end,
 })

 local Button = Tab2:CreateButton({
    Name = "Mid Reação",
    Callback = function()
        game.Workspace.TPSSystem.TPS.Velocity = Vector3.new(110, 110, 110)
    end,
 })

 local Button = Tab2:CreateButton({
    Name = "Gk Reação",
    Callback = function()
        game.Workspace.TPSSystem.TPS.Velocity = Vector3.new(120, 120, 120)
    end,
 })

 local Button = Tab2:CreateButton({
    Name = "Todas Reações",
    Callback = function()
        loadstring(game:HttpGet("https://pastebin.com/raw/GrePU9TQ"))()
    end,
 })

 
 local Tab3 = Window:CreateTab("Ajudas", 4483362458) 

 local Section = Tab3:CreateSection("Habilidades que ajudam as metodidades")

 local Toggle = Tab3:CreateToggle({
    Name = "Ajudante de Drible Aéreo",
    CurrentValue = false,
    Flag = "Toggled", 
    Callback = function(v148)
        if v148 then
    getgenv().boxsettings = {
        box = {

            boxsize = Vector3.new(v32 or 1, v32 or 1, v32 or 1),
            markerOffset = Vector3.new(0, -1, 0),
            boxtransparency = 1
        }
    }
    
  
    local tpsPart = game.Workspace.TPSSystem.TPS

    local function createTPSPart(parent, referencePart)
        local newTPS = Instance.new("Part")
        newTPS.Name = "TPS"
        newTPS.Size = getgenv().boxsettings.box.boxsize 
        newTPS.Anchored = true
        newTPS.Transparency = getgenv().boxsettings.box.boxtransparency 
        newTPS.Parent = parent 
        return newTPS
    end
    
    local newTPSPart = createTPSPart(tpsPart.Parent, tpsPart)

    v30 = game:GetService("RunService").Heartbeat:Connect(function()
        newTPSPart.Size = Vector3.new(v32 or 1, 0, v32 or 1)
    end)

    v31 = game:GetService("RunService").Heartbeat:Connect(function()
        newTPSPart.CFrame = CFrame.new(tpsPart.Position + getgenv().boxsettings.box.markerOffset)
    end)
end

    end,
 })

 local Input = Tab3:CreateInput({
    Name = "Tamanho do Air Dribble Helper",
    PlaceholderText = "Input Placeholder",
    RemoveTextAfterFocusLost = false,
    Callback = function(v149)
        v32 = tonumber(v149) or 1
			if getgenv().boxsettings then
				getgenv().boxsettings.box.boxsize = Vector3.new(v32, v32, v32)
			end

    end,
 })

 local Button = Tab3:CreateButton({
    Name = "ZZZ Ajuda",
    Callback = function()
    game.Workspace.TPSSystem.TPS.Size = Vector3.new(3, 3, 3)
    game.Workspace.TPSSystem.TPS.Velocity = Vector3.new(200, 200, 200)
    game.Workspace.TPSSystem.TPS.Force = Vector3.new(0, 0, 0)
    end,
 })

 local Button = Tab3:CreateButton({
    Name = "Inf Ajuda",
    Callback = function()
    game.Workspace.TPSSystem.TPS.Size = Vector3.new(2.55, 2.55, 2.55)
    game.Workspace.TPSSystem.TPS.Velocity = Vector3.new(110, 110, 110)
    if game.Lighting[game.Players.LocalPlayer.Name].PreferredFoot.Value == 1 then
        DistanceReach = tonumber(Value)
        game.Players.LocalPlayer.Character["Right leg"].Size = Vector3.new(Value, 0.2, Value)
    elseif game.Lighting[game.Players.LocalPlayer.Name].PreferredFoot.Value == 1 then
        DistanceReach = tonumber(Value)
        game.Players.LocalPlayer.Character["Left Leg"].Size = Vector3.new(Value, 0.2, Value)
    end
    end,
 })

 local Tab4 = Window:CreateTab("GamePasses", 4483362458)

 local Toggle = Tab4:CreateToggle({
    Name = "Blue Flame",
    CurrentValue = false,
    Flag = "Toggle1", 
    Callback = function(v106)
        if v106 then
            game:GetService("Players").LocalPlayer.PlayerGui.Start.GamePassMenu.Items.BlueFlame.Tick.Visible = true
            game:GetService("Players").LocalPlayer.PlayerGui.Start.GamePassMenu.Items.BlueFlame.BlueFlame.Style =
                "RobloxRoundButton"
            game:GetService("Players").LocalPlayer.PlayerGui.Start.PowerShot.Image = "rbxassetid://0"
            game:GetService("Players").LocalPlayer.Backpack.FValue.Value = 2
        else
            game:GetService("Players").LocalPlayer.PlayerGui.Start.GamePassMenu.Items.BlueFlame.Tick.Visible = false
            game:GetService("Players").LocalPlayer.PlayerGui.Start.GamePassMenu.Items.BlueFlame.BlueFlame.Style =
                "RobloxRoundDefaultButton"
            game:GetService("Players").LocalPlayer.PlayerGui.Start.PowerShot.Image = "rbxassetid://0"
            game:GetService("Players").LocalPlayer.Backpack.FValue.Value = 1
        end

    end,
 })

 local Toggle = Tab4:CreateToggle({
    Name = "More Curve",
    CurrentValue = false,
    Flag = "Toggle1", 
    Callback = function(v107)
        if v107 then
            local player = game:GetService("Players").LocalPlayer
            local playerGui = player.PlayerGui.Start.GamePassMenu.Items.WoodenFloor
            local character = player.Character
            local humanoid = character and character:FindFirstChildOfClass("Humanoid")

            playerGui.Tick.Visible = true
            playerGui.WoodenFloor.Style = "RobloxRoundButton"
        
            if humanoid then
                v12 = humanoid.AnimationPlayed:Connect(function(animationTrack)
                    local validAnimations = {
                        "OldMKickL", "OldMKick", "OldLKickL", "OldLKick",
                        "MKickL", "MKick", "LKickL", "LKick",
                        "OldDribbleL", "OldDribble", "DribbleL", "Dribble"
                    }
                    
                    if table.find(validAnimations, animationTrack.Name) then
                        local tpsPart = game.Workspace.TPSSystem.TPS
                        local humanoidRootPart = player.Character:FindFirstChild("HumanoidRootPart")
                        
                        if humanoidRootPart and (humanoidRootPart.Position - tpsPart.Position).Magnitude < 155.45 then
                            local curvingValue = player.Backpack:FindFirstChild("Curving") and player.Backpack.Curving.Value
                            
                            if curvingValue == 155.45 or curvingValue == 154.45 then
                                wait(0.1)
                                
                                local kickAction
                                if curvingValue == 155.45 then
                                    kickAction = game:GetService("Workspace").FE.Actions.KickC1
                                elseif curvingValue == 154.45 then
                                    kickAction = game:GetService("Workspace").FE.Actions.KickC2
                                end
                                
                                if kickAction then
                                    kickAction:FireServer(tpsPart, humanoidRootPart)
                                    wait(0.2)
                                    kickAction:FireServer(tpsPart, humanoidRootPart)
                                end
                            end
                        end
                    end
                end)
            end
        else
            if v12 then
                v12:Disconnect()
            end
            
            local playerGui = game:GetService("Players").LocalPlayer.PlayerGui.Start.GamePassMenu.Items.WoodenFloor
            playerGui.Tick.Visible = false
            playerGui.WoodenFloor.Style = "RobloxRoundDefaultButton"
        end
        
    end,
 })

 local Toggle = Tab4:CreateToggle({
    Name = "Powerfull Tackle",
    CurrentValue = false,
    Flag = "Toggle1", 
    Callback = function(v108)
        local player = game:GetService("Players").LocalPlayer
        local playerGui = player:WaitForChild("PlayerGui")
        local startGui = playerGui:WaitForChild("Start")
        local gamePassMenu = startGui:WaitForChild("GamePassMenu")
        local randomWeatherItem = gamePassMenu:WaitForChild("Items"):WaitForChild("RandomWeather")
        
        local tackleGamePass = startGui:FindFirstChild("TackleGamePass") or Instance.new("BoolValue", startGui)
        tackleGamePass.Name = "TackleGamePass"
        tackleGamePass.Value = false
        
        if v108 then
            randomWeatherItem.Tick.Visible = true
            randomWeatherItem.RandomWeather.Style = "RobloxRoundButton"
            tackleGamePass.Value = true
        
            local humanoid = player.Character and player.Character:FindFirstChildOfClass("Humanoid")
            if humanoid then
                v13 = humanoid.AnimationPlayed:Connect(function(animationTrack)
                    if table.find({"TackleL", "Tackle", "OldTackleL", "OldTackle"}, animationTrack.Name) then
                        local humanoidRootPart = player.Character:FindFirstChild("HumanoidRootPart")
                        local tpsPart = game.Workspace.TPSSystem.TPS
        
                        if humanoidRootPart and (humanoidRootPart.Position - tpsPart.Position).Magnitude < 4.87 then
                            wait(0.8)
                            local kickAction = game:GetService("Workspace").FE.Actions.KickG1
                            if kickAction then
                                kickAction:FireServer(tpsPart, humanoidRootPart, 30, Vector3.new(4000000, 700, 4000000))
                            end
                        end
                    end
                end)
            end
        else
            randomWeatherItem.Tick.Visible = false
            randomWeatherItem.RandomWeather.Style = "RobloxRoundDefaultButton"
            tackleGamePass.Value = false
        
            if v13 then
                v13:Disconnect()
            end
        end
        
    end,
 })

 local Toggle = Tab4:CreateToggle({
    Name = "Faster Cooldown",
    CurrentValue = false,
    Flag = "Toggle1", 
    Callback = function(v117)
        local v118 = game:GetService("Players").LocalPlayer
        if v117 then
            v118.PlayerGui.Start.GamePassMenu.Items.Cooldown.Tick.Visible = true
            v118.PlayerGui.Start.GamePassMenu.Items.Cooldown.Cooldown.Style = "RobloxRoundButton"
            v118.PlayerGui.Start.PowerShot.PowerValue.Value = 30
        else
            v118.PlayerGui.Start.GamePassMenu.Items.Cooldown.Tick.Visible = 
