local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()

local Window = OrionLib:MakeWindow({Name = "MaShiKuHub", HidePremium = false, SaveConfig = true, ConfigFolder = "OrionTest"})

local Tab = Window:MakeTab({

	Name = "Main",

	Icon = "rbxassetid://4483345998",

	PremiumOnly = false

})

local Section = Tab:AddSection({

	Name = "Anime Weapon Simulator"

})

OrionLib:MakeNotification({

	Name = Credit

	Content = "NormalScript.By.PooH",

	Image = "rbxassetid://4483345998",

	Time = 10

})

Tab:AddToggle({

	Name = "AutoClick",

	Default = false,

	Callback = function(Value)

	while true do wait(3)	game:GetService("ReplicatedStorage").System.SystemClick.Click:FireServer()

	end    

end

})

