while true do wait()
local args = {
    [1] = "damage",
    [2] = {
        ["EnemyHumanoid"] = workspace.MAP.dummies.Dummy.Humanoid
    }
}

game:GetService("ReplicatedStorage").SkillsInRS.RemoteEvent:FireServer(unpack(args))
end
