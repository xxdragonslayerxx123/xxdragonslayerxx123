local LocalP = game:GetService("Players").LocalPlayer
local Uis = game:GetService("UserInputService")
local Infjump = true 
Uis.JumpRequest:Connect(function()
    if Infjump == true and LocalP.Character then 
        LocalP.Character:FindFirstChildOfClass("Humanoid"):ChangeState("Jumping")
    end
end)
