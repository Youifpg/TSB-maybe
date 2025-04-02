
local Players = game:GetService("Players")
local player = Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()
local humanoid = character:WaitForChild("Humanoid")
local playerGui = player:WaitForChild("PlayerGui")
local deathPosition = nil
local respawnAnimation = "rbxassetid://1"

-- [[ Notify if character is wrong ]]
Hero = game.Players.LocalPlayer.Character:GetAttribute("Character")
if Hero ~= "Bald" then
    game.StarterGui:SetCore("SendNotification", {
        Title = "Wrong Character";
        Text = "use Saitama to work the script!";
        Duration = 5;
    })
    return
end

local function stopAllAnimations(humanoid)
    local animationTracks = humanoid:GetPlayingAnimationTracks()
    for _, track in ipairs(animationTracks) do
        track:Stop()
    end
end

local function onCharacterAdded(character)
    local humanoid = character:WaitForChild("Humanoid")
    
    if deathPosition then
        character:WaitForChild("HumanoidRootPart").CFrame = CFrame.new(deathPosition)
        stopAllAnimations(humanoid)
        task.wait()
        local animation = Instance.new("Animation")
        animation.AnimationId = respawnAnimation
        local animationTrack = humanoid:LoadAnimation(animation)
        animationTrack:Play()
        task.wait(2)
        animationTrack:Stop()
        deathPosition = nil
    end

    humanoid.HealthChanged:Connect(function(health)
        if health <= 0 then
            deathPosition = character:WaitForChild("HumanoidRootPart").Position
        end
    end)
end
task.wait(0)
game.Lighting.TimeOfDay = "00:00:00"
task.wait(0)
local animationId = "103362214977039"

local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()
local humanoid = character:WaitForChild("Humanoid")

local animation = Instance.new("Animation")
animation.AnimationId = "rbxassetid://" .. animationId
local animationTrack = humanoid:LoadAnimation(animation)
animationTrack:Play()
task.wait(0)
local function GetGitSound(GithubSnd,SoundName) --idk what is this for anyway
    local url=GithubSnd
    if not isfile(SoundName..".mp3") then
        writefile(SoundName..".mp3", game:HttpGet(url))
    end
    local sound=Instance.new("Sound")
    sound.SoundId=(getcustomasset or getsynasset)(SoundName..".mp3")
    return sound
end

local Clock = GetGitSound("https://github.com/Kenjihin69/Kenjihin69/blob/main/Screen_Recording_20250122_221218_20250122_222024.mp3?raw=true","shinji spwn1")

Clock.Parent = workspace

Clock.Volume = 4
Clock.TimePosition = 0

Clock:Play()
task.wait(0)
task.spawn(function()
wait(0)
local cutscene = {
    {
["Fov"] = 66.477211,
        ["Cf"] = CFrame.new(8.34422302, -0.162785053, -11.38744354, 0.65602982, -0.0559347011, -0.75265944, 0.102677561, 0.994592607, 0.0155811375, 0.747718096, -0.0875029415, 0.6582222)
},
    {
        ["Fov"] = 66.477211,
        ["Cf"] = CFrame.new(8.34422302, -0.162785053, -11.38744354, 0.65602982, -0.0559347011, -0.75265944, 0.102677561, 0.994592607, 0.0155811375, 0.747718096, -0.0875029415, 0.6582222)
},
    {
["Fov"] = 66.477211,
        ["Cf"] = CFrame.new(8.34422302, -0.162785053, -11.38744354, 0.65602982, -0.0559347011, -0.75265944, 0.102677561, 0.994592607, 0.0155811375, 0.747718096, -0.0875029415, 0.6582222)
},
    {
["Fov"] = 66.477211,
        ["Cf"] = CFrame.new(8.34422302, -0.162785053, -11.38744354, 0.65602982, -0.0559347011, -0.75265944, 0.102677561, 0.994592607, 0.0155811375, 0.747718096, -0.0875029415, 0.6582222)
},
    {
["Fov"] = 66.477211,
        ["Cf"] = CFrame.new(8.34422302, -0.162785053, -11.38744354, 0.65602982, -0.0559347011, -0.75265944, 0.102677561, 0.994592607, 0.0155811375, 0.747718096, -0.0875029415, 0.6582222)
},
    {
["Fov"] = 66.477211,
        ["Cf"] = CFrame.new(8.34422302, -0.162785053, -11.38744354, 0.65602982, -0.0559347011, -0.75265944, 0.102677561, 0.994592607, 0.0155811375, 0.747718096, -0.0875029415, 0.6582222)
},
    {
["Fov"] = 66.477211,
        ["Cf"] = CFrame.new(8.34422302, -0.162785053, -11.38744354, 0.65602982, -0.0559347011, -0.75265944, 0.102677561, 0.994592607, 0.0155811375, 0.747718096, -0.0875029415, 0.6582222)
},
    {
["Fov"] = 66.477211,
        ["Cf"] = CFrame.new(8.34422302, -0.162785053, -11.38744354, 0.65602982, -0.0559347011, -0.75265944, 0.102677561, 0.994592607, 0.0155811375, 0.747718096, -0.0875029415, 0.6582222)
},
    {
["Fov"] = 66.477211,
        ["Cf"] = CFrame.new(8.34422302, -0.162785053, -11.38744354, 0.65602982, -0.0559347011, -0.75265944, 0.102677561, 0.994592607, 0.0155811375, 0.747718096, -0.0875029415, 0.6582222)
},
    {
["Fov"] = 66.477211,
        ["Cf"] = CFrame.new(8.34422302, -0.162785053, -11.38744354, 0.65602982, -0.0559347011, -0.75265944, 0.102677561, 0.994592607, 0.0155811375, 0.747718096, -0.0875029415, 0.6582222)
},
    {
        ["Fov"] = 66.477211,
        ["Cf"] = CFrame.new(8.34422302, -0.162785053, -11.38744354, 0.65602982, -0.0559347011, -0.75265944, 0.102677561, 0.994592607, 0.0155811375, 0.747718096, -0.0875029415, 0.6582222)
    }
}
    local player = game.Players.LocalPlayer
    local camera = workspace.CurrentCamera
    camera.CameraType = Enum.CameraType.Scriptable
    local humanoidRootPart = player.Character.HumanoidRootPart
local e = humanoidRootPart.CFrame - humanoidRootPart.CFrame.LookVector * 25.5
local v2 = e * CFrame.Angles(0, math.rad(57), 0) * CFrame.new(10, 0, -3)
    for i, frame in ipairs(cutscene) do
        camera.CFrame = v2:ToWorldSpace(frame.Cf)
        camera.FieldOfView = frame.Fov
        wait(00000.6)
    end
    camera.CameraType = Enum.CameraType.Custom
end) 
task.wait(1.4)
local Test = game.ReplicatedStorage.Resources.LastBreath.Arm.Arm.Attachment
local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("Left Arm")

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(255, 255, 0)) -- Set color to purple
        child:Emit(15)
        child.Enabled = true
    end
end

task.wait(0)
task.spawn(function()
wait(0)
local cutscene = {
    {
["Fov"] = 66.477211,
        ["Cf"] = CFrame.new(8.34422302, -0.162785053, -11.38744354, 0.65602982, -0.0559347011, -0.75265944, 0.102677561, 0.994592607, 0.0155811375, 0.747718096, -0.0875029415, 0.6582222)
},
    {
        ["Fov"] = 66.477211,
        ["Cf"] = CFrame.new(8.34422302, -0.162785053, -11.38744354, 0.65602982, -0.0559347011, -0.75265944, 0.102677561, 0.994592607, 0.0155811375, 0.747718096, -0.0875029415, 0.6582222)
},
    {
["Fov"] = 66.477211,
        ["Cf"] = CFrame.new(8.34422302, -0.162785053, -11.38744354, 0.65602982, -0.0559347011, -0.75265944, 0.102677561, 0.994592607, 0.0155811375, 0.747718096, -0.0875029415, 0.6582222)
},
    {
["Fov"] = 66.477211,
        ["Cf"] = CFrame.new(8.34422302, -0.162785053, -11.38744354, 0.65602982, -0.0559347011, -0.75265944, 0.102677561, 0.994592607, 0.0155811375, 0.747718096, -0.0875029415, 0.6582222)
},
    {
["Fov"] = 66.477211,
        ["Cf"] = CFrame.new(8.34422302, -0.162785053, -11.38744354, 0.65602982, -0.0559347011, -0.75265944, 0.102677561, 0.994592607, 0.0155811375, 0.747718096, -0.0875029415, 0.6582222)
},
    {
["Fov"] = 66.477211,
        ["Cf"] = CFrame.new(8.34422302, -0.162785053, -11.38744354, 0.65602982, -0.0559347011, -0.75265944, 0.102677561, 0.994592607, 0.0155811375, 0.747718096, -0.0875029415, 0.6582222)
},
    {
["Fov"] = 66.477211,
        ["Cf"] = CFrame.new(8.34422302, -0.162785053, -11.38744354, 0.65602982, -0.0559347011, -0.75265944, 0.102677561, 0.994592607, 0.0155811375, 0.747718096, -0.0875029415, 0.6582222)
},
    {
["Fov"] = 66.477211,
        ["Cf"] = CFrame.new(8.34422302, -0.162785053, -11.38744354, 0.65602982, -0.0559347011, -0.75265944, 0.102677561, 0.994592607, 0.0155811375, 0.747718096, -0.0875029415, 0.6582222)
},
    {
        ["Fov"] = 66.477211,
        ["Cf"] = CFrame.new(8.34422302, -0.162785053, -11.38744354, 0.65602982, -0.0559347011, -0.75265944, 0.102677561, 0.994592607, 0.0155811375, 0.747718096, -0.0875029415, 0.6582222)
    }
}
    local player = game.Players.LocalPlayer
    local camera = workspace.CurrentCamera
    camera.CameraType = Enum.CameraType.Scriptable
    local humanoidRootPart = player.Character.HumanoidRootPart
local e = humanoidRootPart.CFrame - humanoidRootPart.CFrame.LookVector * 25.5
local v2 = e * CFrame.Angles(0, math.rad(57), 0) * CFrame.new(10, 0, -3)
    for i, frame in ipairs(cutscene) do
        camera.CFrame = v2:ToWorldSpace(frame.Cf)
        camera.FieldOfView = frame.Fov
        wait(0.4)
    end
    camera.CameraType = Enum.CameraType.Custom
end)
task.wait(0)
local function GetGitSound(GithubSnd,SoundName) --idk what is this for anyway
    local url=GithubSnd
    if not isfile(SoundName..".mp3") then
        writefile(SoundName..".mp3", game:HttpGet(url))
    end
    local sound=Instance.new("Sound")
    sound.SoundId=(getcustomasset or getsynasset)(SoundName..".mp3")
    return sound
end

local Clock = GetGitSound("https://github.com/Kenjihin69/Kenjihin69/blob/main/Screen_Recording_20250123_091429%20%5Bvocals%5D.mp3?raw=true","shinji this pow")

Clock.Parent = workspace

Clock.Volume = 4
Clock.TimePosition = 0

Clock:Play()
task.wait(0)
local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()

local function anchorCharacter()
    character.HumanoidRootPart.Anchored = true
    wait(3.4) -- Wait
    character.HumanoidRootPart.Anchored = false
end

--ass function
anchorCharacter()
task.wait(0)
local player = game.Players.LocalPlayer
local playerGui = player:WaitForChild("PlayerGui")
local s = Instance.new("ScreenGui")
s.Parent = playerGui

local textLabel = Instance.new("TextLabel")
textLabel.Parent = s
textLabel.Position = UDim2.new(0.5, -200, 0.8, -50)
textLabel.Size = UDim2.new(0, 400, 0, 50)
textLabel.TextSize = 27
textLabel.TextColor3 = Color3.fromRGB(255, 255, 0) --text color
textLabel.Font = Enum.Font.Antique -- font here
textLabel.BackgroundTransparency = 1
textLabel.Text = "" -- dont change
textLabel.TextStrokeTransparency = 0
textLabel.TextStrokeColor3 = Color3.fromRGB(0, 0, 0) --stroke color here

local function type(text)
    local index = 1
    while index <= #text do
        textLabel.Text = string.sub(text, 1, index)
        index = index + 1
        wait(0.02)
    end
end

local function f()
    for i = 1, 20 do
        textLabel.TextTransparency = i / 20
        wait(0.01)
    end
end
local function fs()
coroutine.wrap(function()
textLabel.TextStrokeTransparency = 0.1
task.wait(0.1)
textLabel.TextStrokeTransparency = 0.2
task.wait(0.1)
textLabel.TextStrokeTransparency = 0.3
task.wait(0.1)
textLabel.TextStrokeTransparency = 0.4
task.wait(0.1)
textLabel.TextStrokeTransparency = 0.5
task.wait(0.1)
textLabel.TextStrokeTransparency = 0.6
task.wait(0.1)
textLabel.TextStrokeTransparency = 0.7
task.wait(0.1)
textLabel.TextStrokeTransparency = 0.8
task.wait(0.1)
textLabel.TextStrokeTransparency = 0.9
task.wait(0.1)
textLabel.TextStrokeTransparency = 1
end)()
end
coroutine.wrap(function()
    local m = "THIS POWER" -- text here
    type(m)
    wait(0)
    fs() -- this for stroke lmao
    f()
end)()
task.wait(1)
test:Destroy()

task.wait(0)
local Test = game.ReplicatedStorage.Resources.FinalEffects.HeadEffect.LEye

local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("Head")
test.CFrame = test.CFrame * CFrame.new(0.3, 0, -1.3)
for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(0, 125, 255)) -- Set color to purple
        child:Emit(20)
        
    end
end
task.wait(0)
local Test = game.ReplicatedStorage.Resources.FinalEffects.HeadEffect.LEye

local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("Head")
test.CFrame = test.CFrame * CFrame.new(0, 0, -1.3)
for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(0, 125, 255)) -- Set color to purple
        child:Emit(20)
        
    end
end
task.wait(0)
animationTrack:Stop()
task.wait(0)
-- Services
local Players = game:GetService("Players")
local TweenService = game:GetService("TweenService")

-- Local Player
local player = Players.LocalPlayer
local playerGui = player:WaitForChild("PlayerGui")

-- Color tweening function
local function tweenColor(imageLabel, startColor, endColor, duration)
    local tweenInfo = TweenInfo.new(duration, Enum.EasingStyle.Linear, Enum.EasingDirection.InOut, -1, true)
    local goal = {ImageColor3 = endColor}
    local tween = TweenService:Create(imageLabel, tweenInfo, goal)
    tween:Play()
end

-- GUI and color adjustment function
local function updateBarColor()
    -- Find the ScreenGui on the screen
    local screenGui = playerGui:FindFirstChild("ScreenGui")
    if not screenGui then return end

    -- Find the MagicHealth Frame
    local magicHealthFrame = screenGui:FindFirstChild("MagicHealth")
    if not magicHealthFrame then return end

    -- Find the Health Frame
    local healthFrame = magicHealthFrame:FindFirstChild("Health")
    if not healthFrame then return end

    -- Find the Bar Frame
    local barFrame = healthFrame:FindFirstChild("Bar")
    if not barFrame then return end

    -- Find the ImageLabel with ImageColor3 property inside the Bar Frame
    local imageLabel = barFrame:FindFirstChild("Bar")
    if not imageLabel or not imageLabel:IsA("ImageLabel") then return end

    -- Set initial color to dark red
    imageLabel.ImageColor3 = Color3.fromRGB(0, 125, 255) -- Dark red

    -- Smooth transition from dark red to none
    tweenColor(imageLabel, Color3.fromRGB(0, 125, 255), Color3.fromRGB(0, 125, 255), 2)
end

-- Check the GUI again when the character resets
local function onCharacterAdded(character)
    -- Update the GUI
    updateBarColor()
end

-- Check the local player's character
local function onPlayerAdded()
    local character = player.Character or player.CharacterAdded:Wait()
    onCharacterAdded(character)

    -- Check again when the character changes
    player.CharacterAdded:Connect(onCharacterAdded)
end

-- Check when the player is added
Players.PlayerAdded:Connect(onPlayerAdded)
if player then
    onPlayerAdded()
end
local player = game.Players.LocalPlayer

local playerGui = player.PlayerGui

local hotbar = playerGui:FindFirstChild("Hotbar")

local backpack = hotbar:FindFirstChild("Backpack")

local hotbarFrame = backpack:FindFirstChild("Hotbar")

local baseButton = hotbarFrame:FindFirstChild("1").Base

local ToolName = baseButton.ToolName


ToolName.Text = "Dragon Rush"


local player = game.Players.LocalPlayer

local playerGui = player.PlayerGui

local hotbar = playerGui:FindFirstChild("Hotbar")

local backpack = hotbar:FindFirstChild("Backpack")

local hotbarFrame = backpack:FindFirstChild("Hotbar")

local baseButton = hotbarFrame:FindFirstChild("2").Base

local ToolName = baseButton.ToolName


ToolName.Text = "Quick Kick"


local player = game.Players.LocalPlayer

local playerGui = player.PlayerGui

local hotbar = playerGui:FindFirstChild("Hotbar")

local backpack = hotbar:FindFirstChild("Backpack")

local hotbarFrame = backpack:FindFirstChild("Hotbar")

local baseButton = hotbarFrame:FindFirstChild("3").Base

local ToolName = baseButton.ToolName


ToolName.Text = "Speed Of Fist"


local player = game.Players.LocalPlayer

local playerGui = player.PlayerGui

local hotbar = playerGui:FindFirstChild("Hotbar")

local backpack = hotbar:FindFirstChild("Backpack")

local hotbarFrame = backpack:FindFirstChild("Hotbar")

local baseButton = hotbarFrame:FindFirstChild("4").Base

local ToolName = baseButton.ToolName


ToolName.Text = "Dragon Barrier"


local Players = game:GetService("Players")

local player = Players.LocalPlayer

local playerGui = player:WaitForChild("PlayerGui")


local function findGuiAndSetText()

    local screenGui = playerGui:FindFirstChild("ScreenGui")

    if screenGui then

        local magicHealthFrame = screenGui:FindFirstChild("MagicHealth")

        if magicHealthFrame then

            local textLabel = magicHealthFrame:FindFirstChild("TextLabel")

            if textLabel then

                textLabel.Text = "WRATH OF THE DRAGON"

            end

        end

    end

end


playerGui.DescendantAdded:Connect(findGuiAndSetText)

findGuiAndSetText()


local animationId = 10468665991


local player = game.Players.LocalPlayer

local character = player.Character or player.CharacterAdded:Wait()

local humanoid = character:WaitForChild("Humanoid")


local function onAnimationPlayed(animationTrack)

    if animationTrack.Animation.AnimationId == "rbxassetid://" .. animationId then


local p = game.Players.LocalPlayer

local Humanoid = p.Character:WaitForChild("Humanoid")


for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do

    animTrack:Stop()

end


local AnimAnim = Instance.new("Animation")

AnimAnim.AnimationId = "rbxassetid://140164642047188"

local Anim = Humanoid:LoadAnimation(AnimAnim)


local startTime = 6.8


Anim:Play()

Anim:AdjustSpeed(0)

Anim.TimePosition = startTime

Anim:AdjustSpeed(1.3)
local function GetGitSound(GithubSnd,SoundName) --idk what is this for anyway
    local url=GithubSnd
    if not isfile(SoundName..".mp3") then
        writefile(SoundName..".mp3", game:HttpGet(url))
    end
    local sound=Instance.new("Sound")
    sound.SoundId=(getcustomasset or getsynasset)(SoundName..".mp3")
    return sound
end

local Clock = GetGitSound("https://github.com/Kenjihin69/Kenjihin69/blob/main/Screen_Recording_20250121_200504_20250121_201031.mp3?raw=true","shinji Iahh")

Clock.Parent = workspace

Clock.Volume = 5
Clock.TimePosition = 0

Clock:Play()
task.wait(0.4)
local fx7 = game.ReplicatedStorage.Resources.FiveSeasonsFX["CharFX"].EyeEmit:Clone()
fx7.Parent = game.Players.LocalPlayer.Character["Head"]
for _, child in ipairs(fx7:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(0, 125, 255)) -- Set color to purple
        child:Emit(6) -- Emit 1 particle
    end
end 
local fx7 = Game.ReplicatedStorage.Resources.Ricochet["Impact2"].Part.Attachment:Clone()
fx7.Parent = game.Players.LocalPlayer.Character["Torso"]
for _, child in ipairs(fx7:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(0, 125, 255)) -- Set color to purple
        child:Emit(4) -- Emit 1 particle
    end
end local fx7 = Game.ReplicatedStorage.Resources.Ricochet["Grab"].Part.Attachment:Clone()
fx7.Parent = game.Players.LocalPlayer.Character["Torso"]
for _, child in ipairs(fx7:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(0, 125, 255)) -- Set color to purple
        child:Emit(4) -- Emit 1 particle
    end
end local fx7 = Game.ReplicatedStorage.Resources.Ricochet["TatsuVa2r"].Tatsu.Main:Clone()
fx7.Parent = game.Players.LocalPlayer.Character["Torso"]
for _, child in ipairs(fx7:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(0, 85, 255)) -- Set color to purple
        child:Emit(4) -- Emit 1 particle
    end
end local fx7 = Game.ReplicatedStorage.Resources.Ricochet["FinalLand"].Part.Attachment:Clone()
fx7.Parent = game.Players.LocalPlayer.Character["Torso"]
for _, child in ipairs(fx7:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(0, 125, 255)) -- Set color to purple
        child:Emit(3) -- Emit 1 particle
    end
end
task.wait(0)

local Test = game.ReplicatedStorage.Resources.Ricochet.Upper.ImpactWhite.ImpactWhite.Windy

local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("HumanoidRootPart")

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
        child:Emit(15)

    end
end
task.wait(0)

local Test = game.ReplicatedStorage.Resources.Trashcan2.Thing.Middle.Attachment

local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("HumanoidRootPart")

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
        child:Emit(1)
        
    end
end
task.wait(0)

local Test = game.ReplicatedStorage.Resources.Trashcan2.Throw.Throw.Attachment

local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("HumanoidRootPart")

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
        child:Emit(15)
        
    end
end
task.wait(0)
local Test = game.ReplicatedStorage.Resources.Trashcan2.Throw.Throw.Front

local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("HumanoidRootPart")

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
        child:Emit(15)
        
    end
end
task.wait(0)
loadstring(game:HttpGet('https://raw.githubusercontent.com/kenkenplaygt/kenkenplaygt/refs/heads/main/Name%20Shinji%20Po'))()
    end

end


humanoid.AnimationPlayed:Connect(onAnimationPlayed)


local animationId = 10466974800


local player = game.Players.LocalPlayer

local character = player.Character or player.CharacterAdded:Wait()

local humanoid = character:WaitForChild("Humanoid")


local function onAnimationPlayed(animationTrack)

    if animationTrack.Animation.AnimationId == "rbxassetid://" .. animationId then


local p = game.Players.LocalPlayer

local Humanoid = p.Character:WaitForChild("Humanoid")


for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do

    animTrack:Stop()

end


local AnimAnim = Instance.new("Animation")

AnimAnim.AnimationId = "rbxassetid://17799224866"

local Anim = Humanoid:LoadAnimation(AnimAnim)


local startTime = 0


Anim:Play()

Anim:AdjustSpeed(0)

Anim.TimePosition = startTime

Anim:AdjustSpeed(1)

local ambatukam = game.Players.LocalPlayer.Character:WaitForChild("BarrageBind")
ambatukam:Destroy()
task.wait(0)
local Test = game.ReplicatedStorage.Resources.HammerVfx.FloorFx.Attachment
local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("HumanoidRootPart")

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(0, 125, 255)) -- Set color to purple
        child:Emit(20)
        child.Enabled = true
    end
end
   task.wait(1.2)
    Anim:Stop()
task.wait(0)
test:Destroy()
task.wait(0)
loadstring(game:HttpGet('https://raw.githubusercontent.com/kenkenplaygt/kenkenplaygt/refs/heads/main/Name%20Shinji%20Po'))()
    end

end


humanoid.AnimationPlayed:Connect(onAnimationPlayed)


local animationId = 10471336737


local player = game.Players.LocalPlayer

local character = player.Character or player.CharacterAdded:Wait()

local humanoid = character:WaitForChild("Humanoid")


local function onAnimationPlayed(animationTrack)

    if animationTrack.Animation.AnimationId == "rbxassetid://" .. animationId then


local p = game.Players.LocalPlayer

local Humanoid = p.Character:WaitForChild("Humanoid")


for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do

    animTrack:Stop()

end


local AnimAnim = Instance.new("Animation")

AnimAnim.AnimationId = "rbxassetid://94020267622363"

local Anim = Humanoid:LoadAnimation(AnimAnim)


local startTime = 11.2


Anim:Play()

Anim:AdjustSpeed(0)

Anim.TimePosition = startTime

Anim:AdjustSpeed(1.9)
local function GetGitSound(GithubSnd,SoundName) --idk what is this for anyway
    local url=GithubSnd
    if not isfile(SoundName..".mp3") then
        writefile(SoundName..".mp3", game:HttpGet(url))
    end
    local sound=Instance.new("Sound")
    sound.SoundId=(getcustomasset or getsynasset)(SoundName..".mp3")
    return sound
end

local Clock = GetGitSound("https://github.com/Kenjihin69/Kenjihin69/blob/main/Screen_Recording_20250118_214343_20250121_192557.mp3?raw=true","shinji I kill you")

Clock.Parent = workspace

Clock.Volume = 4
Clock.TimePosition = 0

Clock:Play()
task.wait(0.2)
local Test = game.ReplicatedStorage.Resources.CrushingPull.Stomp.Stomp.Attachment
local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character["Head"]

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
        child:Emit(10)
    end
end
task.wait(0.5)
    Anim:Stop()
task.wait(0)
local player = game.Players.LocalPlayer
local playerGui = player:WaitForChild("PlayerGui")
local s = Instance.new("ScreenGui")
s.Parent = playerGui

local textLabel = Instance.new("TextLabel")
textLabel.Parent = s
textLabel.Position = UDim2.new(0.5, -200, 0.8, -50)
textLabel.Size = UDim2.new(0, 400, 0, 50)
textLabel.TextSize = 27
textLabel.TextColor3 = Color3.fromRGB(255, 255, 0) --text color
textLabel.Font = Enum.Font.Antique -- font here
textLabel.BackgroundTransparency = 1
textLabel.Text = "" -- dont change
textLabel.TextStrokeTransparency = 0
textLabel.TextStrokeColor3 = Color3.fromRGB(0, 0, 0) --stroke color here

local function type(text)
    local index = 1
    while index <= #text do
        textLabel.Text = string.sub(text, 1, index)
        index = index + 1
        wait(0.02)
    end
end

local function f()
    for i = 1, 20 do
        textLabel.TextTransparency = i / 20
        wait(0.01)
    end
end
local function fs()
coroutine.wrap(function()
textLabel.TextStrokeTransparency = 0.1
task.wait(0.1)
textLabel.TextStrokeTransparency = 0.2
task.wait(0.1)
textLabel.TextStrokeTransparency = 0.3
task.wait(0.1)
textLabel.TextStrokeTransparency = 0.4
task.wait(0.1)
textLabel.TextStrokeTransparency = 0.5
task.wait(0.1)
textLabel.TextStrokeTransparency = 0.6
task.wait(0.1)
textLabel.TextStrokeTransparency = 0.7
task.wait(0)
textLabel.TextStrokeTransparency = 0.8
task.wait(0)
textLabel.TextStrokeTransparency = 0.9
task.wait(0)
textLabel.TextStrokeTransparency = 1
end)()
end
coroutine.wrap(function()
    local m = " I'LL KILL YOU!" -- text here
    type(m)
    wait(0)
    fs() -- this for stroke lmao
    f()
end)()
task.wait(0)
loadstring(game:HttpGet('https://raw.githubusercontent.com/kenkenplaygt/kenkenplaygt/refs/heads/main/Name%20Shinji%20Po'))()
    end

end


humanoid.AnimationPlayed:Connect(onAnimationPlayed)


local animationId = 12510170988


local player = game.Players.LocalPlayer

local character = player.Character or player.CharacterAdded:Wait()

local humanoid = character:WaitForChild("Humanoid")


local function onAnimationPlayed(animationTrack)

    if animationTrack.Animation.AnimationId == "rbxassetid://" .. animationId then

local p = game.Players.LocalPlayer

local Humanoid = p.Character:WaitForChild("Humanoid")


for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do

    animTrack:Stop()

end


local AnimAnim = Instance.new("Animation")

AnimAnim.AnimationId = "rbxassetid://16597912086"

local Anim = Humanoid:LoadAnimation(AnimAnim)


local startTime = 0


Anim:Play()

Anim:AdjustSpeed(0)

Anim.TimePosition = startTime

Anim:AdjustSpeed(1)
task.wait(0.5)
local e = Game.ReplicatedStorage.Resources.Sorcerer.LimitlessBarrier["Core"].EndEmit.Ground:Clone()
e.Parent = game.Players.LocalPlayer.Character["HumanoidRootPart"]
for _, child in ipairs(e:GetChildren()) do
    if child:IsA("ParticleEmitter") then
        child:Emit(2)
    end
end
task.wait(0)
local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()

local function anchorCharacter()
    character.HumanoidRootPart.Anchored = true
    wait(0.4) -- Wait
    character.HumanoidRootPart.Anchored = false
end

--unction
anchorCharacter()
task.wait(0)
loadstring(game:HttpGet('https://raw.githubusercontent.com/kenkenplaygt/kenkenplaygt/refs/heads/main/Name%20Shinji%20Po'))()
    end

end

humanoid.AnimationPlayed:Connect(onAnimationPlayed)

local animationId = 11343318134 ---ult 1


local player = game.Players.LocalPlayer

local character = player.Character or player.CharacterAdded:Wait()

local humanoid = character:WaitForChild("Humanoid")


local function onAnimationPlayed(animationTrack)

    if animationTrack.Animation.AnimationId == "rbxassetid://" .. animationId then

local p = game.Players.LocalPlayer

local Humanoid = p.Character:WaitForChild("Humanoid")


for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do

    animTrack:Stop()

end


local AnimAnim = Instance.new("Animation")

AnimAnim.AnimationId = "rbxassetid://76530443909428"

local Anim = Humanoid:LoadAnimation(AnimAnim)


local startTime = 0

Anim:Play()

Anim:AdjustSpeed(0)

Anim.TimePosition = startTime

Anim:AdjustSpeed(0.7)
local Test = game.ReplicatedStorage.Emotes.DemonParticles.RootAttachment
local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("HumanoidRootPart")

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(0, 125, 255)) -- Set color to purple
        child:Emit(1)
    end
end
task.wait(5.5)
Players = game:GetService("Players")
 local speaker = Players.LocalPlayer
 workspace.CurrentCamera:remove()
     wait(.1)
     workspace.CurrentCamera.CameraSubject = speaker.Character:FindFirstChildWhichIsA('Humanoid')
     workspace.CurrentCamera.CameraType = "Custom"
     speaker.CameraMinZoomDistance = 0.5
     speaker.CameraMaxZoomDistance = 400
     speaker.CameraMode = "Classic"
     speaker.Character.Head.Anchored = false
task.wait(0)
local function GetGitSound(GithubSnd,SoundName) --idk what is this for anyway
    local url=GithubSnd
    if not isfile(SoundName..".mp3") then
        writefile(SoundName..".mp3", game:HttpGet(url))
    end
    local sound=Instance.new("Sound")
    sound.SoundId=(getcustomasset or getsynasset)(SoundName..".mp3")
    return sound
end
local Clock = GetGitSound("https://github.com/Kenjihin69/Kenjihin69/blob/main/Screen_Recording_20250115_063749.mp3?raw=true","shinji scream")

Clock.Parent = workspace

Clock.Volume = 7
Clock.TimePosition = 0

Clock:Play()

task.wait(1)
local AnimAnim2 = Instance.new("Animation")

AnimAnim2.AnimationId = "rbxassetid://140164642047188"

local Anim2 = Humanoid:LoadAnimation(AnimAnim2)


local startTime = 6.8


Anim:Stop()

Anim2:Play()

Anim2:AdjustSpeed(0)

Anim2.TimePosition = startTime

Anim2:AdjustSpeed(0.6)
task.wait(0)
-- Get the player's camera
local player = game.Players.LocalPlayer
local camera = game.Workspace.CurrentCamera

-- Set the camera's CameraType to Scriptable (this "freezes" the camera)
camera.CameraType = Enum.CameraType.Scriptable

-- Get the player's position
local playerPosition = player.Character.HumanoidRootPart.Position

-- Set the camera's position above the player (e.g., 50 units above)
local freezePosition = playerPosition + Vector3.new(-5, 1, -5) -- x, y, z coordinates, y is higher than player's position

-- Set the camera's CFrame (position + orientation)
camera.CFrame = CFrame.new(freezePosition)

-- Optional: Make the camera look at the player (or another point if desired)
camera.CFrame = CFrame.new(freezePosition, playerPosition)
task.wait(0)
local Test = game.ReplicatedStorage.Emotes.DemonParticles.RootAttachment
local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("HumanoidRootPart")

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(0, 125, 255)) -- Set color to purple
        child:Emit(1)
    end
end
task.wait(1.6)
local Test = game.ReplicatedStorage.Resources.Sunrise.FinalFX.Explode.Attachment
local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("HumanoidRootPart")

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(0, 125, 255)) -- Set color to purple
        child:Emit(10)
        end
end
task.wait(0)
local Test = game.ReplicatedStorage.Resources.KJEffects.lastkick.Attachment
local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("HumanoidRootPart")

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
        child:Emit(15)
    end
end
task.wait(0)
Clock:Stop()    
task.wait(0.6)
Players = game:GetService("Players")
 local speaker = Players.LocalPlayer
 workspace.CurrentCamera:remove()
     wait(.1)
     workspace.CurrentCamera.CameraSubject = speaker.Character:FindFirstChildWhichIsA('Humanoid')
     workspace.CurrentCamera.CameraType = "Custom"
     speaker.CameraMinZoomDistance = 0.5
     speaker.CameraMaxZoomDistance = 400
     speaker.CameraMode = "Classic"
     speaker.Character.Head.Anchored = false

    end

end
humanoid.AnimationPlayed:Connect(onAnimationPlayed)


local animationId = 11365563255 --- two ult


local player = game.Players.LocalPlayer

local character = player.Character or player.CharacterAdded:Wait()

local humanoid = character:WaitForChild("Humanoid")


local function onAnimationPlayed(animationTrack)

    if animationTrack.Animation.AnimationId == "rbxassetid://" .. animationId then

local p = game.Players.LocalPlayer

local Humanoid = p.Character:WaitForChild("Humanoid")


for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do

    animTrack:Stop()

end


local AnimAnim = Instance.new("Animation")

AnimAnim.AnimationId = "rbxassetid://128022763591042"

local Anim = Humanoid:LoadAnimation(AnimAnim)


local startTime = 0.6


Anim:Play()

Anim:AdjustSpeed(0)

Anim.TimePosition = startTime

Anim:AdjustSpeed(1)

local fx7 = game.ReplicatedStorage.Resources.FiveSeasonsFX["CharFX"].EyeEmit:Clone()
fx7.Parent = game.Players.LocalPlayer.Character["Head"]
for _, child in ipairs(fx7:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(0, 125, 255)) -- Set color to purple
        child:Emit(6) -- Emit 1 particle
    end
end 
task.wait(0.4)
local AnimAnim2 = Instance.new("Animation")

AnimAnim2.AnimationId = "rbxassetid://136370737633649"

local Anim2 = Humanoid:LoadAnimation(AnimAnim2)


local startTime = 4.3


Anim:Stop()

Anim2:Play()

Anim2:AdjustSpeed(0)

Anim2.TimePosition = startTime

Anim2:AdjustSpeed(0000000000.1)

local Test = game.ReplicatedStorage.Resources.Sunrise.Constant2.Part.Constant

local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("HumanoidRootPart")

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(0, 125, 255)) -- Set color to purple
        child:Emit(20)
        child.Enabled = true
    end
end
task.wait(0.3)
-- Get the player's camera
local player = game.Players.LocalPlayer
local camera = game.Workspace.CurrentCamera

-- Set the camera's CameraType to Scriptable (this "freezes" the camera)
camera.CameraType = Enum.CameraType.Scriptable

-- Get the player's position
local playerPosition = player.Character.HumanoidRootPart.Position

-- Set the camera's position above the player (e.g., 50 units above)
local freezePosition = playerPosition + Vector3.new(50, 70 ,50) -- x, y, z coordinates, y is higher than player's position

-- Set the camera's CFrame (position + orientation)
camera.CFrame = CFrame.new(freezePosition)

-- Optional: Make the camera look at the player (or another point if desired)
camera.CFrame = CFrame.new(freezePosition, playerPosition)
task.wait(1)
-- best Cframe fly function
coroutine.wrap(function()
    local Players = game:GetService("Players")
    local player = game.Players.LocalPlayer
    local RunService = game:GetService("RunService")
    local Workspace = game:GetService("Workspace")
    local Camera = Workspace.CurrentCamera

    local character = player.Character or player.CharacterAdded:Wait()
    local humanoidRootPart = character:WaitForChild("HumanoidRootPart")

    local normalGravity = Workspace.Gravity
    local spinSpeed = 800
    local spinDuration = 3
    local initialRadius = 200
    local finalRadius = 1
    local riseHeight = 0
    local riseDuration = 3

    local function getNearestHumanoid()
        local nearestHumanoid, shortestDistance
        for _, descendant in ipairs(Workspace.Live:GetDescendants()) do
            if descendant:IsA("Humanoid") and descendant.Parent.Name ~= game.Players.LocalPlayer.Character.Name then
                local humanoidRoot = descendant.Parent:FindFirstChild("HumanoidRootPart")
                if humanoidRoot then
                    local distance = (humanoidRootPart.Position - humanoidRoot.Position).Magnitude
                    if not nearestHumanoid or distance < shortestDistance then
                        nearestHumanoid, shortestDistance = humanoidRoot, distance
                    end
                end
            end
        end
        return nearestHumanoid
    end

    local function spinAndRise()
        Workspace.Gravity = 0

        local startTime = tick()
        local originalPosition = humanoidRootPart.Position
        local nearestHumanoid = getNearestHumanoid()

        while tick() - startTime < spinDuration do
            local elapsedTime = tick() - startTime
            local angle = math.rad(spinSpeed) * elapsedTime
            local progress = elapsedTime / spinDuration

            local currentRadius = initialRadius + (finalRadius - initialRadius) * progress
            local xOffset, zOffset = math.cos(angle) * currentRadius, math.sin(angle) * currentRadius
            local riseAmount = math.min(riseHeight * elapsedTime / riseDuration, riseHeight)

            local newPosition = originalPosition + Vector3.new(xOffset, riseAmount, zOffset)
            if nearestHumanoid then
                humanoidRootPart.CFrame = CFrame.new(newPosition, nearestHumanoid.Position)
            else
                humanoidRootPart.Position = newPosition
            end

            RunService.Stepped:Wait()
        end

       
        Workspace.Gravity = normalGravity
    end

    spinAndRise()
end)()
task.wait(0.5)
local AnimAnim2 = Instance.new("Animation")

AnimAnim2.AnimationId = "rbxassetid://79761806706382"

local Anim2 = Humanoid:LoadAnimation(AnimAnim2)


local startTime = 0


Anim2:Stop()

Anim2:Play()

Anim2:AdjustSpeed(0)

Anim2.TimePosition = startTime

Anim2:AdjustSpeed(0.9)
task.wait(2.6)
-- Get the player's camera
local player = game.Players.LocalPlayer
local camera = game.Workspace.CurrentCamera

-- Set the camera's CameraType to Scriptable (this "freezes" the camera)
camera.CameraType = Enum.CameraType.Scriptable

-- Get the player's position
local playerPosition = player.Character.HumanoidRootPart.Position

-- Set the camera's position above the player (e.g., 50 units above)
local freezePosition = playerPosition + Vector3.new(-7, 1, -7) -- x, y, z coordinates, y is higher than player's position

-- Set the camera's CFrame (position + orientation)
camera.CFrame = CFrame.new(freezePosition)

-- Optional: Make the camera look at the player (or another point if desired)
camera.CFrame = CFrame.new(freezePosition, playerPosition)
task.wait(0)
test:Destroy()
task.wait(0)
local fx7 = game.ReplicatedStorage.Resources.FiveSeasonsFX["CharFX"].EyeEmit:Clone()
fx7.Parent = game.Players.LocalPlayer.Character["Right Arm"]
for _, child in ipairs(fx7:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(0, 125, 255)) -- Set color to purple
        child:Emit(6) -- Emit 1 particle
    end
end 
task.wait(1)
local Test = game.ReplicatedStorage.Resources.GrandFissureFinisher.DragonExplode.Part.Main
local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character["HumanoidRootPart"]


for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(0, 125, 255)) -- Set color to purple
        child:Emit(20)
    end
end
task.wait(0)
Players = game:GetService("Players")
 local speaker = Players.LocalPlayer
 workspace.CurrentCamera:remove()
     wait(.1)
     workspace.CurrentCamera.CameraSubject = speaker.Character:FindFirstChildWhichIsA('Humanoid')
     workspace.CurrentCamera.CameraType = "Custom"
     speaker.CameraMinZoomDistance = 0.5
     speaker.CameraMaxZoomDistance = 400
     speaker.CameraMode = "Classic"
     speaker.Character.Head.Anchored = false
    end

end

humanoid.AnimationPlayed:Connect(onAnimationPlayed)

local animationId = 15955393872 ---wall combo 


local player = game.Players.LocalPlayer

local character = player.Character or player.CharacterAdded:Wait()

local humanoid = character:WaitForChild("Humanoid")


local function onAnimationPlayed(animationTrack)

    if animationTrack.Animation.AnimationId == "rbxassetid://" .. animationId then

local p = game.Players.LocalPlayer

local Humanoid = p.Character:WaitForChild("Humanoid")


for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do

    animTrack:Stop()

end


local AnimAnim = Instance.new("Animation")

AnimAnim.AnimationId = "rbxassetid://18897648446"

local Anim = Humanoid:LoadAnimation(AnimAnim)


local startTime = 3.8


Anim:Play()

Anim:AdjustSpeed(0)

Anim.TimePosition = startTime

Anim:AdjustSpeed(1)
local function GetGitSound(GithubSnd,SoundName) --idk what is this for anyway
    local url=GithubSnd
    if not isfile(SoundName..".mp3") then
        writefile(SoundName..".mp3", game:HttpGet(url))
    end
    local sound=Instance.new("Sound")
    sound.SoundId=(getcustomasset or getsynasset)(SoundName..".mp3")
    return sound
end

local Clock = GetGitSound("https://github.com/Kenjihin69/Kenjihin69/blob/main/Screen_Recording_20250121_202931_20250121_203018_20250121_204216_20250121_204307.mp3?raw=true","shinji spin wall combo")

Clock.Parent = workspace

Clock.Volume = 5
Clock.TimePosition = 0

Clock:Play()
task.wait(0.4)
local AnimAnim2 = Instance.new("Animation")

AnimAnim2.AnimationId = "rbxassetid://76530443909428"

local Anim2 = Humanoid:LoadAnimation(AnimAnim2)


local startTime = 0


Anim:Stop()

Anim2:Play()

Anim2:AdjustSpeed(0)

Anim2.TimePosition = startTime

Anim2:AdjustSpeed(3)
local Test = game.ReplicatedStorage.Resources.Sunrise.Constant2.Part.Constant

local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("Torso")

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(0, 125, 255)) -- Set color to purple
        child:Emit(20)
        child.Enabled = true
    end
end
task.wait(1.4)
test:Destroy()

task.wait(0)
local AnimAnim2 = Instance.new("Animation")

AnimAnim2.AnimationId = "rbxassetid://79761806706382"

local Anim2 = Humanoid:LoadAnimation(AnimAnim2)


local startTime = 2


Anim:Stop()

Anim2:Play()

Anim2:AdjustSpeed(0)

Anim2.TimePosition = startTime

Anim2:AdjustSpeed(1.2)
task.wait(0.7)
local Test = game.ReplicatedStorage.Resources.CrushingPull.Stomp.Stomp.Attachment
local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character["Head"]

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
        child:Emit(10)
    end
end
    end

end

humanoid.AnimationPlayed:Connect(onAnimationPlayed)

local animationId = 12983333733 ---3 ult


local player = game.Players.LocalPlayer

local character = player.Character or player.CharacterAdded:Wait()

local humanoid = character:WaitForChild("Humanoid")


local function onAnimationPlayed(animationTrack)

    if animationTrack.Animation.AnimationId == "rbxassetid://" .. animationId then

local p = game.Players.LocalPlayer

local Humanoid = p.Character:WaitForChild("Humanoid")


for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do

    animTrack:Stop()

end


local AnimAnim = Instance.new("Animation")

AnimAnim.AnimationId = "rbxassetid://15962443652"

local Anim = Humanoid:LoadAnimation(AnimAnim)


local startTime = 0


Anim:Play()

Anim:AdjustSpeed(0)

Anim.TimePosition = startTime

Anim:AdjustSpeed(1)
local Test = game.ReplicatedStorage.Resources.LastBreath.Arm.Arm.Attachment
local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("Right Arm")

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(255, 255, 0)) -- Set color to purple
        child:Emit(5)
        child.Enabled = true
    end
end
task.wait(0)
Players = game:GetService("Players")
 local speaker = Players.LocalPlayer
 workspace.CurrentCamera:remove()
     wait(.1)
     workspace.CurrentCamera.CameraSubject = speaker.Character:FindFirstChildWhichIsA('Humanoid')
     workspace.CurrentCamera.CameraType = "Custom"
     speaker.CameraMinZoomDistance = 0.5
     speaker.CameraMaxZoomDistance = 400
     speaker.CameraMode = "Classic"
     speaker.Character.Head.Anchored = false
task.wait(0)
local Players = game:GetService("Players")
local player = Players.LocalPlayer
local humanoid = player.Character.Humanoid
local s = tick()
coroutine.wrap(function()
while tick() - s < 5 do
    humanoid.AutoRotate = true
    wait(0)
end
end)()
task.wait(0)
local function GetGitSound(GithubSnd,SoundName) --idk what is this for anyway
    local url=GithubSnd
    if not isfile(SoundName..".mp3") then
        writefile(SoundName..".mp3", game:HttpGet(url))
    end
    local sound=Instance.new("Sound")
    sound.SoundId=(getcustomasset or getsynasset)(SoundName..".mp3")
    return sound
end

local Clock = GetGitSound("https://github.com/Kenjihin69/Kenjihin69/blob/main/lv_0_20250123153409.mp3?raw=true","shinji this bomb")

Clock.Parent = workspace

Clock.Volume = 6
Clock.TimePosition = 0

Clock:Play()
task.wait(0)
local startTime = tick()  -- Get the current time in seconds Uh yep
local duration = 0.4  -- Duration in sec Heh

local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()

local floatSpeed = 3 -- Adjust speed 
local duration = 1.6 -- Duration in sec :whatthehellbro: 0.1 cuz yes

local humanoidRootPart = character:FindFirstChild("HumanoidRootPart")
if humanoidRootPart then
    local startTime = tick()
    while tick() - startTime < duration do
        wait(0.01) -- Controls how the loop runs googoogaga
        humanoidRootPart.CFrame = humanoidRootPart.CFrame + humanoidRootPart.CFrame.LookVector * floatSpeed * 0.1

    end
end
task.wait(0)
test:Destroy()
task.wait(0)
local AnimAnim2 = Instance.new("Animation")

AnimAnim2.AnimationId = "rbxassetid://18897115785"

local Anim2 = Humanoid:LoadAnimation(AnimAnim2)


local startTime = 0


Anim:Stop()

Anim2:Play()

Anim2:AdjustSpeed(0)

Anim2.TimePosition = startTime

Anim2:AdjustSpeed(1)
local Test = game:GetService("ReplicatedStorage").Resources.Fang.OneInch2.dash3.VFX
local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("HumanoidRootPart")

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
        child:Emit(1)
       child.Color = ColorSequence.new(Color3.fromRGB(0, 125, 255)) -- Set color to purple
child.Enabled = true 
    end
end

task.wait(0)
local startTime = tick()  -- Get the current time in seconds Uh yep
local duration = 2  -- Duration in sec Heh

local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()

local floatSpeed = 100 -- Adjust speed 
local duration = 3 -- Duration in sec :whatthehellbro: 0.1 cuz yes

local humanoidRootPart = character:FindFirstChild("HumanoidRootPart")
if humanoidRootPart then
    local startTime = tick()
    while tick() - startTime < duration do
        wait(0.01) -- Controls how the loop runs googoogaga
        humanoidRootPart.CFrame = humanoidRootPart.CFrame + humanoidRootPart.CFrame.LookVector * floatSpeed * 0.1

    end
end

task.wait(0)
Anim2:Stop()
task.wait(0)
test:Destroy()
task.wait(0)
local AnimAnim2 = Instance.new("Animation")

AnimAnim2.AnimationId = "rbxassetid://140164642047188"

local Anim2 = Humanoid:LoadAnimation(AnimAnim2)


local startTime = 6.8


Anim:Stop()

Anim2:Play()

Anim2:AdjustSpeed(0)

Anim2.TimePosition = startTime

Anim2:AdjustSpeed(1.2)
local Test = game.ReplicatedStorage.Emotes.DemonParticles.RootAttachment

local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("HumanoidRootPart")
test.CFrame = test.CFrame * CFrame.new(0, 0, -4)
for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(255, 255, 0)) -- Set color to purple
        child:Emit(1)
        
    end
end
task.wait(0)
local Test = game:GetService("ReplicatedStorage").Resources.FuneralEffect.Center
local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character["Right Arm"]


for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
        child:Emit(15)
       child.Enabled = true
    end
end

task.wait(1)
test:Destroy()
task.wait(0)
Clock:Stop()  
    end

end

humanoid.AnimationPlayed:Connect(onAnimationPlayed) ----ult

local animationId = 12447707844
local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()
local humanoid = character:WaitForChild("Humanoid")

local function onAnimationPlayed(animationTrack)

if animationTrack.Animation.AnimationId == "rbxassetid://" .. animationId then
        local x = math.random(1, 2)
        if x == 1 then
            local p = game.Players.LocalPlayer
            local Humanoid = p.Character:WaitForChild("Humanoid")
            
            for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do
                animTrack:Stop()
            end
            
            local AnimAnim = Instance.new("Animation")
            AnimAnim.AnimationId = "rbxassetid://15962443652"
            local Anim = Humanoid:LoadAnimation(AnimAnim)
            local startTime = 0
            Anim:Play()
            Anim:AdjustSpeed(0)
            Anim.TimePosition = startTime
            Anim:AdjustSpeed(0)

            Anim:AdjustSpeed(1)
              local function GetGitSound(GithubSnd,SoundName) --idk what is this for anyway
    local url=GithubSnd
    if not isfile(SoundName..".mp3") then
        writefile(SoundName..".mp3", game:HttpGet(url))
    end
    local sound=Instance.new("Sound")
    sound.SoundId=(getcustomasset or getsynasset)(SoundName..".mp3")
    return sound
end

local Clock = GetGitSound("https://github.com/Kenjihin69/Kenjihin69/blob/main/Screen_Recording_20250117_165259_20250117_165434_20250117_193129%20%5Bmusic%5D.mp3?raw=true","shinji song")

Clock.Parent = workspace

Clock.Volume = 5
Clock.TimePosition = 0

Clock:Play()
task.wait(0)
local Test = game.ReplicatedStorage.Resources.CrabSlash.Slam.Part.Attachment

local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("HumanoidRootPart")

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
        child:Emit(5)
    end
end
task.wait(0)
local Test = game.ReplicatedStorage.Resources.SunsetEffects.UpCy.UpCylinder.Attachment
local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("HumanoidRootPart")

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(255, 255, 255)) -- Set color to purple
        child:Emit(10)      
    end
end
task.wait(0)
local Test = game.ReplicatedStorage.Resources.Fissure.DragonExplode.Part.Main

local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("HumanoidRootPart")

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(128, 128, 128)) -- Set color to purple
        child:Emit(15)
    end
end
task.wait(0)
local Test = game.ReplicatedStorage.Resources.SunsetEffects.UpCy.UpCylinder.Attachment
local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("HumanoidRootPart")

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(255, 255, 255)) -- Set color to purple
        child:Emit(20)      
    end
end
local Test = game:GetService("ReplicatedStorage").Resources.Sunblitz.Final.Final.Another
local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character["Head"]


for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
     child.Color = ColorSequence.new(Color3.fromRGB(255, 255, 255))         
        child:Emit(20)
        
    end
end
task.wait(0)
local Test = game.ReplicatedStorage.Emotes.VFX.VfxMods.Boundless.vfx.Smoke.Smoke.floor

local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("HumanoidRootPart")

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
        child:Emit(20)
        
    end
end
task.wait(0)
local Test = game.ReplicatedStorage.Resources.LastBreath.PreCam.Floor.Floor.smoke

local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("HumanoidRootPart")

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
        child:Emit(15)
        
    end
end

task.wait(0)
local startTime = tick()  -- Get the current time in seconds Uh yep
local duration = 2  -- Duration in sec Heh

local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()

local floatSpeed = 3 -- Adjust speed 
local duration = 1.7 -- Duration in sec :whatthehellbro: 0.1 cuz yes

local humanoidRootPart = character:FindFirstChild("HumanoidRootPart")
if humanoidRootPart then
    local startTime = tick()
    while tick() - startTime < duration do
        wait(0.01) -- Controls how the loop runs googoogaga
        humanoidRootPart.CFrame = humanoidRootPart.CFrame + humanoidRootPart.CFrame.LookVector * floatSpeed * 0.1

    end
end
task.wait(0)
local Test = game.ReplicatedStorage.Resources.LastBreath.Arm.Arm.Attachment
local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("Right Arm")

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(255, 255, 0)) -- Set color to purple
        child:Emit(5)
        child.Enabled = true
    end
end

task.wait(0)
local startTime = tick()  -- Get the current time in seconds Uh yep
local duration = 1  -- Duration in sec Heh

local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()

local floatSpeed = 3 -- Adjust speed 
local duration = 1.7 -- Duration in sec :whatthehellbro: 0.1 cuz yes

local humanoidRootPart = character:FindFirstChild("HumanoidRootPart")
if humanoidRootPart then
    local startTime = tick()
    while tick() - startTime < duration do
        wait(0.01) -- Controls how the loop runs googoogaga
        humanoidRootPart.CFrame = humanoidRootPart.CFrame + humanoidRootPart.CFrame.LookVector * floatSpeed * 0.1

    end
end
task.wait(0)
local function GetGitSound(GithubSnd,SoundName) --idk what is this for anyway
    local url=GithubSnd
    if not isfile(SoundName..".mp3") then
        writefile(SoundName..".mp3", game:HttpGet(url))
    end
    local sound=Instance.new("Sound")
    sound.SoundId=(getcustomasset or getsynasset)(SoundName..".mp3")
    return sound
end

local Clock = GetGitSound("https://github.com/Kenjihin69/Kenjihin69/blob/main/Screen_Recording_20250118_145555.mp3?raw=true","shinji kung ku")

Clock.Parent = workspace

Clock.Volume = 2
Clock.TimePosition = 0

Clock:Play()
task.wait(0)
        test:Destroy()
task.wait(0.1)
local AnimAnim2 = Instance.new("Animation")

AnimAnim2.AnimationId = "rbxassetid://16746843881"

local Anim2 = Humanoid:LoadAnimation(AnimAnim2)


local startTime = 0


Anim:Stop()

Anim2:Play()

Anim2:AdjustSpeed(0)

Anim2.TimePosition = startTime

Anim2:AdjustSpeed(1)
local Test = game.ReplicatedStorage.Emotes.Menacing.Player2
local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("Head")

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(0, 125, 255)) -- Set color to purple    
        child:Emit(1)

    end
end
task.wait(0.7)
 local Test = game.ReplicatedStorage.Resources.Dragon.Eye.Attachment

local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("HumanoidRootPart")
test.CFrame = test.CFrame * CFrame.new(7, 1.8, 0)
for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(0, 125, 255)) -- Set color to purple
        child:Emit(1)
        
    end
end
task.wait(0)
 local Test = game.ReplicatedStorage.Resources.Dragon.Eye.Attachment

local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("HumanoidRootPart")
test.CFrame = test.CFrame * CFrame.new(-7, 1.8, 0)
for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(0, 125, 255)) -- Set color to purple
        child:Emit(1)
        
    end
end
task.wait(0)
local Test = game.ReplicatedStorage.Emotes.VFX.VfxMods.Boundless.vfx.Smoke.Smoke.floor

local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("HumanoidRootPart")

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
        child:Emit(20)
        
    end
end
task.wait(0)
local Test = game.ReplicatedStorage.Resources.LastBreath.PreCam.Floor.Floor.smoke

local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("HumanoidRootPart")

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
        child:Emit(15)
        
    end
end
task.wait(0)
local Test = game.ReplicatedStorage.Emotes.BackgroundCrashoutVfx.Background
local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("HumanoidRootPart")

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(0, 125, 255)) -- Set color to purple  
        child:Emit(10)
        
    end
end
task.wait(0)
local player = game.Players.LocalPlayer
local playerGui = player:WaitForChild("PlayerGui")
local s = Instance.new("ScreenGui")
s.Parent = playerGui

local textLabel = Instance.new("TextLabel")
textLabel.Parent = s
textLabel.Position = UDim2.new(0.5, -200, 0.8, -50)
textLabel.Size = UDim2.new(0, 400, 0, 50)
textLabel.TextSize = 27
textLabel.TextColor3 = Color3.fromRGB(255, 255, 0) --text color
textLabel.Font = Enum.Font.Antique -- font here
textLabel.BackgroundTransparency = 1
textLabel.Text = "" -- dont change
textLabel.TextStrokeTransparency = 0
textLabel.TextStrokeColor3 = Color3.fromRGB(0, 0, 0) --stroke color here

local function type(text)
    local index = 1
    while index <= #text do
        textLabel.Text = string.sub(text, 1, index)
        index = index + 1
        wait(0.02)
    end
end

local function f()
    for i = 1, 20 do
        textLabel.TextTransparency = i / 20
        wait(0.01)
    end
end
local function fs()
coroutine.wrap(function()
textLabel.TextStrokeTransparency = 0.1
task.wait(0.1)
textLabel.TextStrokeTransparency = 0.2
task.wait(0.1)
textLabel.TextStrokeTransparency = 0.3
task.wait(0.1)
textLabel.TextStrokeTransparency = 0.4
task.wait(0.1)
textLabel.TextStrokeTransparency = 0.5
task.wait(0.1)
textLabel.TextStrokeTransparency = 0.6
task.wait(0.1)
textLabel.TextStrokeTransparency = 0.7
task.wait(0.1)
textLabel.TextStrokeTransparency = 0.8
task.wait(0.1)
textLabel.TextStrokeTransparency = 0.9
task.wait(0.1)
textLabel.TextStrokeTransparency = 1
end)()
end
coroutine.wrap(function()
    local m = " KUNG FU IT'S MEANT TO KILL!" -- text here
    type(m)
    wait(0)
    fs() -- this for stroke lmao
    f()
end)()
task.wait(2.7)
test:Destroy()
task.wait(0)
Anim2:Stop()
task.wait(0)
loadstring(game:HttpGet('https://raw.githubusercontent.com/kenkenplaygt/kenkenplaygt/refs/heads/main/Ult%20shinji'))()
    elseif x == 2 then
        local p = game.Players.LocalPlayer
            local Humanoid = p.Character:WaitForChild("Humanoid")
            
            for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do
                animTrack:Stop()
            end
            
            local AnimAnim = Instance.new("Animation")
            AnimAnim.AnimationId = "rbxassetid://95000469063288"
            local Anim = Humanoid:LoadAnimation(AnimAnim)
            local startTime = 9.9
            Anim:Play()
            Anim:AdjustSpeed(0)
            Anim.TimePosition = startTime
            Anim:AdjustSpeed(0.5)
local function GetGitSound(GithubSnd,SoundName) --idk what is this for anyway
    local url=GithubSnd
    if not isfile(SoundName..".mp3") then
        writefile(SoundName..".mp3", game:HttpGet(url))
    end
    local sound=Instance.new("Sound")
    sound.SoundId=(getcustomasset or getsynasset)(SoundName..".mp3")
    return sound
end
local Clock = GetGitSound("https://github.com/Kenjihin69/Kenjihin69/blob/main/lv_0_20250111144901.mp3?raw=true","Shinji1")

Clock.Parent = workspace

Clock.Volume = 7
Clock.TimePosition = 0

Clock:Play()
task.wait(0)
local Test = game.StarterPlayer.StarterCharacter.Head.ketsupDrop


local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("Head")

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
        child:Emit(20)
        child.Enabled = true
    end
end
task.wait(1.5)
test:Destroy()
task.wait(0.3)
local Test = game.StarterPlayer.StarterCharacter.Head.ketsupDrop

local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("Head")

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
        child:Emit(15)
        
    end
end
task.wait(0.7)
local AnimAnim2 = Instance.new("Animation")

AnimAnim2.AnimationId = "rbxassetid://107649573628906"

local Anim2 = Humanoid:LoadAnimation(AnimAnim2)


local startTime = 3.5


Anim:Stop()

Anim2:Play()

Anim2:AdjustSpeed(0)

Anim2.TimePosition = startTime

Anim2:AdjustSpeed(0.9)
task.wait(0.7)
 -- Get the player's camera
local player = game.Players.LocalPlayer
local camera = game.Workspace.CurrentCamera

-- Set the camera's CameraType to Scriptable (this "freezes" the camera)
camera.CameraType = Enum.CameraType.Scriptable

-- Get the player's position
local playerPosition = player.Character.HumanoidRootPart.Position

-- Set the camera's position above the player (e.g., 50 units above)
local freezePosition = playerPosition + Vector3.new(-6, 1, -6) -- x, y, z coordinates, y is higher than player's position

-- Set the camera's CFrame (position + orientation)
camera.CFrame = CFrame.new(freezePosition)

-- Optional: Make the camera look at the player (or another point if desired)
camera.CFrame = CFrame.new(freezePosition, playerPosition)
task.wait(0.5)
local Test = game.ReplicatedStorage.Emotes.DemonParticles.RootAttachment
local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("HumanoidRootPart")

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(0, 125, 255)) -- Set color to purple
        child:Emit(1)
    end
end
task.wait(0)
local fx7 = game.ReplicatedStorage.Resources.FiveSeasonsFX["CharFX"].EyeEmit:Clone()
fx7.Parent = game.Players.LocalPlayer.Character["Head"]
for _, child in ipairs(fx7:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(0, 125, 255)) -- Set color to purple
        child:Emit(6) -- Emit 1 particle
    end
end 
local player = game.Players.LocalPlayer
local playerGui = player:WaitForChild("PlayerGui")
local s = Instance.new("ScreenGui")
s.Parent = playerGui

local textLabel = Instance.new("TextLabel")
textLabel.Parent = s
textLabel.Position = UDim2.new(0.5, -200, 0.8, -50)
textLabel.Size = UDim2.new(0, 400, 0, 50)
textLabel.TextSize = 27
textLabel.TextColor3 = Color3.fromRGB(255, 255, 0) --text color
textLabel.Font = Enum.Font.Antique -- font here
textLabel.BackgroundTransparency = 1
textLabel.Text = "" -- dont change
textLabel.TextStrokeTransparency = 0
textLabel.TextStrokeColor3 = Color3.fromRGB(0, 0, 0) --stroke color here

local function type(text)
    local index = 1
    while index <= #text do
        textLabel.Text = string.sub(text, 1, index)
        index = index + 1
        wait(0.02)
    end
end

local function f()
    for i = 1, 20 do
        textLabel.TextTransparency = i / 20
        wait(0.01)
    end
end
local function fs()
coroutine.wrap(function()
textLabel.TextStrokeTransparency = 0.1
task.wait(0.1)
textLabel.TextStrokeTransparency = 0.2
task.wait(0.1)
textLabel.TextStrokeTransparency = 0.3
task.wait(0.1)
textLabel.TextStrokeTransparency = 0.4
task.wait(0.1)
textLabel.TextStrokeTransparency = 0.5
task.wait(0.1)
textLabel.TextStrokeTransparency = 0.6
task.wait(0.1)
textLabel.TextStrokeTransparency = 0.7
task.wait(0.1)
textLabel.TextStrokeTransparency = 0.8
task.wait(0.1)
textLabel.TextStrokeTransparency = 0.9
task.wait(0.1)
textLabel.TextStrokeTransparency = 1
end)()
end
coroutine.wrap(function()
    local m = "DAMN YOU.." -- text here
    type(m)
    wait(0)
    fs() -- this for stroke lmao
    f()
end)()
task.wait(1)
local workspace = game.Workspace
 Players = game:GetService("Players")
 local speaker = Players.LocalPlayer
 workspace.CurrentCamera:remove()
     wait(.1)
     workspace.CurrentCamera.CameraSubject = speaker.Character:FindFirstChildWhichIsA('Humanoid')
     workspace.CurrentCamera.CameraType = "Custom"
     speaker.CameraMinZoomDistance = 0.5
     speaker.CameraMaxZoomDistance = 400
     speaker.CameraMode = "Classic"
     speaker.Character.Head.Anchored = false

task.wait(0.3)
local fx7 = game.ReplicatedStorage.Resources.FiveSeasonsFX["CharFX"].EyeEmit:Clone()
fx7.Parent = game.Players.LocalPlayer.Character["Head"]
for _, child in ipairs(fx7:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(0, 125, 255)) -- Set color to purple
        child:Emit(6) -- Emit 1 particle
    end
end 
 task.wait(0)
loadstring(game:HttpGet('https://raw.githubusercontent.com/kenkenplaygt/kenkenplaygt/refs/heads/main/Ult%20shinji'))()
       end
    end
end
humanoid.AnimationPlayed:Connect(onAnimationPlayed)


local animationId = 10470104242 ---downslam 


local player = game.Players.LocalPlayer

local character = player.Character or player.CharacterAdded:Wait()

local humanoid = character:WaitForChild("Humanoid")


local function onAnimationPlayed(animationTrack)

    if animationTrack.Animation.AnimationId == "rbxassetid://" .. animationId then

local p = game.Players.LocalPlayer

local Humanoid = p.Character:WaitForChild("Humanoid")


for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do

    animTrack:Stop()

end


local AnimAnim = Instance.new("Animation")

AnimAnim.AnimationId = "rbxassetid://18897119503"

local Anim = Humanoid:LoadAnimation(AnimAnim)


local startTime = 0

Anim:Play()

Anim:AdjustSpeed(0)

Anim.TimePosition = startTime

Anim:AdjustSpeed(1.5)


    end

end
humanoid.AnimationPlayed:Connect(onAnimationPlayed)
-- m1s anims with vfxs

local animationId = 10469493270
 
 
local player = game.Players.LocalPlayer
 
local character = player.Character or player.CharacterAdded:Wait()
 
local humanoid = character:WaitForChild("Humanoid")
 
 
local function onAnimationPlayed(animationTrack)
 
    if animationTrack.Animation.AnimationId == "rbxassetid://" .. animationId then
 
 
local p = game.Players.LocalPlayer
 
local Humanoid = p.Character:WaitForChild("Humanoid")
 
 
for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do
 
    animTrack:Stop()
 
end
 
 
local AnimAnim = Instance.new("Animation")
 
AnimAnim.AnimationId = "rbxassetid://17325513870"
 
local Anim = Humanoid:LoadAnimation(AnimAnim)
 
 
local startTime = 0
 
 
Anim:Play()
 
Anim:AdjustSpeed(1)
 
Anim.TimePosition = startTime

Anim:AdjustSpeed(1)
 local Test = game.ReplicatedStorage.Resources.LastBreath.Arm.Arm.Attachment
local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("Right Arm")

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(255, 255, 0)) -- Set color to purple
        child:Emit(5)
        child.Enabled = true
    end
end
task.wait(0.4)
test:Destroy()
    end
 
end
 
humanoid.AnimationPlayed:Connect(onAnimationPlayed) ---m2

local animationId = 10469630950
 
 
local player = game.Players.LocalPlayer
 
local character = player.Character or player.CharacterAdded:Wait()
 
local humanoid = character:WaitForChild("Humanoid")
 
 
local function onAnimationPlayed(animationTrack)
 
    if animationTrack.Animation.AnimationId == "rbxassetid://" .. animationId then
 
 
local p = game.Players.LocalPlayer
 
local Humanoid = p.Character:WaitForChild("Humanoid")
 
 
for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do
 
    animTrack:Stop()
 
end
 
 
local AnimAnim = Instance.new("Animation")
 
AnimAnim.AnimationId = "rbxassetid://13532600125"
 
local Anim = Humanoid:LoadAnimation(AnimAnim)
 
 
local startTime = 0
 
 
Anim:Play()
 
Anim:AdjustSpeed(1)
 
Anim.TimePosition = startTime
 
Anim:AdjustSpeed(1)
 local Test = game.ReplicatedStorage.Resources.LastBreath.Arm.Arm.Attachment
local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("Left Arm")

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(255, 255, 0)) -- Set color to purple
        child:Emit(5)
        child.Enabled = true
    end
end
 task.wait(0.4)
test:Destroy()
    end
 
end
 
 
humanoid.AnimationPlayed:Connect(onAnimationPlayed) ---m3

local animationId = 10469639222
 
 
local player = game.Players.LocalPlayer
 
local character = player.Character or player.CharacterAdded:Wait()
 
local humanoid = character:WaitForChild("Humanoid")
 
 
local function onAnimationPlayed(animationTrack)
 
    if animationTrack.Animation.AnimationId == "rbxassetid://" .. animationId then
 
 
local p = game.Players.LocalPlayer
 
local Humanoid = p.Character:WaitForChild("Humanoid")
 
 
for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do
 
    animTrack:Stop()
 
end
 
 
local AnimAnim = Instance.new("Animation")
 
AnimAnim.AnimationId = "rbxassetid://104895379416342"
 
local Anim = Humanoid:LoadAnimation(AnimAnim)
 
 
local startTime = 0
 
 
Anim:Play()
 
Anim:AdjustSpeed(1)
 
Anim.TimePosition = startTime
 
Anim:AdjustSpeed(1)
task.wait(0.3)
local Test = game.ReplicatedStorage.Resources.LastBreath.Arm.Arm.Attachment
local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("Right Arm")

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(255, 255, 0)) -- Set color to purple
        child:Emit(1)
        
    end
end
task.wait(0)
local Test = game.ReplicatedStorage.Resources.LastBreath.Arm.Arm.Attachment
local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character:WaitForChild("Left Arm")

for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(255, 255, 0)) -- Set color to purple
        child:Emit(1)
        
    end
end
    end
 
end
 
 humanoid.AnimationPlayed:Connect(onAnimationPlayed) ---m4

local animationId = 10469643643
 
 
local player = game.Players.LocalPlayer
 
local character = player.Character or player.CharacterAdded:Wait()
 
local humanoid = character:WaitForChild("Humanoid")
 
 
local function onAnimationPlayed(animationTrack)
 
    if animationTrack.Animation.AnimationId == "rbxassetid://" .. animationId then
 
 
local p = game.Players.LocalPlayer
 
local Humanoid = p.Character:WaitForChild("Humanoid")
 
 
for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do
 
    animTrack:Stop()
 
end
 
 
local AnimAnim = Instance.new("Animation")
 
AnimAnim.AnimationId = "rbxassetid://18181348446"
 
local Anim = Humanoid:LoadAnimation(AnimAnim)
 
 
local startTime = 0

Anim:Play()
 
Anim:AdjustSpeed(1)
 
Anim.TimePosition = startTime
 
Anim:AdjustSpeed(1)
task.wait(0.4)
 local Test = game:GetService("ReplicatedStorage").Resources.FuneralEffect.Center
local test = Test:Clone()
test.Parent = game.Players.LocalPlayer.Character["Left Leg"]


for _, child in ipairs(test:GetChildren()) do
    if child:IsA("ParticleEmitter") then
        child:Emit(10)
    end
end
    end
 
end

humanoid.AnimationPlayed:Connect(onAnimationPlayed)


local Players = game:GetService("Players")

local player = Players.LocalPlayer

local character = player.Character or player.CharacterAdded:Wait()

local humanoid = character:WaitForChild("Humanoid")


local animationIdsToStop = {

    [10469493270] = true,

    [10469630950] = true,

    [10469639222] = true,

    [10469643643] = true,

}


local replacementAnimations = {

    ["10469643643"] = "rbxassetid://17889290569",

    ["10469639222"] = "rbxassetid://17889471098",

    ["10469630950"] = "rbxassetid://17889461810",

    ["10469493270"] = "rbxassetid://17889458563",

}


local queue = {}

local isAnimating = false


local function playReplacementAnimation(animationId)

    if isAnimating then

        table.insert(queue, animationId)

        return

    end

   

    isAnimating = true

    local replacementAnimationId = replacementAnimations[tostring(animationId)]

    if replacementAnimationId then

        local AnimAnim = Instance.new("Animation")

        AnimAnim.AnimationId = replacementAnimationId

        local Anim = humanoid:LoadAnimation(AnimAnim)

        Anim:Play()

       

        Anim.Stopped:Connect(function()

            isAnimating = false

            if #queue > 0 then

                local nextAnimationId = table.remove(queue, 1)

                playReplacementAnimation(nextAnimationId)

            end

        end)

    else

        isAnimating = false

    end

end


local function stopSpecificAnimations()

    for _, track in ipairs(humanoid:GetPlayingAnimationTracks()) do

        local animationId = tonumber(track.Animation.AnimationId:match("%d+"))

        if animationIdsToStop[animationId] then

            track:Stop()

        end

    end

end


local function onAnimationPlayed(animationTrack)

    local animationId = tonumber(animationTrack.Animation.AnimationId:match("%d+"))

    if animationIdsToStop[animationId] then

        stopSpecificAnimations()

        animationTrack:Stop()

       

        local replacementAnimationId = replacementAnimations[tostring(animationId)]

        if replacementAnimationId then

            playReplacementAnimation(animationId)

        end

    end

end

if getgenv().speedtools then
local tool = Instance.new("Tool")
tool.Name = "Light Of Speed"
tool.RequiresHandle = false
tool.ToolTip = "ooh kick yes yes baby"

tool.Parent = game.Players.LocalPlayer.Backpack

local ToolNumber = 1
local cooldownTime = 4
local isCooldownActive = false  -- To prevent activation during cooldown

local player = game.Players.LocalPlayer
local playerGui = player:WaitForChild("PlayerGui")
local hotbar = playerGui:WaitForChild("Hotbar")
local backpack = hotbar:WaitForChild("Backpack")
local localScript = backpack:WaitForChild("LocalScript")
local cooldown = localScript:WaitForChild("Cooldown")
local clonedCooldown

-- Function to execute when the tool is equipped
local function onActivated()
    -- Prevent activation if cooldown is active
    if isCooldownActive then return end
    isCooldownActive = true

    clonedCooldown = cooldown:Clone()
    local hotbarSlot1 = hotbar:WaitForChild("Backpack"):WaitForChild("Hotbar"):WaitForChild(ToolNumber):WaitForChild("Base")
    clonedCooldown.Parent = hotbarSlot1
    clonedCooldown.BackgroundColor3 = Color3.fromRGB(167, 57, 57)

    loadstring(game:HttpGet('https://raw.githubusercontent.com/kenkenplaygt/kenkenplaygt/refs/heads/main/Slide'))()

    local startSize = clonedCooldown.Size
    local endSize = UDim2.new(startSize.X.Scale, startSize.X.Offset, 0, 0)

    spawn(function()
        local startTime = tick()
        local initialSize = clonedCooldown.Size

        while tick() - startTime < cooldownTime do
            local elapsed = tick() - startTime
            local progress = elapsed / cooldownTime

            -- Adjust cooldown size
            local newSize = UDim2.new(
                initialSize.X.Scale,
                initialSize.X.Offset,
                initialSize.Y.Scale * (1 - progress),
                initialSize.Y.Offset * (1 - progress)
            )

            clonedCooldown.Size = newSize
            wait()
        end

        -- End of cooldown
        clonedCooldown.Size = endSize
        clonedCooldown:Destroy()
        isCooldownActive = false  -- Reset cooldown
    end)
end

tool.Equipped:Connect(onActivated)

tool.Parent = game.Players.LocalPlayer.Backpack
end
if getgenv().speedpunch then
local tool = Instance.new("Tool")
tool.Name = "Speed Of Punch"
tool.RequiresHandle = false
tool.ToolTip = "ooh kick yes yes baby"

tool.Parent = game.Players.LocalPlayer.Backpack

local ToolNumber = 1
local cooldownTime = 4
local isCooldownActive = false  -- To prevent activation during cooldown

local player = game.Players.LocalPlayer
local playerGui = player:WaitForChild("PlayerGui")
local hotbar = playerGui:WaitForChild("Hotbar")
local backpack = hotbar:WaitForChild("Backpack")
local localScript = backpack:WaitForChild("LocalScript")
local cooldown = localScript:WaitForChild("Cooldown")
local clonedCooldown

-- Function to execute when the tool is equipped
local function onActivated()
    -- Prevent activation if cooldown is active
    if isCooldownActive then return end
    isCooldownActive = true

    clonedCooldown = cooldown:Clone()
    local hotbarSlot1 = hotbar:WaitForChild("Backpack"):WaitForChild("Hotbar"):WaitForChild(ToolNumber):WaitForChild("Base")
    clonedCooldown.Parent = hotbarSlot1
    clonedCooldown.BackgroundColor3 = Color3.fromRGB(167, 57, 57)

    loadstring(game:HttpGet('https://raw.githubusercontent.com/kenkenplaygt/kenkenplaygt/refs/heads/main/Mek'))()

    local startSize = clonedCooldown.Size
    local endSize = UDim2.new(startSize.X.Scale, startSize.X.Offset, 0, 0)

    spawn(function()
        local startTime = tick()
        local initialSize = clonedCooldown.Size

        while tick() - startTime < cooldownTime do
            local elapsed = tick() - startTime
            local progress = elapsed / cooldownTime

            -- Adjust cooldown size
            local newSize = UDim2.new(
                initialSize.X.Scale,
                initialSize.X.Offset,
                initialSize.Y.Scale * (1 - progress),
                initialSize.Y.Offset * (1 - progress)
            )

            clonedCooldown.Size = newSize
            wait()
        end

        -- End of cooldown
        clonedCooldown.Size = endSize
        clonedCooldown:Destroy()
        isCooldownActive = false  -- Reset cooldown
    end)
end

tool.Equipped:Connect(onActivated)

tool.Parent = game.Players.LocalPlayer.Backpack
end
local tool = Instance.new("Tool")
tool.Name = "dance"
tool.RequiresHandle = false
tool.ToolTip = "ooh kick yes yes baby"

tool.Parent = game.Players.LocalPlayer.Backpack

local ToolNumber = 1
local cooldownTime = 4
local isCooldownActive = false  -- To prevent activation during cooldown

local player = game.Players.LocalPlayer
local playerGui = player:WaitForChild("PlayerGui")
local hotbar = playerGui:WaitForChild("Hotbar")
local backpack = hotbar:WaitForChild("Backpack")
local localScript = backpack:WaitForChild("LocalScript")
local cooldown = localScript:WaitForChild("Cooldown")
local clonedCooldown

-- Function to execute when the tool is equipped
local function onActivated()
    -- Prevent activation if cooldown is active
    if isCooldownActive then return end
    isCooldownActive = true

    clonedCooldown = cooldown:Clone()
    local hotbarSlot1 = hotbar:WaitForChild("Backpack"):WaitForChild("Hotbar"):WaitForChild(ToolNumber):WaitForChild("Base")
    clonedCooldown.Parent = hotbarSlot1
    clonedCooldown.BackgroundColor3 = Color3.fromRGB(167, 57, 57)

    loadstring(game:HttpGet('https://raw.githubusercontent.com/kenkenplaygt/kenkenplaygt/refs/heads/main/Baby%20ok'))()

    local startSize = clonedCooldown.Size
    local endSize = UDim2.new(startSize.X.Scale, startSize.X.Offset, 0, 0)

    spawn(function()
        local startTime = tick()
        local initialSize = clonedCooldown.Size

        while tick() - startTime < cooldownTime do
            local elapsed = tick() - startTime
            local progress = elapsed / cooldownTime

            -- Adjust cooldown size
            local newSize = UDim2.new(
                initialSize.X.Scale,
                initialSize.X.Offset,
                initialSize.Y.Scale * (1 - progress),
                initialSize.Y.Offset * (1 - progress)
            )

            clonedCooldown.Size = newSize
            wait()
        end

        -- End of cooldown
        clonedCooldown.Size = endSize
        clonedCooldown:Destroy()
        isCooldownActive = false  -- Reset cooldown
    end)
end

tool.Equipped:Connect(onActivated)

tool.Parent = game.Players.LocalPlayer.Backpack

-- sgui
local sG = Instance.new("ScreenGui")
sG.Name = "UIContainer"
sG.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")

-- txlabel
local tL = Instance.new("TextLabel")
tL.Size = UDim2.new(1, 0, 0, 15) -- smaller size
tL.Position = UDim2.new(0, 0, 0, 0) -- Top
tL.BackgroundTransparency = 1 -- by
tL.Text = "Shinji create by tp exploit  and Golden head" -- Updated text
tL.TextColor3 = Color3.new(1, 1, 1) -- clr
tL.Font = Enum.Font.Arcade 
tL.TextScaled = true -- scale
tL.TextTransparency = 0.6 -- opaque
tL.Parent = sG
