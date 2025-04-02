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
    imageLabel.ImageColor3 = Color3.fromRGB(0, 255, 255) -- Dark red

    -- Smooth transition from dark red to none
    tweenColor(imageLabel, Color3.fromRGB(0, 255, 255), Color3.fromRGB(127, 255, 212), 2)
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


ToolName.Text = "Soul Barrage"


local player = game.Players.LocalPlayer

local playerGui = player.PlayerGui

local hotbar = playerGui:FindFirstChild("Hotbar")

local backpack = hotbar:FindFirstChild("Backpack")

local hotbarFrame = backpack:FindFirstChild("Hotbar")

local baseButton = hotbarFrame:FindFirstChild("2").Base

local ToolName = baseButton.ToolName


ToolName.Text = "Shrine Slam"


local player = game.Players.LocalPlayer

local playerGui = player.PlayerGui

local hotbar = playerGui:FindFirstChild("Hotbar")

local backpack = hotbar:FindFirstChild("Backpack")

local hotbarFrame = backpack:FindFirstChild("Hotbar")

local baseButton = hotbarFrame:FindFirstChild("3").Base

local ToolName = baseButton.ToolName


ToolName.Text = "Blood Swipe"


local player = game.Players.LocalPlayer

local playerGui = player.PlayerGui

local hotbar = playerGui:FindFirstChild("Hotbar")

local backpack = hotbar:FindFirstChild("Backpack")

local hotbarFrame = backpack:FindFirstChild("Hotbar")

local baseButton = hotbarFrame:FindFirstChild("4").Base

local ToolName = baseButton.ToolName


ToolName.Text = "Dismantle Counter"


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

                textLabel.Text = "MHB SUCK"

            end

        end

    end

end


playerGui.DescendantAdded:Connect(findGuiAndSetText)

findGuiAndSetText()


local animationId = 12273188754


local player = game.Players.LocalPlayer

local character = player.Character or player.CharacterAdded:Wait()

local humanoid = character:WaitForChild("Humanoid")


local function onAnimationPlayed(animationTrack)

    if animationTrack.Animation.AnimationId == "rbxassetid://" .. animationId then


local p = game.Players.LocalPlayer

local Humanoid = p.Character:WaitForChild("Humanoid")


for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do

    animTrack:Stop()
local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()
end


local AnimAnim = Instance.new("Animation")

AnimAnim.AnimationId = "rbxassetid://18897695481"

local Anim = Humanoid:LoadAnimation(AnimAnim)


local startTime = 0


Anim:Play()

Anim:AdjustSpeed(0)

Anim.TimePosition = startTime

Anim:AdjustSpeed(1.4)

task.wait(1.5)

local AnimAnim2 = Instance.new("Animation")

AnimAnim2.AnimationId = "rbxassetid://18249294373"

local Anim2 = Humanoid:LoadAnimation(AnimAnim2)


local startTime = 0


Anim:Stop()

Anim2:Play()

Anim2:AdjustSpeed(0)

Anim2.TimePosition = startTime

Anim2:AdjustSpeed(1.3)
local final1 = game.ReplicatedStorage.Resources.KJEffects["KJWallCombo"].FinalImpact.Attachment:Clone()
final1.Parent = game.Players.LocalPlayer.Character["Head"]
for _, child in ipairs(final1:GetChildren()) do
    if child:IsA("ParticleEmitter") then -- Check if the child is a ParticleEmitter
        child:Emit(10) -- Emit 20 particles
    end
end
task.wait(0.1)
local hit1 = game.ReplicatedStorage.Resources.KJEffects["lastkick"].Attachment:Clone()
hit1.Parent = game.Players.LocalPlayer.Character["HumanoidRootPart"]
    for _, child in ipairs(hit1:GetChildren()) do
        if child:IsA("ParticleEmitter") then -- Check if the child is a ParticleEmitter
            child:Emit(3) -- Emit 20 particles
        end
    end
task.wait(0.1)
loadstring(game:HttpGet('https://pastebin.com/raw/drMCu0ru'))()
    end

end



humanoid.AnimationPlayed:Connect(onAnimationPlayed)


local animationId = 12296113986


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

AnimAnim.AnimationId = "rbxassetid://16699717165"

local Anim = Humanoid:LoadAnimation(AnimAnim)


local startTime = 4


Anim:Play()

Anim:AdjustSpeed(0)

Anim.TimePosition = startTime

Anim:AdjustSpeed(0.3)
local boom1 = game.ReplicatedStorage.Resources.KJEffects["ImpactEffect2"].Attachment:Clone()
boom1.Parent = game.Players.LocalPlayer.Character["Right Arm"]
    for _, child in ipairs(boom1:GetChildren()) do
        if child:IsA("ParticleEmitter") then -- Check if the child is a ParticleEmitter
child.Color = ColorSequence.new(Color3.fromRGB(255, 255, 237)) -- Set color to green
            child:Emit(20) -- Emit 20 particles
        end
    end
task.wait(0.1)
local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()

local function anchorCharacter()
    character.HumanoidRootPart.Anchored = true
    wait(1.2) -- Wait
    character.HumanoidRootPart.Anchored = false
end

--ass function
anchorCharacter()

task.wait(0.1)

local AnimAnim2 = Instance.new("Animation")

AnimAnim2.AnimationId = "rbxassetid://16311141574"

local Anim2 = Humanoid:LoadAnimation(AnimAnim2)


local startTime = 2


Anim:Stop()

Anim2:Play()

Anim2:AdjustSpeed(0)

Anim2.TimePosition = startTime

Anim2:AdjustSpeed(1)
task.wait(0.4)
local flash = Game.ReplicatedStorage.Resources.KJEffects.DropkickExtra["firstHit"].Attachment:Clone()
flash.Parent = game.Players.LocalPlayer.Character["Left Arm"]
for _, child in ipairs(flash:GetChildren()) do
    if child:IsA("ParticleEmitter") then
        child:Emit(4) -- Emit 1 particle
    end
end

task.wait(0.1)
loadstring(game:HttpGet('https://pastebin.com/raw/drMCu0ru'))()
    end

end


humanoid.AnimationPlayed:Connect(onAnimationPlayed)


local animationId = 12309835105


local player = game.Players.LocalPlayer

local character = player.Character or player.CharacterAdded:Wait()

local humanoid = character:WaitForChild("Humanoid")


local function onAnimationPlayed(animationTrack)

    if animationTrack.Animation.AnimationId == "rbxassetid://" .. animationId then


local p = game.Players.LocalPlayer

local Humanoid = p.Character:WaitForChild("Humanoid")


for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do

    animTrack:Stop()
local fx7 = Game.ReplicatedStorage.Resources.CrabBeam["Blaswwwt"].dashpunch.Attachment:Clone()
fx7.Parent = game.Players.LocalPlayer.Character["Torso"]
for _, child in ipairs(fx7:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(255, 0, 0)) -- Set color to stuff
        child:Emit(1) -- Emit STUFF particle
    end
end
end


local AnimAnim = Instance.new("Animation")

AnimAnim.AnimationId = "rbxassetid://13532562418"

local Anim = Humanoid:LoadAnimation(AnimAnim)


local startTime = 0


Anim:Play()

Anim:AdjustSpeed(0)

Anim.TimePosition = startTime

Anim:AdjustSpeed(0.5)

task.wait(0.6)

local AnimAnim2 = Instance.new("Animation")

AnimAnim2.AnimationId = "rbxassetid://18249294373"

local Anim2 = Humanoid:LoadAnimation(AnimAnim2)


local startTime = 0


Anim:Stop()

Anim2:Play()

Anim2:AdjustSpeed(0)

Anim2.TimePosition = startTime

Anim2:AdjustSpeed(1)

-- Aqua color sequence (cyan and light blue)
local aqua = ColorSequence.new{
    ColorSequenceKeypoint.new(0, Color3.fromRGB(0, 255, 255)), -- cyan
    ColorSequenceKeypoint.new(1, Color3.fromRGB(127, 255, 212)) -- light aqua
}

local fx5 = game.ReplicatedStorage.Resources.FiveSeasonsFX["CharFX"].ArmBurst.Attachment:Clone()
fx5.Parent = game.Players.LocalPlayer.Character["Right Arm"]
for _, child in ipairs(fx5:GetChildren()) do
    if child:IsA("ParticleEmitter") then
        child.Color = aqua -- Change particle color to aqua
        child:Emit(6) -- Emit 20 particles
    end
end

task.wait(0.1)

local fx7 = game.ReplicatedStorage.Resources.FiveSeasonsFX["CharFX"].ArmFX:Clone()
fx7.Parent = game.Players.LocalPlayer.Character["Right Arm"]
for _, child in ipairs(fx7:GetChildren()) do
    if child:IsA("ParticleEmitter") then
        child.Color = aqua -- Change particle color to aqua
        child:Emit(1) -- Emit 1 particle
    end
end
wait(1.4)
        fx7:Destroy()

task.wait(0.1)
loadstring(game:HttpGet('https://pastebin.com/raw/drMCu0ru'))()

    end

end


humanoid.AnimationPlayed:Connect(onAnimationPlayed)


local animationId = 13603396939 --- counter 


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

AnimAnim.AnimationId = "rbxassetid://16311141574"

local Anim = Humanoid:LoadAnimation(AnimAnim)


local startTime = 0.2


Anim:Play()

Anim:AdjustSpeed(0)

Anim.TimePosition = startTime

Anim:AdjustSpeed(0.9)
local final1 = game.ReplicatedStorage.Resources.Meteor["ExploVar1"].Part.Attachment:Clone()
        final1.Parent = game.Players.LocalPlayer.Character["Torso"]
        for _, child in ipairs(final1:GetChildren()) do
            if child:IsA("ParticleEmitter") then -- Check if the child is a ParticleEmitter
child.Color = ColorSequence.new(Color3.fromRGB(255, 255, 237)) -- Set color to green
                child:Emit(2) -- Emit 20 particles
            end
        end
task.wait(1.4)
local boom1 = game.ReplicatedStorage.Resources.KJEffects["ImpactEffect2"].Attachment:Clone()
boom1.Parent = game.Players.LocalPlayer.Character["Right Arm"]
    for _, child in ipairs(boom1:GetChildren()) do
        if child:IsA("ParticleEmitter") then -- Check if the child is a ParticleEmitter
child.Color = ColorSequence.new(Color3.fromRGB(255, 255, 237)) -- Set color to green
            child:Emit(4) -- Emit 20 particles
        end
    end
task.wait(0.7)
local fx7 = Game.ReplicatedStorage.Resources.CrabBeam["Blaswwwt"].dashpunch.Attachment:Clone()
fx7.Parent = game.Players.LocalPlayer.Character["Torso"]
for _, child in ipairs(fx7:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = ColorSequence.new(Color3.fromRGB(255, 255, 237)) -- Set color to green
        child:Emit(8) -- Emit STUFF particle
    end
end
    end

end

humanoid.AnimationPlayed:Connect(onAnimationPlayed)

local animationId = 12460977270 --ult one


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

AnimAnim.AnimationId = "rbxassetid://15090141089"

local Anim = Humanoid:LoadAnimation(AnimAnim)


local startTime = 0

Anim:Play()

Anim:AdjustSpeed(0)

Anim.TimePosition = startTime

Anim:AdjustSpeed(6)

task.wait(1.4)

local AnimAnim2 = Instance.new("Animation")

AnimAnim2.AnimationId = "rbxassetid://18897119503"

local Anim2 = Humanoid:LoadAnimation(AnimAnim2)


local startTime = 0.3


Anim:Stop()

Anim2:Play()

Anim2:AdjustSpeed(0)

Anim2.TimePosition = startTime

Anim2:AdjustSpeed(1.2)
local flash = Game.ReplicatedStorage.Resources.KJEffects.DropkickExtra["firstHit"].Attachment:Clone()
flash.Parent = game.Players.LocalPlayer.Character["Right Leg"]
for _, child in ipairs(flash:GetChildren()) do
    if child:IsA("ParticleEmitter") then
        child:Emit(7) -- Emit 1 particle
    end
end
task.wait(0.1)
-- Aqua color sequence (cyan and light blue)
local aqua = ColorSequence.new{
    ColorSequenceKeypoint.new(0, Color3.fromRGB(0, 255, 255)), -- cyan
    ColorSequenceKeypoint.new(1, Color3.fromRGB(127, 255, 212)) -- light aqua
}

local wow1 = game.ReplicatedStorage.Resources.Dragon["Complete"].Part.Debri:Clone()
wow1.Parent = game.Players.LocalPlayer.Character["Torso"]
    for _, child in ipairs(wow1:GetChildren()) do
        if child:IsA("ParticleEmitter") then 
child.Color = aqua -- Change particle color to aqua
           child:Emit(6) -- Emit 20 particles
        end
    end
    end

end

humanoid.AnimationPlayed:Connect(onAnimationPlayed)

local animationId = 16310343179 ---wall combo 


local player = game.Players.LocalPlayer

local character = player.Character or player.CharacterAdded:Wait()

local humanoid = character:WaitForChild("Humanoid")


local function onAnimationPlayed(animationTrack)

    if animationTrack.Animation.AnimationId == "rbxassetid://" .. animationId then

local p = game.Players.LocalPlayer

local Humanoid = p.Character:WaitForChild("Humanoid")


for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do

    animTrack:Stop()
local red4 = game.ReplicatedStorage.Resources.FiveSeasonsFX["CharFX"].EyeEmit:Clone()
red4.Parent = game.Players.LocalPlayer.Character["Head"]
    for _, child in ipairs(red4:GetChildren()) do
        if child:IsA("ParticleEmitter") then -- Check if the child is a 
            child:Emit(20) -- Emit 20 particles
        end
    end
end


local AnimAnim = Instance.new("Animation")

AnimAnim.AnimationId = "rbxassetid://16062712948"

local Anim = Humanoid:LoadAnimation(AnimAnim)


local startTime = 0.6


Anim:Play()

Anim:AdjustSpeed(0)

Anim.TimePosition = startTime

Anim:AdjustSpeed(1.7)

task.wait(1.8)

local AnimAnim2 = Instance.new("Animation")

AnimAnim2.AnimationId = "rbxassetid://18249294373"

local Anim2 = Humanoid:LoadAnimation(AnimAnim2)


local startTime = 0


Anim:Stop()

Anim2:Play()

Anim2:AdjustSpeed(0)

Anim2.TimePosition = startTime

Anim2:AdjustSpeed(1)
task.wait(0.4)
-- Aqua color sequence (cyan and light blue)
local aqua = ColorSequence.new{
    ColorSequenceKeypoint.new(0, Color3.fromRGB(0, 255, 255)), -- cyan
    ColorSequenceKeypoint.new(1, Color3.fromRGB(127, 255, 212)) -- light aqua
}

local fx5 = game.ReplicatedStorage.Resources.FiveSeasonsFX["CharFX"].ArmBurst.Attachment:Clone()
fx5.Parent = game.Players.LocalPlayer.Character["Right Arm"]
for _, child in ipairs(fx5:GetChildren()) do
    if child:IsA("ParticleEmitter") then
        child.Color = aqua -- Change particle color to aqua
        child:Emit(20) -- Emit 20 particles
    end
end
task.wait(0.1)
loadstring(game:HttpGet('https://raw.githubusercontent.com/Kenjihin69/Kenjihin69/refs/heads/main/Yujihit'))()

task.wait(0.1)
local fine3 = game.ReplicatedStorage.Resources.KJEffects["fine...Emit"].EmitBatch2:Clone()
fine3.Parent = game.Players.LocalPlayer.Character["Right Arm"]
    for _, child in ipairs(fine3:GetChildren()) do
        if child:IsA("ParticleEmitter") then -- Check if the child is a ParticleEmitter
            child:Emit(1) -- Emit 20 particles
        end
    end
task.wait(0.1)
local soundeffect = Instance.new("Sound")
soundeffect.SoundId = "rbxassetid://18443813318"
soundeffect.Parent = game.Players.LocalPlayer.Character.Torso
soundeffect:Play()
soundeffect.Volume = 3
    end

end

humanoid.AnimationPlayed:Connect(onAnimationPlayed)

local animationId = 14057231976 ---ult move 3


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

AnimAnim.AnimationId = "rbxassetid://18896127525"

local Anim = Humanoid:LoadAnimation(AnimAnim)


local startTime = 0


Anim:Play()

Anim:AdjustSpeed(0)

Anim.TimePosition = startTime

Anim:AdjustSpeed(1)
task.wait(0.6)
local fx5 = game.ReplicatedStorage.Resources.FiveSeasonsFX["CharFX"].ArmBurst.Attachment:Clone()
fx5.Parent = game.Players.LocalPlayer.Character["Right Arm"]
for _, child in ipairs(fx5:GetChildren()) do
    if child:IsA("ParticleEmitter") then
        child:Emit(7) -- Emit 20 particles
    end
end

 task.wait(0.5)
local fx5 = game.ReplicatedStorage.Resources.FiveSeasonsFX["CharFX"].ArmBurst.Attachment:Clone()
fx5.Parent = game.Players.LocalPlayer.Character["Right Arm"]
for _, child in ipairs(fx5:GetChildren()) do
    if child:IsA("ParticleEmitter") then
        child:Emit(15) -- Emit 20 particles
    end
end

task.wait(0.1)
loadstring(game:HttpGet('https://raw.githubusercontent.com/Kenjihin69/Kenjihin69/refs/heads/main/Yujihit'))()

task.wait(0.1)
local flash = Game.ReplicatedStorage.Resources.KJEffects.DropkickExtra["firstHit"].Attachment:Clone()
flash.Parent = game.Players.LocalPlayer.Character["Right Arm"]
for _, child in ipairs(flash:GetChildren()) do
    if child:IsA("ParticleEmitter") then
        child:Emit(6) -- Emit 1 particle
    end
end
task.wait(0.1)
local hit1 = game.ReplicatedStorage.Resources.KJEffects["lastkick"].Attachment:Clone()
hit1.Parent = game.Players.LocalPlayer.Character["HumanoidRootPart"]
    for _, child in ipairs(hit1:GetChildren()) do
        if child:IsA("ParticleEmitter") then -- Check if the child is a ParticleEmitter
            child:Emit(5) -- Emit 20 particles
        end
    end

task.wait(0.1)
local soundeffect = Instance.new("Sound")
soundeffect.SoundId = "rbxassetid://18443813318"
soundeffect.Parent = game.Players.LocalPlayer.Character.Torso
soundeffect:Play()
soundeffect.Volume = 5

task.wait(0.1)
loadstring(game:HttpGet('https://pastebin.com/raw/NAZhXT91'))()

    end
end
humanoid.AnimationPlayed:Connect(onAnimationPlayed)

local animationId = 12467789963 ---ult move 2 final hunt


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

AnimAnim.AnimationId = "rbxassetid://18896127525"

local Anim = Humanoid:LoadAnimation(AnimAnim)


local startTime = 0


Anim:Play()

Anim:AdjustSpeed(0)

Anim.TimePosition = startTime

Anim:AdjustSpeed(1.2)
task.wait(0.8)
loadstring(game:HttpGet('https://raw.githubusercontent.com/Kenjihin69/Kenjihin69/refs/heads/main/Nuke%20black%20flash'))()

task.wait(0.1)
-- Aqua color sequence (cyan and light blue)
local aqua = ColorSequence.new{
    ColorSequenceKeypoint.new(0, Color3.fromRGB(0, 255, 255)), -- cyan
    ColorSequenceKeypoint.new(1, Color3.fromRGB(127, 255, 212)) -- light aqua
}

local fx7 = Game.ReplicatedStorage.Resources.CrabBeam["Blaswwwt"].dashpunch.Attachment:Clone()
fx7.Parent = game.Players.LocalPlayer.Character["Torso"]
for _, child in ipairs(fx7:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = aqua -- Change particle color to aqua
        child:Emit(14) -- Emit STUFF particle
    end
end
task.wait(0.1)
loadstring(game:HttpGet('https://pastebin.com/raw/NAZhXT91'))()
    end
end
humanoid.AnimationPlayed:Connect(onAnimationPlayed)


local animationId = 13813099821 ---4 move ult not miss


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

AnimAnim.AnimationId = "rbxassetid://13813099821"

local Anim = Humanoid:LoadAnimation(AnimAnim)


local startTime = 0

Anim:Play()

Anim:AdjustSpeed(0)

Anim.TimePosition = startTime

Anim:AdjustSpeed(1)
-- Aqua color sequence (cyan and light blue)
local aqua = ColorSequence.new{
    ColorSequenceKeypoint.new(0, Color3.fromRGB(0, 255, 255)), -- cyan
    ColorSequenceKeypoint.new(1, Color3.fromRGB(127, 255, 212)) -- light aqua
}

local fx7 = Game.ReplicatedStorage.Resources.CrabBeam["Blaswwwt"].dashpunch.Attachment:Clone()
fx7.Parent = game.Players.LocalPlayer.Character["Torso"]
for _, child in ipairs(fx7:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = aqua -- Change particle color to aqua
        child:Emit(4) -- Emit STUFF particle
    end
end
task.wait(0.1)
local launch1 = game.ReplicatedStorage.Resources.KJEffects["launchup"].launchything:Clone()
            launch1.Parent = game.Players.LocalPlayer.Character["Torso"]
                for _, child in ipairs(launch1:GetChildren()) do
                    if child:IsA("ParticleEmitter") then -- Check if the child is a ParticleEmitter
                        child:Emit(3) -- Emit 20 particles
                    end
                end
task.wait(0.1)
loadstring(game:HttpGet('https://pastebin.com/raw/NAZhXT91'))()
    end

end
humanoid.AnimationPlayed:Connect(onAnimationPlayed) --ult
 
local animationId = 12342141464
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
            AnimAnim.AnimationId = "rbxassetid://13643152947"
            local Anim = Humanoid:LoadAnimation(AnimAnim)
            local startTime = 0
            Anim:Play()
            Anim:AdjustSpeed(0)
            Anim.TimePosition = startTime
            Anim:AdjustSpeed(1)
 
            Anim:AdjustSpeed(1)
local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()
local humanoid = character:WaitForChild("Humanoid")
local humanoidRootPart = character:WaitForChild("HumanoidRootPart")
local camera = workspace.CurrentCamera  -- Reference to the camera


local dashSpeed = 100
local dashDuration = 3.2
local isDashing = false


local dashAnim = Instance.new("Animation")
dashAnim.AnimationId = "rbxassetid://0"
local animTrack = humanoid:LoadAnimation(dashAnim)
 

local function moveForward()
    if isDashing then return end
    isDashing = true

    wait(0.1)


    local bodyVelocity = Instance.new("BodyVelocity")
    bodyVelocity.MaxForce = Vector3.new(100000, 100000, 100000)  -- Max force to apply the movement
    bodyVelocity.Parent = humanoidRootPart

    local dashEndTime = tick() + dashDuration  -- Time when dash should end

    while tick() < dashEndTime do
       
        local cameraDirection = camera.CFrame.LookVector
        local dashDirection = Vector3.new(cameraDirection.X, 0, cameraDirection.Z).unit

        bodyVelocity.Velocity = dashDirection * dashSpeed

        wait(0.05)  
    end

 
    animTrack:Stop()

  
    bodyVelocity:Destroy()
    isDashing = false
end


moveForward()  

task.wait(0.1)
 
local AnimAnim2 = Instance.new("Animation")
 
AnimAnim2.AnimationId = "rbxassetid://18435303746"
 
local Anim2 = Humanoid:LoadAnimation(AnimAnim2)
 
 
local startTime = 2.7
 
 
Anim:Stop()
 
Anim2:Play()
 
Anim2:AdjustSpeed(0)
 
Anim2.TimePosition = startTime

Anim2:AdjustSpeed(1) 
task.wait(0.1)
-- Aqua color sequence (cyan and light blue)
local aqua = ColorSequence.new{
    ColorSequenceKeypoint.new(0, Color3.fromRGB(0, 255, 255)), -- cyan
    ColorSequenceKeypoint.new(1, Color3.fromRGB(127, 255, 212)) -- light aqua
}

local red4_2 = game.ReplicatedStorage.Resources.StoicBomb["Stage1"].Floor.Attachment:Clone()
red4_2.Parent = game.Players.LocalPlayer.Character["Left Leg"]
for _, child in ipairs(red4_2:GetChildren()) do
    if child:IsA("ParticleEmitter") then
child.Color = aqua -- Change particle color to aqua
        child:Emit(40)
    end
end
task.wait(0.1)
loadstring(game:HttpGet('https://raw.githubusercontent.com/Kenjihin69/Kenjihin69/refs/heads/main/Yujihit'))()
wait(2)
        red4_2:Destroy()

     task.wait(1)      
    elseif x == 2 then
        local p = game.Players.LocalPlayer
            local Humanoid = p.Character:WaitForChild("Humanoid")
 
            for _, animTrack in pairs(Humanoid:GetPlayingAnimationTracks()) do
                animTrack:Stop()
loadstring(game:HttpGet('https://raw.githubusercontent.com/Kenjihin69/Kenjihin69/refs/heads/main/Cutscenes%20make'))()

            end
 
            local AnimAnim = Instance.new("Animation")
            AnimAnim.AnimationId = "rbxassetid://15962326593"
            local Anim = Humanoid:LoadAnimation(AnimAnim)
            local startTime = 0
            Anim:Play()
            Anim:AdjustSpeed(0)
            Anim.TimePosition = startTime
            Anim:AdjustSpeed(1)
 local startTime = tick()  -- Get the current time in seconds Uh yep
local duration = 2  -- Duration in sec Heh

local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()

local floatSpeed = 5 -- Adjust speed fuck you nigga length you want
local duration = 3 -- Duration in sec :whatthehellbro: 0.1 cuz yes

local humanoidRootPart = character:FindFirstChild("HumanoidRootPart")
if humanoidRootPart then
    local startTime = tick()
    while tick() - startTime < duration do
        wait(0.01) -- Controls how the loop runs googoogaga
        humanoidRootPart.CFrame = humanoidRootPart.CFrame + humanoidRootPart.CFrame.LookVector * floatSpeed * 0.1

    end
end

task.wait(0.4)          
          local AnimAnim2 = Instance.new("Animation")
 
AnimAnim2.AnimationId = "rbxassetid://15957376722"
 
local Anim2 = Humanoid:LoadAnimation(AnimAnim2)
 
 
local startTime = 0
 
 
Anim:Stop()
 
Anim2:Play()
 
Anim2:AdjustSpeed(0)
 
Anim2.TimePosition = startTime
 
Anim2:AdjustSpeed(0.8)
local red4 = game.ReplicatedStorage.Resources.FiveSeasonsFX["CharFX"].EyeEmit:Clone()
red4.Parent = game.Players.LocalPlayer.Character["Head"]
    for _, child in ipairs(red4:GetChildren()) do
        if child:IsA("ParticleEmitter") then -- Check if the child is a 
            child:Emit(20) -- Emit 20 particles
        end
    end
task.wait(1)
loadstring(game:HttpGet('https://raw.githubusercontent.com/Kenjihin69/Kenjihin69/refs/heads/main/Yujihit'))()
       end
    end
end

humanoid.AnimationPlayed:Connect(onAnimationPlayed)


local animationId = 10479335397 ---dash


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

AnimAnim.AnimationId = "rbxassetid://17838006839"

local Anim = Humanoid:LoadAnimation(AnimAnim)


local startTime = 0


Anim:Play()

Anim:AdjustSpeed(0)

Anim.TimePosition = startTime

Anim:AdjustSpeed(1.1)

delay(1.2, function()
 
    Anim:Stop()
 
end)
local hit1 = game.ReplicatedStorage.Resources.KJEffects["lastkick"].Attachment:Clone()
hit1.Parent = game.Players.LocalPlayer.Character["HumanoidRootPart"]
    for _, child in ipairs(hit1:GetChildren()) do
        if child:IsA("ParticleEmitter") then -- Check if the child is a ParticleEmitter
            child:Emit(7) -- Emit 20 particles
        end
    end
    end

end

humanoid.AnimationPlayed:Connect(onAnimationPlayed)


local animationId = 10503381238 --up cut


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

AnimAnim.AnimationId = "rbxassetid://14900168720"

local Anim = Humanoid:LoadAnimation(AnimAnim)


local startTime = 1.3


Anim:Play()

Anim:AdjustSpeed(0)

Anim.TimePosition = startTime

Anim:AdjustSpeed(1.4)


    end

end

humanoid.AnimationPlayed:Connect(onAnimationPlayed)


local animationId = 10470104242 ---down slam


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

AnimAnim.AnimationId = "rbxassetid://17858878027"

local Anim = Humanoid:LoadAnimation(AnimAnim)


local startTime = 0

Anim:Play()

Anim:AdjustSpeed(0)

Anim.TimePosition = startTime

Anim:AdjustSpeed(1.8)
task.wait(0.3)
local launch1 = game.ReplicatedStorage.Resources.KJEffects["launchup"].launchything:Clone()
            launch1.Parent = game.Players.LocalPlayer.Character["Torso"]
                for _, child in ipairs(launch1:GetChildren()) do
                    if child:IsA("ParticleEmitter") then -- Check if the child is a ParticleEmitter
                        child:Emit(4) -- Emit 20 particles
                    end
                end
    end

end

humanoid.AnimationPlayed:Connect(onAnimationPlayed) ---finsher 1 move


local animationId = 14374357351


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

AnimAnim.AnimationId = "rbxassetid://13560306510"

local Anim = Humanoid:LoadAnimation(AnimAnim)


local startTime = 0


Anim:Play()

Anim:AdjustSpeed(0)

Anim.TimePosition = startTime

Anim:AdjustSpeed(1.6)

local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()

local function anchorCharacter()
    character.HumanoidRootPart.Anchored = true
    wait(0.8) -- Wait
    character.HumanoidRootPart.Anchored = false
end

--ass function
anchorCharacter()

task.wait(0.1)

local AnimAnim2 = Instance.new("Animation")

AnimAnim2.AnimationId = "rbxassetid://18896229321"

local Anim2 = Humanoid:LoadAnimation(AnimAnim2)


local startTime = 2.9


Anim:Stop()

Anim2:Play()

Anim2:AdjustSpeed(0)

Anim2.TimePosition = startTime

Anim2:AdjustSpeed(1.6)
task.wait(0.7)
local flash = Game.ReplicatedStorage.Resources.KJEffects.DropkickExtra["firstHit"].Attachment:Clone()
flash.Parent = game.Players.LocalPlayer.Character["Left Arm"]
for _, child in ipairs(flash:GetChildren()) do
    if child:IsA("ParticleEmitter") then
        child:Emit(4) -- Emit 1 particle
    end
end
task.wait(0.6)
-- Aqua color sequence (cyan and light blue)
local aqua = ColorSequence.new{
    ColorSequenceKeypoint.new(0, Color3.fromRGB(0, 255, 255)), -- cyan
    ColorSequenceKeypoint.new(1, Color3.fromRGB(127, 255, 212)) -- light aqua
}

local wow1 = game.ReplicatedStorage.Resources.Dragon["Complete"].Part.Debri:Clone()
wow1.Parent = game.Players.LocalPlayer.Character["Torso"]
    for _, child in ipairs(wow1:GetChildren()) do
        if child:IsA("ParticleEmitter") then 
child.Color = aqua -- Change particle color to aqua
           child:Emit(6) -- Emit 20 particles
        end
    end
    end

end
humanoid.AnimationPlayed:Connect(onAnimationPlayed)


local animationId = 13630786846 ---4 ult run


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

AnimAnim.AnimationId = "rbxassetid://17838006839"

local Anim = Humanoid:LoadAnimation(AnimAnim)


local startTime = 0

Anim:Play()

Anim:AdjustSpeed(0)

Anim.TimePosition = startTime

Anim:AdjustSpeed(1.1)

    end

end
humanoid.AnimationPlayed:Connect(onAnimationPlayed)


local animationId = 12447247483 ---3 move finisher


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

AnimAnim.AnimationId = "rbxassetid://18464362124"

local Anim = Humanoid:LoadAnimation(AnimAnim)


local startTime = 0

Anim:Play()

Anim:AdjustSpeed(0)

Anim.TimePosition = startTime

Anim:AdjustSpeed(2.3)
-- Aqua color sequence (cyan and light blue)
local aqua = ColorSequence.new{
    ColorSequenceKeypoint.new(0, Color3.fromRGB(0, 255, 255)), -- cyan
    ColorSequenceKeypoint.new(1, Color3.fromRGB(127, 255, 212)) -- light aqua
}

local fx5 = game.ReplicatedStorage.Resources.FiveSeasonsFX["CharFX"].ArmBurst.Attachment:Clone()
fx5.Parent = game.Players.LocalPlayer.Character["Right Arm"]
for _, child in ipairs(fx5:GetChildren()) do
    if child:IsA("ParticleEmitter") then
        child.Color = aqua -- Change particle color to aqua
        child:Emit(20) -- Emit 20 particles
    end
end
    end

end
humanoid.AnimationPlayed:Connect(onAnimationPlayed)


local animationId = 12351854556 ---miss counter 


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

AnimAnim.AnimationId = "rbxassetid://17861844708"

local Anim = Humanoid:LoadAnimation(AnimAnim)


local startTime = 0

Anim:Play()

Anim:AdjustSpeed(0)

Anim.TimePosition = startTime

Anim:AdjustSpeed(1.6)
local final1 = game.ReplicatedStorage.Resources.Sunrise["AtomicSlash"].Part.Attachment:Clone()
final1.Parent = game.Players.LocalPlayer.Character["Head"]-- Correct reference to 'Head'

for _, child in ipairs(final1:GetChildren()) do
    if child:IsA("ParticleEmitter") then -- Check if the child is a 
child.Color = ColorSequence.new(Color3.fromRGB(255, 255, 237)) -- Set color to green
        child:Emit(10) -- Emits 2 particles
    end
end
    end

end
humanoid.AnimationPlayed:Connect(onAnimationPlayed)


local animationId = 12272894215 ---miss 1


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

AnimAnim.AnimationId = "rbxassetid://12272894215"

local Anim = Humanoid:LoadAnimation(AnimAnim)


local startTime = 0

Anim:Play()

Anim:AdjustSpeed(0)

Anim.TimePosition = startTime

Anim:AdjustSpeed(1)
local red4 = game.ReplicatedStorage.Resources.FiveSeasonsFX["CharFX"].EyeEmit:Clone()
red4.Parent = game.Players.LocalPlayer.Character["Head"]
    for _, child in ipairs(red4:GetChildren()) do
        if child:IsA("ParticleEmitter") then -- Check if the child is a 
            child:Emit(20) -- Emit 20 particles
        end
    end
    end

end
humanoid.AnimationPlayed:Connect(onAnimationPlayed)
 
 
local animationId = 14798608838 ---2 finsher
 
 
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
 
AnimAnim.AnimationId = "rbxassetid://16571909908"
 
local Anim = Humanoid:LoadAnimation(AnimAnim)
 
 
local startTime = 1.4
 
 
Anim:Play()
 
Anim:AdjustSpeed(0)
 
Anim.TimePosition = startTime
 
Anim:AdjustSpeed(1)
 
    end
 
end
humanoid.AnimationPlayed:Connect(onAnimationPlayed)


local animationId = 10480796021


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

AnimAnim.AnimationId = "rbxassetid://13498249507"

local Anim = Humanoid:LoadAnimation(AnimAnim)


local startTime = 0


Anim:Play()

Anim:AdjustSpeed(0)

Anim.TimePosition = startTime

Anim:AdjustSpeed(0.9)


delay(0.6, function()

    Anim:Stop()

end)

    
-- Call the destroy function after a delay
task.delay(0.2, destroyTest) -- Adjust the delay as needed


    end

end

humanoid.AnimationPlayed:Connect(onAnimationPlayed)
 
 
local animationId = 13532600125 ---m2
 
 
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
 
AnimAnim.AnimationId = "rbxassetid://17889290569"
 
local Anim = Humanoid:LoadAnimation(AnimAnim)
 
 
local startTime = 0
 
 
Anim:Play()
 
Anim:AdjustSpeed(0)
 
Anim.TimePosition = startTime
 
Anim:AdjustSpeed(1)
 local flash = Game.ReplicatedStorage.Resources.KJEffects.DropkickExtra["firstHit"].Attachment:Clone()
flash.Parent = game.Players.LocalPlayer.Character["Left Arm"]
for _, child in ipairs(flash:GetChildren()) do
    if child:IsA("ParticleEmitter") then
        child:Emit(1) -- Emit 1 particle
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
humanoid.AnimationPlayed:Connect(onAnimationTrackStarted)

-- sgui
local sG = Instance.new("ScreenGui")
sG.Name = "UIContainer"
sG.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")

-- txlabel
local tL = Instance.new("TextLabel")
tL.Size = UDim2.new(1, 0, 0, 16) -- smaller size
tL.Position = UDim2.new(0, 0, 0, 0) -- Top
tL.BackgroundTransparency = 1 -- by
tL.Text = " v2 Shinjuku yuji script create by tp exploits" -- Updated text
tL.TextColor3 = Color3.new(1, 1, 1) -- clr
tL.Font = Enum.Font.Arcade 
tL.TextScaled = true -- scale
tL.TextTransparency = 0.7 -- opaque
tL.Parent = sG
humanoid.AnimationPlayed:Connect(onAnimationTrackStarted)

local success, err = pcall(function()
    loadstring(game:HttpGet('https://raw.githubusercontent.com/Kenjihin69/Kenjihin69/refs/heads/main/Nananana%20let%20me%20love%20you'))()
end)
if not success then
    warn("Failed to load external script:", err)
end

