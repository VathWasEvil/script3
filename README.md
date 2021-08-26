-- Gui to Lua
-- Version: 3.2

-- Instances:

local HDAdmin = Instance.new("Folder")
local CustomFeatures = Instance.new("Configuration")
local Server = Instance.new("Folder")
local Assets = Instance.new("Folder")
local Modules = Instance.new("Folder")
local Morphs = Instance.new("Folder")
local Tools = Instance.new("Folder")
local Client = Instance.new("Folder")
local StarterKit = Instance.new("Folder")
local Assets_2 = Instance.new("Folder")
local Audio = Instance.new("Folder")
local Modules_2 = Instance.new("Folder")
local SharedModules = Instance.new("Folder")
local Signals = Instance.new("Folder")

--Properties:

HDAdmin.Name = "HD Admin"
HDAdmin.Parent = game.Workspace

CustomFeatures.Name = "CustomFeatures"
CustomFeatures.Parent = HDAdmin

Server.Name = "Server"
Server.Parent = CustomFeatures

Assets.Name = "Assets"
Assets.Parent = Server

Modules.Name = "Modules"
Modules.Parent = Server

Morphs.Name = "Morphs"
Morphs.Parent = Server

Tools.Name = "Tools"
Tools.Parent = Server

Client.Name = "Client"
Client.Parent = CustomFeatures

StarterKit.Name = "StarterKit"
StarterKit.Parent = Client

Assets_2.Name = "Assets"
Assets_2.Parent = Client

Audio.Name = "Audio"
Audio.Parent = Client

Modules_2.Name = "Modules"
Modules_2.Parent = Client

SharedModules.Name = "SharedModules"
SharedModules.Parent = Client

Signals.Name = "Signals"
Signals.Parent = Client

-- Scripts:

local function HFOG_fake_script() -- HDAdmin.About 
	local script = Instance.new('Script', HDAdmin)

	--[[
		
	For information on how to setup and use HD Admin, visit:
	
	https://devforum.roblox.com/t/HD/216819
	
	--]]
end
coroutine.wrap(HFOG_fake_script)()
local function ZKGEEV_fake_script() -- nil.Loader 
	local script = Instance.new('Script', nil)

	--[[
		This loads HD Admin into your game.
		
		Require the 'HD Admin MainModule' by the HD Admin group for automatic updates.
		
		You can view the HD Admin Main Module here:
		https://www.roblox.com/library/3239236979/HD
		
	--]]
	
	local loaderFolder = script.Parent.Parent
	local mainModule = require(3239236979)
	mainModule:Initialize(loaderFolder)
	loaderFolder:Destroy()
end
coroutine.wrap(ZKGEEV_fake_script)()
