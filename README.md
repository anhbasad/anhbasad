local AnisForCommandAndMore = Instance.new("ScreenGui")
local Main = Instance.new("Frame")
local BeautyA = Instance.new("Frame")
local Name = Instance.new("TextLabel")
local BeautyB = Instance.new("Frame")
local Credit = Instance.new("TextLabel")
local WalkSpeed = Instance.new("TextButton")
local Btools = Instance.new("TextButton")
local Noclip = Instance.new("TextButton")
local Admin = Instance.new("TextButton")
local Aimbot = Instance.new("TextButton")
local JailbreakGui = Instance.new("TextButton")
local Gravity = Instance.new("TextButton")
local InfJump = Instance.new("TextButton")
local QToTeleport = Instance.new("TextButton")
local Exit = Instance.new("TextButton")
local Open = Instance.new("TextButton")
 
-- Properties
 
AnisForCommandAndMore.Name = "Anis For Command And More"
AnisForCommandAndMore.Parent = game.CoreGui
AnisForCommandAndMore.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
 
Main.Name = "Main"
Main.Parent = AnisForCommandAndMore
Main.Active = true
Main.BackgroundColor3 = Color3.new(0.113725, 0.113725, 0.113725)
Main.Position = UDim2.new(0.26543209, 0, 0.291154802, 0)
Main.Size = UDim2.new(0, 596, 0, 406)
Main.Visible = false
Main.Draggable = true
 
BeautyA.Name = "BeautyA"
BeautyA.Parent = Main
BeautyA.BackgroundColor3 = Color3.new(1, 0, 1)
BeautyA.Size = UDim2.new(0, 596, 0, 39)
 
Name.Name = "Name"
Name.Parent = BeautyA
Name.BackgroundColor3 = Color3.new(1, 1, 1)
Name.BackgroundTransparency = 1
Name.Position = UDim2.new(0.315436244, 0, 0, 0)
Name.Size = UDim2.new(0, 230, 0, 39)
Name.Font = Enum.Font.Cartoon
Name.Text = "venuslockscript"
Name.TextColor3 = Color3.new(1, 1, 1)
Name.TextScaled = true
Name.TextSize = 20
Name.TextWrapped = true
 
BeautyB.Name = "BeautyB"
BeautyB.Parent = Main
BeautyB.BackgroundColor3 = Color3.new(1, 0, 1)
BeautyB.Position = UDim2.new(0, 0, 0.903940916, 0)
BeautyB.Size = UDim2.new(0, 596, 0, 39)
 
Credit.Name = "Credit"
Credit.Parent = BeautyB
Credit.BackgroundColor3 = Color3.new(1, 1, 1)
Credit.BackgroundTransparency = 1
Credit.Position = UDim2.new(0.315436244, 0, 0, 0)
Credit.Size = UDim2.new(0, 230, 0, 39)
Credit.Font = Enum.Font.Cartoon
Credit.Text = ""
Credit.TextColor3 = Color3.new(1, 1, 1)
Credit.TextSize = 20
 
WalkSpeed.Name = "WalkSpeed"
WalkSpeed.Parent = Main
WalkSpeed.BackgroundColor3 = Color3.new(1, 0, 1)
WalkSpeed.Position = UDim2.new(0, 0, 0.145320192, 0)
WalkSpeed.Size = UDim2.new(0, 173, 0, 59)
WalkSpeed.Font = Enum.Font.Cartoon
WalkSpeed.Text = "WalkSpeed"
WalkSpeed.TextColor3 = Color3.new(1, 1, 1)
WalkSpeed.TextScaled = true
WalkSpeed.TextSize = 14
WalkSpeed.MouseButton1Down:connect(function()
game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = 150
end)
 
Btools.Name = "Btools"
Btools.Parent = Main
Btools.BackgroundColor3 = Color3.new(1, 0, 1)
Btools.Position = UDim2.new(0.364093959, 0, 0.145320192, 0)
Btools.Size = UDim2.new(0, 173, 0, 59)
Btools.Font = Enum.Font.Cartoon
Btools.Text = "Btools"
Btools.TextColor3 = Color3.new(1, 1, 1)
Btools.TextScaled = true
Btools.TextSize = 14
Btools.MouseButton1Down:connect(function()
game.StarterGui:SetCoreGuiEnabled(Enum.CoreGuiType.Backpack, true)
for index, child in pairs(game:GetService("Workspace"):GetChildren()) do
   if child.ClassName == "Part" then
       child.Locked = false
   end
   if child.ClassName == "MeshPart" then
       child.Locked = false
   end
   if child.ClassName == "UnionOperation" then
       child.Locked = false
   end
   if child.ClassName == "Model" then
       for index, chil in pairs(child:GetChildren()) do
           if chil.ClassName == "Part" then
               chil.Locked = false
           end
           if chil.ClassName == "MeshPart" then
               chil.Locked = false
           end
           if chil.ClassName == "UnionOperation" then
               chil.Locked = false
           end
           if chil.ClassName == "Model" then
               for index, childe in pairs(chil:GetChildren()) do
                   if childe.ClassName == "Part" then
                       childe.Locked = false
                   end
                   if childe.ClassName == "MeshPart" then
                       childe.Locked = false
                   end
                   if childe.ClassName == "UnionOperation" then
                       childe.Locked = false
                   end
                   if childe.ClassName == "Model" then
                       for index, childeo in pairs(childe:GetChildren()) do
                           if childeo.ClassName == "Part" then
                               childeo.Locked = false
                           end
                           if childeo.ClassName == "MeshPart" then
                               childeo.Locked = false
                           end
                           if childeo.ClassName == "UnionOperation" then
                               childeo.Locked = false
                           end
                           if childeo.ClassName == "Model" then
                           end
                       end
                   end
               end
           end
       end
   end
end
c = Instance.new("HopperBin", game:GetService("Players").LocalPlayer.Backpack)
c.BinType = Enum.BinType.Hammer
c = Instance.new("HopperBin", game:GetService("Players").LocalPlayer.Backpack)
c.BinType = Enum.BinType.Clone
c = Instance.new("HopperBin", game:GetService("Players").LocalPlayer.Backpack)
c.BinType = Enum.BinType.Grab
end)
 
Noclip.Name = "Noclip"
Noclip.Parent = Main
Noclip.BackgroundColor3 = Color3.new(1, 0, 1)
Noclip.Position = UDim2.new(0.709731519, 0, 0.145320192, 0)
Noclip.Size = UDim2.new(0, 173, 0, 59)
Noclip.Font = Enum.Font.Cartoon
Noclip.Text = "Noclip"
Noclip.TextColor3 = Color3.new(1, 1, 1)
Noclip.TextScaled = true
Noclip.TextSize = 14
Noclip.MouseButton1Down:connect(function()
noclip = false
game:GetService('RunService').Stepped:connect(function()
if noclip then
game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
end
end)
plr = game.Players.LocalPlayer
mouse = plr:GetMouse()
mouse.KeyDown:connect(function(key)
 
if key == "e" then
noclip = not noclip
game.Players.LocalPlayer.Character.Humanoid:ChangeState(11)
end
end)
print('Loaded')
print('Press "E" to noclip')
 
end)
 
Admin.Name = "Admin"
Admin.Parent = Main
Admin.BackgroundColor3 = Color3.new(1, 0, 1)
Admin.Position = UDim2.new(0.709731519, 0, 0.42610836, 0)
Admin.Size = UDim2.new(0, 173, 0, 59)
Admin.Font = Enum.Font.Cartoon
Admin.Text = "Admin"
Admin.TextColor3 = Color3.new(1, 1, 1)
Admin.TextScaled = true
Admin.TextSize = 14
Admin.MouseButton1Down:connect(function()
-- Creator: illremember#3799
 
-- Credits to infinite yield, harkinian, dex creators
 
prefix = ":"
wait(0.3)
Commands = {
    '[-] cmdbar is shown when ; is pressed.',
    '[1] kill [plr] -- You need a tool! Will kill the player, use rkill to kill you and player',
    '[2] bring [plr] -- You need a tool! Will bring player to you',
    '[3] spin [plr] -- You need a tool! Makes you and the player spin crazy',
    '[4] unspin -- Use after using spin cmd and dying, so you stop loop teleporting',
    '[5] attach [plr] -- You need a tool! Attaches you to player',
    '[6] unattach [plr] -- Attempts to unattach you from a player',
    '[7] follow [plr] -- Makes you follow behind the player',
    '[8] unfollow',
    '[9] freefall [plr] -- You need a tool! Teleports you and the player up into the air',
    '[10] trail [plr] -- The opposite of follow, you stay infront of player',
    '[11] untrail',
    '[12] orbit [plr] -- Makes you orbit the player',
    '[13] unorbit',
    '[14] fling [plr] -- Makes you fling the player',
    '[15] unfling',
    '[16] fecheck -- Checks if the game is FE or not',
    '[17] void [plr] -- Teleports player to the void',
    '[18] noclip -- Gives you noclip to walk through walls',
    '[19] clip -- Removes noclip',
    '[20] speed [num]/ws [num] -- Changes how fast you walk 16 is default',
    '[21] jumppower [num]/jp [num] -- Changes how high you jump 50 is default',
    '[22] hipheight [num]/hh [num] -- Changes how high you float 0 is default',
    '[23] default -- Changes your speed, jumppower and hipheight to default values',
    '[24] annoy [plr] -- Loop teleports you to the player',
    '[25] unannoy',
    '[26] headwalk [plr] -- Loop teleports you to the player head',
    '[27] unheadwalk',
    '[28] nolimbs -- Removes your arms and legs',
    '[29] god -- Gives you FE Godmode',
    '[30] drophats -- Drops your accessories',
    '[31] droptool -- Drops any tool you have equipped',
    '[32] loopdhats -- Loop drops your accessories',
    '[33] unloopdhats',
    '[34] loopdtool -- Loop drops any tools you have equipped',
    '[35] unloopdtool',
    '[36] invisible -- Gives you invisibility CREDIT TO TIMELESS',
    '[37] view [plr] -- Changes your camera to the player character',
    '[38] unview',
    '[39] goto [plr] -- Teleports you to player',
    '[40] fly -- Allows you to fly, credit to Infinite Yield',
    '[41] unfly',
    '[42] chat [msg] -- Makes you chat a message',
    '[43] spam [msg] -- Spams a message',
    '[44] unspam',
    '[45] spamwait [num] -- Changes delay of chatting a message for the spam command in seconds default is 1 second',
    '[46] pmspam [plr] -- Spams a player in private message',
    '[47] unpmspam',
    '[48] cfreeze [plr] -- Freezes a player on your client, they will only be frozen for you',
    '[49] uncfreeze [plr]',
    '[50] unlockws -- Unlocks the workspace',
    '[51] lockws -- Locks the workspace',
    '[52] btools -- Gives you btools that will only show to you useful for deleting certain blocks only for you',
    '[53] pstand -- Enables platform stand',
    '[54] unpstand -- Disables platform stand',
    '[55] blockhead -- Removes your head mesh',
    '[56] sit',
    '[57] bringobj [obj] -- Only shows on client, brings an object/part to you constantly, can be used to bring healing parts, weapons, money etc, type in exact name',
    '[58] wsvis [num] -- Changes visibility of workspace parts, num should be between 0 and 1, only shows client sided',
    '[59] hypertotal -- Loads in my FE GUI Hypertotal',
    '[60] cmds -- Prints all commands',
    '[61] rmeshhats/blockhats -- Removes the meshes of all your accessories aka block hats',
    '[62] rmeshtool/blocktool -- Removes the mesh of the tool you have equipped aka block tool',
    '[63] spinner -- Makes you spin',
    '[64] nospinner',
    '[65] reach [num] -- Gives you reach, mostly used for swords, say ;reachd for default and enter number after for custom',
    '[66] noreach -- Removes reach, must have tool equipped',
    '[67] rkill [plr] -- Kills you and the player, use kill to just kill the player without dying',
    '[68] tp me [plr] -- Alternative to goto',
    '[69] cbring [plr] -- Brings player infront of you, shows only on client, allows you to do damage to player',
    '[70] uncbring',
    '[71] swap [plr] -- You need a tool! Swaps players position with yours and your position with players',
    '[72] givetool [plr] -- Gives the tool you have equipped to the player',
    '[73] glitch [plr] -- Glitches you and the player, looks very cool',
    '[74] unglitch -- Unglitches you',
    '[75] grespawn -- Alternative to normal respawn and usually works best for when you want to reset with FE Godmode',
    '[76] explorer -- Loads up DEX',
    '[77] reset -- Resets your character.',
    '[78] anim [id] -- Applies an animation on you, must be created by ROBLOX',
    '[79] animgui -- Loads up Energize animations GUI',
    '[80] savepos -- Saves your current position',
    '[81] loadpos -- Teleports you to your saved position',
    '[82] bang [plr] -- 18+ will not work if you have FE Godmode on',
    '[83] unbang',
    '[84] delcmdbar -- Removes the command bar completely',
    '[85] bringmod [obj] -- Brings all the parts in a model, client only, comes from ;bringobj enter exact name of model',
    '[86] shutdown -- Uses harkinians script to shutdown server',
    '[87] respawn -- If grespawn doesnt work you can use respawn',
    '[88] delobj [obj] -- Deletes a certain brick in workspace, client sided',
    '[89] getplrs -- Prints all players in game',
    '[90] deldecal -- Deletes all decals client sided',
    '[91] opfinality -- Loads in my FE GUI Opfinality',
    '[92] remotes -- Prints all remotes in the game in the console when added',
    '[93] noremotes -- Stops printing remotes',
    '[94] tpdefault -- Stops all loop teleports to a player',
    '[95] stopsit -- Will not allow you to sit',
    '[96] gosit -- Allows you to sit',
    '[97] clicktp -- Enables click tp',
    '[98] noclicktp -- Disables click tp',
    '[99] toolson -- If any tools are dropped in the workspace you will automatically get them',
    '[100] toolsoff -- Stops ;toolson',
    '[101] version -- Gets the admin version',
    '[102] state [num] -- Changes your humanoid state, ;unstate to stop.',
    '[103] gravity [num] -- Changes workspace gravity default is 196.2',
    '[104] pgs -- Checks if the game has PGSPhysicsSolverEnabled enabled',
    '[105] clickdel -- Delete any block you press q on, client sided',
    '[106] noclickdel -- Stops clickdel',
    '[107] looprhats -- Loop removes mesh of your hats/loop block hats',
    '[108] unlooprhats -- Stops loop removing mesh',
    '[109] looprtool -- Loop removes mesh of your tool/loop block tools',
    '[110] unlooprtool -- Stops loop removing mesh',
    '[111] givealltools [plr] -- Gives all the tools you have in your backpack to the player',
    '[112] age [plr] -- Makes you chat the account age of the player',
    '[113] id [plr] -- Makes you chat the account ID of the player',
    '[114] .age [plr] -- Privately shows you the account age of the player',
    '[115] .id [plr] -- Privately shows you the account ID of the player',
    '[116] gameid -- Shows the game ID',
    '[117] removeinvis -- Removes all invisible walls/parts, client sided',
    '[118] removefog -- Removes fog, client sided',
    '[119] disable -- Disables your character by removing humanoid',
    '[120] enable -- Enables your character by adding humanoid',
    '[121] prefix [key] -- Changes the prefix used, default is ;',
    '[122] ;resetprefix -- Resets the prefix to ; incase you change it to an unusable prefix. Say exactly ";resetprefix" to do this command, no matter what your prefix is set to.',
    '[123] flyspeed [num] -- Change your fly speed, default is 1',
    '[124] carpet [plr] -- Makes you a carpet for a player, will not work if FE Godmode is on',
    '[125] uncarpet -- Stops carpet player',
    '[126] stare [plr] -- Turns your character to stare at another player',
    '[127] unstare -- Stops stare player',
    '[128] logchat -- Logs all chat (including /e and whispers) of all players',
    '[129] unlogchat -- Disables logchat',
    '[130] fixcam -- Fixes/resets your camera',
    '[131] unstate -- Stops changing state',
}
speedget = 1
 
lplayer = game:GetService("Players").LocalPlayer
 
lplayer.CharacterAdded:Connect(function(character)
    spin = false
    flying = false
    staring = false
    banpl = false
end)
 
function change()
    prefix = prefix
    speedfly = speedfly
end
 
function GetPlayer(String) -- Credit to Timeless/xFunnieuss
    local Found = {}
    local strl = String:lower()
    if strl == "all" then
        for i,v in pairs(game:GetService("Players"):GetPlayers()) do
            table.insert(Found,v)
        end
    elseif strl == "others" then
        for i,v in pairs(game:GetService("Players"):GetPlayers()) do
            if v.Name ~= lplayer.Name then
                table.insert(Found,v)
            end
        end  
    elseif strl == "me" then
        for i,v in pairs(game:GetService("Players"):GetPlayers()) do
            if v.Name == lplayer.Name then
                table.insert(Found,v)
            end
        end  
    else
        for i,v in pairs(game:GetService("Players"):GetPlayers()) do
            if v.Name:lower():sub(1, #String) == String:lower() then
                table.insert(Found,v)
            end
        end    
    end
    return Found    
end
 
local Mouse = lplayer:GetMouse()
 
spin = false
followed = false
traill = false
noclip = false
annoying = false
hwalk = false
droppinghats = false
droppingtools = false
flying = false
spamdelay = 1
spamming = false
spammingpm = false
cbringing = false
remotes = true
added = true
binds = false
stopsitting = false
clickgoto = false
gettingtools = false
removingmeshhats = false
removingmeshtool = false
clickdel = false
staring = false
chatlogs = false
banpl = false
changingstate = false
statechosen = 0
 
adminversion = "Reviz Admin by illremember, Version 2.0"
 
flying = false
speedfly = 1
 
function plrchat(plr, chat)
print(plr.Name..": "..tick().."\n"..chat)
end
 
for i,v in pairs(game:GetService("Players"):GetPlayers()) do
v.Chatted:connect(function(chat)
if chatlogs then
plrchat(v, chat)
end
end)
end
game:GetService("Players").PlayerAdded:connect(function(plr)
plr.Chatted:connect(function(chat)
if chatlogs then
plrchat(plr, chat)
end
end)
end)
 
 
local ScreenGui = Instance.new("ScreenGui")
local Frame = Instance.new("Frame")
local CMDBAR = Instance.new("TextBox")
ScreenGui.Parent = game:GetService("CoreGui")
Frame.Parent = ScreenGui
Frame.BackgroundColor3 = Color3.new(0.3, 0.1, 0.1)
Frame.BackgroundTransparency = 0.3
Frame.Position = UDim2.new(0.5, 0, 0, 10)
Frame.Size = UDim2.new(0, 200, 0, 40)
Frame.Active = true
Frame.Draggable = true
CMDBAR.Name = "CMDBAR"
CMDBAR.Parent = Frame
CMDBAR.BackgroundColor3 = Color3.new(0.105882, 0.164706, 0.207843)
CMDBAR.BackgroundTransparency = 0.20000000298023
CMDBAR.Size = UDim2.new(0, 180, 0, 20)
CMDBAR.Position = UDim2.new(0.05, 0, 0.25, 0)
CMDBAR.Font = Enum.Font.SourceSansLight
CMDBAR.FontSize = Enum.FontSize.Size14
CMDBAR.TextColor3 = Color3.new(0.945098, 0.945098, 0.945098)
CMDBAR.TextScaled = true
CMDBAR.TextSize = 14
CMDBAR.TextWrapped = true
CMDBAR.Text = "Press ; to type, Enter to execute"
 
local CMDS = Instance.new("ScreenGui")
local CMDSFRAME = Instance.new("Frame")
local ScrollingFrame = Instance.new("ScrollingFrame")
local TextLabel = Instance.new("TextLabel")
local closegui = Instance.new("TextButton")
CMDS.Name = "CMDS"
CMDS.Parent = game:GetService("CoreGui")
CMDSFRAME.Name = "CMDSFRAME"
CMDSFRAME.Parent = CMDS
CMDSFRAME.Active = true
CMDSFRAME.BackgroundColor3 = Color3.new(0.223529, 0.231373, 0.309804)
CMDSFRAME.BorderSizePixel = 0
CMDSFRAME.Draggable = true
CMDSFRAME.Position = UDim2.new(0, 315, 0, 100)
CMDSFRAME.Size = UDim2.new(0, 275, 0, 275)
CMDSFRAME.Visible = false
ScrollingFrame.Parent = CMDSFRAME
ScrollingFrame.BackgroundColor3 = Color3.new(0.160784, 0.160784, 0.203922)
ScrollingFrame.BorderSizePixel = 0
ScrollingFrame.Position = UDim2.new(0, 0, 0.0729999989, 0)
ScrollingFrame.Size = UDim2.new(1.04999995, 0, 0.92900002, 0)
ScrollingFrame.CanvasSize = UDim2.new(0, 0, 10, 0)
TextLabel.Parent = ScrollingFrame
TextLabel.BackgroundColor3 = Color3.new(1, 1, 1)
TextLabel.BackgroundTransparency = 1
TextLabel.Size = UDim2.new(0.930000007, 0, 1, 0)
TextLabel.Font = Enum.Font.SourceSans
TextLabel.FontSize = Enum.FontSize.Size18
TextLabel.Text = "[-] cmdbar is shown when ; is pressed.,\n[1] kill [plr] -- You need a tool! Will kill the player, use rkill to kill you and player,\n[2] bring [plr] -- You need a tool! Will bring player to you,\n[3] spin [plr] -- You need a tool! Makes you and the player spin crazy,\n[4] unspin -- Use after using spin cmd and dying, so you stop loop teleporting,\n[5] attach [plr] -- You need a tool! Attaches you to player,\n[6] unattach [plr] -- Attempts to unattach you from a player,\n[7] follow [plr] -- Makes you follow behind the player,\n[8] unfollow,\n[9] freefall [plr] -- You need a tool! Teleports you and the player up into the air,\n[10] trail [plr] -- The opposite of follow, you stay infront of player,\n[11] untrail,\n[12] orbit [plr] -- Makes you orbit the player,\n[13] unorbit,\n[14] fling [plr] -- Makes you fling the player,\n[15] unfling,\n[16] fecheck -- Checks if the game is FE or not,\n[17] void [plr] -- Teleports player to the void,\n[18] noclip -- Gives you noclip to walk through walls,\n[19] clip -- Removes noclip,\n[20] speed [num]/ws [num] -- Changes how fast you walk 16 is default,\n[21] jumppower [num]/jp [num] -- Changes how high you jump 50 is default,\n[22] hipheight [num]/hh [num] -- Changes how high you float 0 is default,\n[23] default -- Changes your speed, jumppower and hipheight to default values,\n[24] annoy [plr] -- Loop teleports you to the player,\n[25] unannoy,\n[26] headwalk [plr] -- Loop teleports you to the player head,\n[27] unheadwalk,\n[28] nolimbs -- Removes your arms and legs,\n[29] god -- Gives you FE Godmode,\n[30] drophats -- Drops your accessories,\n[31] droptool -- Drops any tool you have equipped,\n[32] loopdhats -- Loop drops your accessories,\n[33] unloopdhats,\n[34] loopdtool -- Loop drops any tools you have equipped,\n[35] unloopdtool,\n[36] invisible -- Gives you invisibility CREDIT TO TIMELESS,\n[37] view [plr] -- Changes your camera to the player character,\n[38] unview,\n[39] goto [plr] -- Teleports you to player,\n[40] fly -- Allows you to fly,\n[41] unfly,\n[42] chat [msg] -- Makes you chat a message,\n[43] spam [msg] -- Spams a message,\n[44] unspam,\n[45] spamwait [num] -- Changes delay of chatting a message for the spam command in seconds default is 1 second,\n[46] pmspam [plr] -- Spams a player in private message,\n[47] unpmspam,\n[48] cfreeze [plr] -- Freezes a player on your client, they will only be frozen for you,\n[49] uncfreeze [plr],\n[50] unlockws -- Unlocks the workspace,\n[51] lockws -- Locks the workspace,\n[52] btools -- Gives you btools that will only show to you useful for deleting certain blocks only for you,\n[53] pstand -- Enables platform stand,\n[54] unpstand -- Disables platform stand,\n[55] blockhead -- Removes your head mesh,\n[56] sit,\n[57] bringobj [obj] -- Only shows on client, brings an object/part to you constantly, can be used to bring healing parts, weapons, money etc, type in exact name,\n[58] wsvis [num] -- Changes visibility of workspace parts, num should be between 0 and 1, only shows client sided,\n[59] hypertotal -- Loads in my FE GUI Hypertotal,\n[60] cmds -- Prints all commands,\n[61] rmeshhats/blockhats -- Removes the meshes of all your accessories aka block hats,\n[62] rmeshtool/blocktool -- Removes the mesh of the tool you have equipped aka block tool,\n[63] spinner -- Makes you spin,\n[64] nospinner,\n[65] reach [num] -- Gives you reach, mostly used for swords, say ;reachd for default and enter number after for custom,\n[66] noreach -- Removes reach, must have tool equipped,\n[67] rkill [plr] -- Kills you and the player, use kill to just kill the player without dying,\n[68] tp me [plr] -- Alternative to goto,\n[69] cbring [plr] -- Brings player infront of you, shows only on client, allows you to do damage to player,\n[70] uncbring,\n[71] swap [plr] -- You need a tool! Swaps players position with yours and your position with players,\n[72] givetool [plr] -- Gives the tool you have equipped to the player,\n[73] glitch [plr] -- Glitches you and the player, looks very cool,\n[74] unglitch -- Unglitches you,\n[75] grespawn -- Alternative to normal respawn and usually works best for when you want to reset with FE Godmode,\n[76] explorer -- Loads up DEX,\n[77] reset -- Resets your character.,\n[78] anim [id] -- Applies an animation on you, must be created by ROBLOX,\n[79] animgui -- Loads up Energize animations GUI,\n[80] savepos -- Saves your current position,\n[81] loadpos -- Teleports you to your saved position,\n[82] bang [plr] -- 18+,\n[83] unbang,\n[84] delcmdbar -- Removes the command bar completely,\n[85] bringmod [obj] -- Brings all the parts in a model, client only, comes from ;bringobj enter exact name of model,\n[86] shutdown -- Uses harkinians script to shutdown server,\n[87] respawn -- If grespawn doesnt work you can use respawn,\n[88] delobj [obj] -- Deletes a certain brick in workspace, client sided,\n[89] getplrs -- Prints all players in game,\n[90] deldecal -- Deletes all decals client sided,\n[91] opfinality -- Loads in my FE GUI Opfinality,\n[92] remotes -- Prints all remotes in the game in the console when added,\n[93] noremotes -- Stops printing remotes,\n[94] tpdefault -- Stops all loop teleports to a player,\n[95] stopsit -- Will not allow you to sit,\n[96] gosit -- Allows you to sit,\n[97] clicktp -- Enables click tp,\n[98] noclicktp -- Disables click tp,\n[99] toolson -- If any tools are dropped in the workspace you will automatically get them,\n[100] toolsoff -- Stops ;toolson,\n[101] version -- Gets the admin version, \n This list of commands is NOT showing everything, go to my thread in the pastebin link to see ALL commands."
TextLabel.TextColor3 = Color3.new(1, 1, 1)
TextLabel.TextSize = 15
TextLabel.TextWrapped = true
TextLabel.TextXAlignment = Enum.TextXAlignment.Left
TextLabel.TextYAlignment = Enum.TextYAlignment.Top
closegui.Name = "closegui"
closegui.Parent = CMDSFRAME
closegui.BackgroundColor3 = Color3.new(0.890196, 0.223529, 0.0588235)
closegui.BorderSizePixel = 0
closegui.Position = UDim2.new(0.995000005, 0, 0, 0)
closegui.Size = UDim2.new(0.0545952693, 0, 0.0728644878, 0)
closegui.Font = Enum.Font.SourceSansBold
closegui.FontSize = Enum.FontSize.Size24
closegui.Text = "X"
closegui.TextColor3 = Color3.new(1, 1, 1)
closegui.TextSize = 20
 
closegui.MouseButton1Click:connect(function()
    CMDSFRAME.Visible = false
end)
 
game:GetService('RunService').Stepped:connect(function()
    if spin then
        lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[spinplr.Name].Character.HumanoidRootPart.CFrame
    end
    if followed then
        lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[flwplr.Name].Character.HumanoidRootPart.CFrame + game:GetService("Players")[flwplr.Name].Character.HumanoidRootPart.CFrame.lookVector * -5
    end
    if traill then
        lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[trlplr.Name].Character.HumanoidRootPart.CFrame + game:GetService("Players")[trlplr.Name].Character.HumanoidRootPart.CFrame.lookVector * 5
    end
    if annoying then
        lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[annplr.Name].Character.HumanoidRootPart.CFrame
    end
    if hwalk then
        lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[hdwplr.Name].Character.HumanoidRootPart.CFrame + Vector3.new(0, 4, 0)
    end
    if staring then
        lplayer.Character.HumanoidRootPart.CFrame = CFrame.new(lplayer.Character.Torso.Position, game:GetService("Players")[stareplr.Name].Character.Torso.Position)
    end
end)
game:GetService('RunService').Stepped:connect(function()
    if noclip then
        if lplayer.Character.Humanoid.RigType == Enum.HumanoidRigType.R6 then
            lplayer.Character.Head.CanCollide = false
            lplayer.Character.Torso.CanCollide = false
            lplayer.Character["Left Leg"].CanCollide = false
            lplayer.Character["Right Leg"].CanCollide = false
        else
            lplayer.Character.Humanoid:ChangeState(11)
        end
    end
    if changingstate then
        lplayer.Character.Humanoid:ChangeState(statechosen)
    end
end)
game:GetService('RunService').Stepped:connect(function()
    if droppinghats then
        for i,v in pairs(lplayer.Character:GetChildren()) do
            if (v:IsA("Accessory")) or (v:IsA("Hat")) then
                v.Parent = workspace
            end
        end
    end
    if droppingtools then
        for i,v in pairs(lplayer.Character:GetChildren()) do
            if (v:IsA("Tool")) then
                v.Parent = workspace
            end
        end
    end
    if removingmeshhats then
        for i,v in pairs(lplayer.Character:GetChildren()) do
            if (v:IsA("Accessory")) or (v:IsA("Hat")) then
                v.Handle.Mesh:Destroy()
            end
        end
    end
    if removingmeshtool then
        for i,v in pairs(lplayer.Character:GetChildren()) do
            if (v:IsA("Tool")) then
                v.Handle.Mesh:Destroy()
            end
        end
    end
end)
game:GetService('RunService').Stepped:connect(function()
    if banpl then
        lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[bplrr].Character.HumanoidRootPart.CFrame
    end
end)
game:GetService('RunService').Stepped:connect(function()
    if stopsitting then
        lplayer.Character.Humanoid.Sit = false
    end
end)
 
plr = lplayer
hum = plr.Character.HumanoidRootPart
mouse = plr:GetMouse()
mouse.KeyDown:connect(function(key)
    if key == "e" then
        if mouse.Target then
            if clickgoto then
                hum.CFrame = CFrame.new(mouse.Hit.x, mouse.Hit.y + 5, mouse.Hit.z)
            elseif clickdel then
                mouse.Target:Destroy()
            end
        end
    end
end)
 
game:GetService("Workspace").ChildAdded:connect(function(part)
    if gettingtools then
        if part:IsA("Tool") then
            part.Handle.CFrame = lplayer.Character.HumanoidRootPart.CFrame
        end
    end
end)
 
lplayer.Chatted:Connect(function(msg)
    if string.sub(msg, 1, 6) == (prefix.."kill ") then
        if string.sub(msg, 7) == "me" then
            lplayer.Character.HumanoidRootPart.CFrame = CFrame.new(100000,0,100000)
        else
            for i,v in pairs(GetPlayer(string.sub(msg, 7)))do
                local NOW = lplayer.Character.HumanoidRootPart.CFrame
                lplayer.Character.Humanoid.Name = 1
                local l = lplayer.Character["1"]:Clone()
                l.Parent = lplayer.Character
                l.Name = "Humanoid"
                wait(0.1)
                lplayer.Character["1"]:Destroy()
                game:GetService("Workspace").CurrentCamera.CameraSubject = lplayer.Character
                lplayer.Character.Animate.Disabled = true
                wait(0.1)
                lplayer.Character.Animate.Disabled = false
                lplayer.Character.Humanoid.DisplayDistanceType = "None"
                for i,v in pairs(game:GetService'Players'.LocalPlayer.Backpack:GetChildren())do
                lplayer.Character.Humanoid:EquipTool(v)
                end
                local function tp(player,player2)
                local char1,char2=player.Character,player2.Character
                if char1 and char2 then
                char1:MoveTo(char2.Head.Position)
                end
                end
                wait(0.1)
                lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character.HumanoidRootPart.CFrame
                wait(0.2)
                lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character.HumanoidRootPart.CFrame
                wait(0.5)
                lplayer.Character.HumanoidRootPart.CFrame = CFrame.new(Vector3.new(-100000,10,-100000))
                wait(0.7)
                tp(lplayer,game:GetService("Players")[v.Name])
                wait(0.7)
                lplayer.Character.HumanoidRootPart.CFrame = NOW
                game:GetService("StarterGui"):SetCore("SendNotification", {
                Title = "Tools needed!";
                Text = "You need a tool in your backpack for this command!";
                })
            end
        end
    end
    if string.sub(msg, 1, 7) == (prefix.."bring ") then
        for i,v in pairs(GetPlayer(string.sub(msg, 8)))do
            local NOW = lplayer.Character.HumanoidRootPart.CFrame
            lplayer.Character.Humanoid.Name = 1
            local l = lplayer.Character["1"]:Clone()
            l.Parent = lplayer.Character
            l.Name = "Humanoid"
            wait(0.1)
            lplayer.Character["1"]:Destroy()
            game:GetService("Workspace").CurrentCamera.CameraSubject = lplayer.Character
            lplayer.Character.Animate.Disabled = true
            wait(0.1)
            lplayer.Character.Animate.Disabled = false
            lplayer.Character.Humanoid.DisplayDistanceType = "None"
            for i,v in pairs(game:GetService'Players'.LocalPlayer.Backpack:GetChildren())do
            lplayer.Character.Humanoid:EquipTool(v)
            end
            local function tp(player,player2)
            local char1,char2=player.Character,player2.Character
            if char1 and char2 then
            char1.HumanoidRootPart.CFrame = char2.HumanoidRootPart.CFrame
            end
            end
            local function getout(player,player2)
            local char1,char2=player.Character,player2.Character
            if char1 and char2 then
            char1:MoveTo(char2.Head.Position)
            end
            end
            tp(game:GetService("Players")[v.Name], lplayer)
            wait(0.2)
            tp(game:GetService("Players")[v.Name], lplayer)
            wait(0.5)
            lplayer.Character.HumanoidRootPart.CFrame = NOW
            wait(0.5)
            getout(lplayer, game:GetService("Players")[v.Name])
            wait(0.3)
            lplayer.Character.HumanoidRootPart.CFrame = NOW
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Tools needed!";
            Text = "You need a tool in your backpack for this command!";
            })
        end
    end
    if string.sub(msg, 1, 6) == (prefix.."spin ") then
        for i,v in pairs(GetPlayer(string.sub(msg, 7))) do
            lplayer.Character.Humanoid.Name = 1
            local l = lplayer.Character["1"]:Clone()
            l.Parent = lplayer.Character
            l.Name = "Humanoid"
            wait(0.1)
            lplayer.Character["1"]:Destroy()
            game:GetService("Workspace").CurrentCamera.CameraSubject = lplayer.Character
            lplayer.Character.Animate.Disabled = true
            wait(0.1)
            lplayer.Character.Animate.Disabled = false
            lplayer.Character.Humanoid.DisplayDistanceType = "None"
            lplayer.Character.Animate.Disabled = false
            for i,v in pairs(game:GetService'Players'.LocalPlayer.Backpack:GetChildren())do
            lplayer.Character.Humanoid:EquipTool(v)
            end
            lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character["Left Arm"].CFrame
            spinplr = v
            wait(0.5)
            spin = true
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Tools needed!";
            Text = "You need a tool in your backpack for this command!";
            })
        end
    end
    if string.sub(msg, 1, 7) == (prefix.."unspin") then
        spin = false
    end
    if string.sub(msg, 1, 8) == (prefix.."attach ") then
        for i,v in pairs(GetPlayer(string.sub(msg, 9))) do
            lplayer.Character.Humanoid.Name = 1
            local l = lplayer.Character["1"]:Clone()
            l.Parent = lplayer.Character
            l.Name = "Humanoid"
            wait(0.1)
            lplayer.Character["1"]:Destroy()
            game:GetService("Workspace").CurrentCamera.CameraSubject = lplayer.Character
            lplayer.Character.Animate.Disabled = true
            wait(0.1)
            lplayer.Character.Animate.Disabled = false
            lplayer.Character.Humanoid.DisplayDistanceType = "None"
            for i,v in pairs(game:GetService'Players'.LocalPlayer.Backpack:GetChildren())do
            lplayer.Character.Humanoid:EquipTool(v)
            end
            lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character["Left Arm"].CFrame
            wait(0.3)
            lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character["Left Arm"].CFrame
            attplr = v
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Tools needed!";
            Text = "You need a tool in your backpack for this command!";
            })
        end
    end
    if string.sub(msg, 1, 10) == (prefix.."unattach ") then
        for i,v in pairs(GetPlayer(string.sub(msg, 11))) do
            local function getout(player,player2)
            local char1,char2=player.Character,player2.Character
            if char1 and char2 then
            char1:MoveTo(char2.Head.Position)
            end
            end
            getout(lplayer, game:GetService("Players")[v.Name])
        end
    end
    if string.sub(msg, 1, 8) == (prefix.."follow ") then
        for i,v in pairs(GetPlayer(string.sub(msg, 9))) do
            followed = true
            flwplr = v
        end
    end
    if string.sub(msg, 1, 9) == (prefix.."unfollow") then
        followed = false
    end
    if string.sub(msg, 1, 10) == (prefix.."freefall ") then
        for i,v in pairs(GetPlayer(string.sub(msg, 11))) do
            local NOW = lplayer.Character.HumanoidRootPart.CFrame
            lplayer.Character.Humanoid.Name = 1
            local l = lplayer.Character["1"]:Clone()
            l.Parent = lplayer.Character
            l.Name = "Humanoid"
            wait(0.1)
            lplayer.Character["1"]:Destroy()
            game:GetService("Workspace").CurrentCamera.CameraSubject = lplayer.Character
            lplayer.Character.Animate.Disabled = true
            wait(0.1)
            lplayer.Character.Animate.Disabled = false
            lplayer.Character.Humanoid.DisplayDistanceType = "None"
            for i,v in pairs(game:GetService'Players'.LocalPlayer.Backpack:GetChildren())do
            lplayer.Character.Humanoid:EquipTool(v)
            end
            lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character.HumanoidRootPart.CFrame
            wait(0.2)
            lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character.HumanoidRootPart.CFrame
            wait(0.6)
            lplayer.Character.HumanoidRootPart.CFrame = NOW
            wait(0.6)
            lplayer.Character.HumanoidRootPart.CFrame = CFrame.new(0,50000,0)
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Tools needed!";
            Text = "You need a tool in your backpack for this command!";
            })
        end
    end
    if string.sub(msg, 1, 7) == (prefix.."trail ") then
        for i,v in pairs(GetPlayer(string.sub(msg, 8))) do
            traill = true
            trlplr = v
        end
    end
    if string.sub(msg, 1, 8) == (prefix.."untrail") then
        traill = false
    end
    if string.sub(msg, 1, 7) == (prefix.."orbit ") then
        if string.sub(msg, 8) == "all" or string.sub(msg, 8) == "others" or string.sub(msg, 8) == "me" then
            lplayer.Character.HumanoidRootPart.CFrame = lplayer.Character.HumanoidRootPart.CFrame
        else
            for i,v in pairs(GetPlayer(string.sub(msg, 8))) do
                local o = Instance.new("RocketPropulsion")
                o.Parent = lplayer.Character.HumanoidRootPart
                o.Name = "Orbit"
                o.Target = game:GetService("Players")[v.Name].Character.HumanoidRootPart
                o:Fire()
                noclip = true
            end
        end
    end
    if string.sub(msg, 1, 8) == (prefix.."unorbit") then
        lplayer.Character.HumanoidRootPart.Orbit:Destroy()
        noclip = false
    end
    if string.sub(msg, 1, 7) == (prefix.."fling ") then
        if string.sub(msg, 8) == "all" or string.sub(msg, 8) == "others" or string.sub(msg, 8) == "me" then
            lplayer.Character.HumanoidRootPart.CFrame = lplayer.Character.HumanoidRootPart.CFrame
        else
            for i,v in pairs(GetPlayer(string.sub(msg, 8))) do
                local y = Instance.new("RocketPropulsion")
                y.Parent = lplayer.Character.HumanoidRootPart
                y.CartoonFactor = 1
                y.MaxThrust = 800000
                y.MaxSpeed = 1000
                y.ThrustP = 200000
                y.Name = "Fling"
                game:GetService("Workspace").CurrentCamera.CameraSubject = game:GetService("Players")[v.Name].Character.Head
                y.Target = game:GetService("Players")[v.Name].Character.HumanoidRootPart
                y:Fire()
                noclip = true
            end
        end
    end
    if string.sub(msg, 1, 8) == (prefix.."unfling") then
        noclip = false
        lplayer.Character.HumanoidRootPart.Fling:Destroy()
        game:GetService("Workspace").CurrentCamera.CameraSubject = lplayer.Character.Head
        wait(0.4)
        lplayer.Character.HumanoidRootPart.Fling:Destroy()
    end
    if string.sub(msg, 1, 8) == (prefix.."fecheck") then
        if game:GetService("Workspace").FilteringEnabled == true then
            warn("FE is Enabled (Filtering Enabled)")
            game:GetService("StarterGui"):SetCore("SendNotification", {
                Title = "FE is Enabled";
                Text = "Filtering Enabled. Enjoy using Reviz Admin!";
            })
        else
            warn("FE is Disabled (Filtering Disabled) Consider using a different admin script.")
            game:GetService("StarterGui"):SetCore("SendNotification", {
                Title = "FE is Disabled";
                Text = "Filtering Disabled. Consider using a different admin script.";
            })
        end
    end
    if string.sub(msg, 1, 6) == (prefix.."void ") then
        for i,v in pairs(GetPlayer(string.sub(msg, 7))) do
            lplayer.Character.Humanoid.Name = 1
            local l = lplayer.Character["1"]:Clone()
            l.Parent = lplayer.Character
            l.Name = "Humanoid"
            wait(0.1)
            lplayer.Character["1"]:Destroy()
            game:GetService("Workspace").CurrentCamera.CameraSubject = lplayer.Character
            lplayer.Character.Animate.Disabled = true
            wait(0.1)
            lplayer.Character.Animate.Disabled = false
            lplayer.Character.Humanoid.DisplayDistanceType = "None"
            for i,v in pairs(game:GetService'Players'.LocalPlayer.Backpack:GetChildren())do
            lplayer.Character.Humanoid:EquipTool(v)
            end
            lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character.HumanoidRootPart.CFrame
            wait(0.2)
            lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character.HumanoidRootPart.CFrame
            wait(0.6)
            lplayer.Character.HumanoidRootPart.CFrame = CFrame.new(999999999999999,0,999999999999999)
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Tools needed!";
            Text = "You need a tool in your backpack for this command!";
            })
        end
    end
    if string.sub(msg, 1, 7) == (prefix.."noclip") then
        noclip = true
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "Noclip enabled";
        Text = "Type ;clip to disable";
        })
    end
    if string.sub(msg, 1, 5) == (prefix.."clip") then
        noclip = false
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "Noclip disabled";
        Text = "Type ;noclip to enable";
        })
    end
    if string.sub(msg, 1, 7) == (prefix.."speed ") then
        lplayer.Character.Humanoid.WalkSpeed = (string.sub(msg, 8))
    end
    if string.sub(msg, 1, 4) == (prefix.."ws ") then
        lplayer.Character.Humanoid.WalkSpeed = (string.sub(msg, 5))
    end
    if string.sub(msg, 1, 11) == (prefix.."hipheight ") then
        lplayer.Character.Humanoid.HipHeight = (string.sub(msg, 12))
    end
    if string.sub(msg, 1, 4) == (prefix.."hh ") then
        lplayer.Character.Humanoid.HipHeight = (string.sub(msg, 5))
    end
    if string.sub(msg, 1, 11) == (prefix.."jumppower ") then
        lplayer.Character.Humanoid.JumpPower = (string.sub(msg, 12))
    end
    if string.sub(msg, 1, 4) == (prefix.."jp ") then
        lplayer.Character.Humanoid.JumpPower = (string.sub(msg, 5))
    end
    if string.sub(msg, 1, 8) == (prefix.."default") then
        lplayer.Character.Humanoid.JumpPower = 50
        lplayer.Character.Humanoid.WalkSpeed = 16
        lplayer.Character.Humanoid.HipHeight = 0
    end
    if string.sub(msg, 1, 7) == (prefix.."annoy ") then
        for i,v in pairs(GetPlayer(string.sub(msg, 8))) do
            annoying = true
            annplr = v
        end
    end
    if string.sub(msg, 1, 8) == (prefix.."unannoy") then
        annoying = false
    end
    if string.sub(msg, 1, 10) == (prefix.."headwalk ") then
        for i,v in pairs(GetPlayer(string.sub(msg, 11))) do
            hwalk = true
            hdwplr = v
        end
    end
    if string.sub(msg, 1, 11) == (prefix.."unheadwalk") then
        hwalk = false
    end
    if string.sub(msg, 1, 8) == (prefix.."nolimbs") then
        lplayer.Character["Left Leg"]:Destroy()
        lplayer.Character["Left Arm"]:Destroy()
        lplayer.Character["Right Leg"]:Destroy()
        lplayer.Character["Right Arm"]:Destroy()
    end
    if string.sub(msg, 1, 4) == (prefix.."god") then
        lplayer.Character.Humanoid.Name = 1
        local l = lplayer.Character["1"]:Clone()
        l.Parent = lplayer.Character
        l.Name = "Humanoid"
        wait(0.1)
        lplayer.Character["1"]:Destroy()
        game:GetService("Workspace").CurrentCamera.CameraSubject = lplayer.Character
        lplayer.Character.Animate.Disabled = true
        wait(0.1)
        lplayer.Character.Animate.Disabled = false
        lplayer.Character.Humanoid.DisplayDistanceType = "None"
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "FE Godmode enabled";
        Text = "Use ;grespawn or ;respawn to remove";
        })
    end
    if string.sub(msg, 1, 9) == (prefix.."drophats") then
        for i,v in pairs(lplayer.Character:GetChildren()) do
            if (v:IsA("Accessory")) or (v:IsA("Hat")) then
                v.Parent = workspace
            end
        end
    end
    if string.sub(msg, 1, 9) == (prefix.."droptool") then
        for i,v in pairs(lplayer.Character:GetChildren()) do
            if (v:IsA("Tool")) then
                v.Parent = workspace
            end
        end
    end
    if string.sub(msg, 1, 10) == (prefix.."loopdhats") then
        droppinghats = true
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "Loop Drop Enabled";
        Text = "Type ;unloopdhats to disable";
        })
    end
    if string.sub(msg, 1, 12) == (prefix.."unloopdhats") then
        droppinghats = false
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "Loop Drop Disabled";
        Text = "Type ;loopdhats to enable.";
        })
    end
    if string.sub(msg, 1, 10) == (prefix.."loopdtool") then
        droppingtools = true
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "Loop Drop Enabled";
        Text = "Type ;unloopdtool to disable";
        })
    end
    if string.sub(msg, 1, 12) == (prefix.."unloopdtool") then
        droppingtools = false
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "Loop Drop Disabled";
        Text = "Type ;loopdtool to enable.";
        })
    end
    if string.sub(msg, 1, 10) == (prefix.."invisible") then -- Credit to Timeless
        Local = game:GetService('Players').LocalPlayer
        Char  = Local.Character
        touched,tpdback = false, false
        box = Instance.new('Part',workspace)
        box.Anchored = true
        box.CanCollide = true
        box.Size = Vector3.new(10,1,10)
        box.Position = Vector3.new(0,10000,0)
        box.Touched:connect(function(part)
            if (part.Parent.Name == Local.Name) then
                if touched == false then
                    touched = true
                    function apply()
                        if script.Disabled ~= true then
                            no = Char.HumanoidRootPart:Clone()
                            wait(.25)
                            Char.HumanoidRootPart:Destroy()
                            no.Parent = Char
                            Char:MoveTo(loc)
                            touched = false
                        end end
                    if Char then
                        apply()
                    end
                end
            end
        end)
        repeat wait() until Char
        loc = Char.HumanoidRootPart.Position
        Char:MoveTo(box.Position + Vector3.new(0,.5,0))
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "Invisibility enabled!";
        Text = "Reset or use ;respawn to remove.";
        })
    end
    if string.sub(msg, 1, 6) == (prefix.."view ") then
        for i,v in pairs(GetPlayer(string.sub(msg, 7))) do
            if game:GetService("Players")[v.Name].Character.Humanoid then
                game:GetService("Workspace").CurrentCamera.CameraSubject = game:GetService("Players")[v.Name].Character.Humanoid
            else
                game:GetService("Workspace").CurrentCamera.CameraSubject = game:GetService("Players")[v.Name].Character.Head
            end
        end
    end
    if string.sub(msg, 1, 7) == (prefix.."unview") then
        if lplayer.Character.Humanoid then
            game:GetService("Workspace").CurrentCamera.CameraSubject = lplayer.Character.Humanoid
        else
            game:GetService("Workspace").CurrentCamera.CameraSubject = lplayer.Character.Head
        end
    end
    if string.sub(msg, 1, 6) == (prefix.."goto ") then
        for i,v in pairs(GetPlayer(string.sub(msg, 7))) do
            lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character.HumanoidRootPart.CFrame
        end
    end
    if string.sub(msg, 1, 4) == (prefix.."fly") then
    repeat wait() until lplayer and lplayer.Character and lplayer.Character:FindFirstChild('HumanoidRootPart') and lplayer.Character:FindFirstChild('Humanoid')
    repeat wait() until Mouse
   
    local T = lplayer.Character.HumanoidRootPart
    local CONTROL = {F = 0, B = 0, L = 0, R = 0}
    local lCONTROL = {F = 0, B = 0, L = 0, R = 0}
    local SPEED = speedget
   
    local function fly()
        flying = true
        local BG = Instance.new('BodyGyro', T)
        local BV = Instance.new('BodyVelocity', T)
        BG.P = 9e4
        BG.maxTorque = Vector3.new(9e9, 9e9, 9e9)
        BG.cframe = T.CFrame
        BV.velocity = Vector3.new(0, 0.1, 0)
        BV.maxForce = Vector3.new(9e9, 9e9, 9e9)
        spawn(function()
        repeat wait()
        lplayer.Character.Humanoid.PlatformStand = true
        if CONTROL.L + CONTROL.R ~= 0 or CONTROL.F + CONTROL.B ~= 0 then
        SPEED = 50
        elseif not (CONTROL.L + CONTROL.R ~= 0 or CONTROL.F + CONTROL.B ~= 0) and SPEED ~= 0 then
        SPEED = 0
        end
        if (CONTROL.L + CONTROL.R) ~= 0 or (CONTROL.F + CONTROL.B) ~= 0 then
        BV.velocity = ((workspace.CurrentCamera.CoordinateFrame.lookVector * (CONTROL.F + CONTROL.B)) + ((workspace.CurrentCamera.CoordinateFrame * CFrame.new(CONTROL.L + CONTROL.R, (CONTROL.F + CONTROL.B) * 0.2, 0).p) - workspace.CurrentCamera.CoordinateFrame.p)) * SPEED
        lCONTROL = {F = CONTROL.F, B = CONTROL.B, L = CONTROL.L, R = CONTROL.R}
        elseif (CONTROL.L + CONTROL.R) == 0 and (CONTROL.F + CONTROL.B) == 0 and SPEED ~= 0 then
        BV.velocity = ((workspace.CurrentCamera.CoordinateFrame.lookVector * (lCONTROL.F + lCONTROL.B)) + ((workspace.CurrentCamera.CoordinateFrame * CFrame.new(lCONTROL.L + lCONTROL.R, (lCONTROL.F + lCONTROL.B) * 0.2, 0).p) - workspace.CurrentCamera.CoordinateFrame.p)) * SPEED
        else
        BV.velocity = Vector3.new(0, 0.1, 0)
        end
        BG.cframe = workspace.CurrentCamera.CoordinateFrame
                until not flying
                CONTROL = {F = 0, B = 0, L = 0, R = 0}
                lCONTROL = {F = 0, B = 0, L = 0, R = 0}
                SPEED = 0
                BG:destroy()
                BV:destroy()
                lplayer.Character.Humanoid.PlatformStand = false
            end)
        end
    Mouse.KeyDown:connect(function(KEY)
        if KEY:lower() == 'w' then
            CONTROL.F = speedfly
        elseif KEY:lower() == 's' then
            CONTROL.B = -speedfly
        elseif KEY:lower() == 'a' then
            CONTROL.L = -speedfly
        elseif KEY:lower() == 'd' then
            CONTROL.R = speedfly
        end
    end)
    Mouse.KeyUp:connect(function(KEY)
        if KEY:lower() == 'w' then
            CONTROL.F = 0
        elseif KEY:lower() == 's' then
            CONTROL.B = 0
        elseif KEY:lower() == 'a' then
            CONTROL.L = 0
        elseif KEY:lower() == 'd' then
            CONTROL.R = 0
        end
    end)
    fly()
    end
    if string.sub(msg, 1, 6) == (prefix.."unfly") then
        flying = false
        lplayer.Character.Humanoid.PlatformStand = false
    end
    if string.sub(msg, 1, 6) == (prefix.."chat ") then
        game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer((string.sub(msg, 7)), "All")
    end
    if string.sub(msg, 1, 6) == (prefix.."spam ") then
        spamtext = (string.sub(msg, 7))
        spamming = true
    end
    if string.sub(msg, 1, 7) == (prefix.."unspam") then
        spamming = false
    end
    if string.sub(msg, 1, 10) == (prefix.."spamwait ") then
        spamdelay = (string.sub(msg, 11))
    end
    if string.sub(msg, 1, 8) == (prefix.."pmspam ") then
        for i,v in pairs(GetPlayer(string.sub(msg, 9))) do
            pmspammed = v.Name
            spammingpm = true
        end
    end
    if string.sub(msg, 1, 9) == (prefix.."unpmspam") then
        spammingpm = false
    end
    if string.sub(msg, 1, 9) == (prefix.."cfreeze ") then
        for i,v in pairs(GetPlayer(string.sub(msg, 10))) do
            v.Character["Left Leg"].Anchored = true
            v.Character["Left Arm"].Anchored = true
            v.Character["Right Leg"].Anchored = true
            v.Character["Right Arm"].Anchored = true
            v.Character.Torso.Anchored = true
            v.Character.Head.Anchored = true
        end
    end
    if string.sub(msg, 1, 11) == (prefix.."uncfreeze ") then
        for i,v in pairs(GetPlayer(string.sub(msg, 12))) do
            v.Character["Left Leg"].Anchored = false
            v.Character["Left Arm"].Anchored = false
            v.Character["Right Leg"].Anchored = false
            v.Character["Right Arm"].Anchored = false
            v.Character.Torso.Anchored = false
            v.Character.Head.Anchored = false
        end
    end
    if string.sub(msg, 1, 9) == (prefix.."unlockws") then
        local a = game:GetService("Workspace"):getChildren()
        for i = 1, #a do
            if a[i].className == "Part" then
                a[i].Locked = false
            elseif a[i].className == "Model" then
                local r = a[i]:getChildren()
                for i = 1, #r do
                    if r[i].className == "Part" then
                    r[i].Locked = false
                    end
                end
            end
        end
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "Success!";
        Text = "Workspace unlocked. Use ;lockws to lock.";
        })
    end
    if string.sub(msg, 1, 7) == (prefix.."lockws") then
        local a = game:GetService("Workspace"):getChildren()
        for i = 1, #a do
            if a[i].className == "Part" then
                a[i].Locked = true
            elseif a[i].className == "Model" then
                local r = a[i]:getChildren()
                for i = 1, #r do
                    if r[i].className == "Part" then
                    r[i].Locked = true
                    end
                end
            end
        end
    end
    if string.sub(msg, 1, 7) == (prefix.."btools") then
        local Clone_T = Instance.new("HopperBin",lplayer.Backpack)
        Clone_T.BinType = "Clone"
        local Destruct = Instance.new("HopperBin",lplayer.Backpack)
        Destruct.BinType = "Hammer"
        local Hold_T = Instance.new("HopperBin",lplayer.Backpack)
        Hold_T.BinType = "Grab"
    end
    if string.sub(msg, 1, 7) == (prefix.."pstand") then
        lplayer.Character.Humanoid.PlatformStand = true
    end
    if string.sub(msg, 1, 9) == (prefix.."unpstand") then
        lplayer.Character.Humanoid.PlatformStand = false
    end
    if string.sub(msg, 1, 10) == (prefix.."blockhead") then
        lplayer.Character.Head.Mesh:Destroy()
    end
    if string.sub(msg, 1, 4) == (prefix.."sit") then
        lplayer.Character.Humanoid.Sit = true
    end
    if string.sub(msg, 1, 10) == (prefix.."bringobj ") then
        local function bringobjw()
        for i,obj in ipairs(game:GetService("Workspace"):GetDescendants()) do
        if obj.Name == (string.sub(msg, 11)) then
        obj.CFrame = lplayer.Character.HumanoidRootPart.CFrame
        obj.CanCollide = false
        obj.Transparency = 0.7
        wait()
        obj.CFrame = lplayer.Character["Left Leg"].CFrame
        wait()
        obj.CFrame = lplayer.Character["Right Leg"].CFrame
        wait()
        obj.CFrame = lplayer.Character["Head"].CFrame
        end
        end
        end
        while wait() do
            bringobjw()
        end
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "BringObj";
        Text = "BringObj enabled.";
        })
    end
    if string.sub(msg, 1, 7) == (prefix.."wsvis ") then
        vis = (string.sub(msg, 8))
        local a = game:GetService("Workspace"):GetDescendants()
        for i = 1, #a do
            if a[i].className == "Part" then
                a[i].Transparency = vis
            elseif a[i].className == "Model" then
                local r = a[i]:getChildren()
                for i = 1, #r do
                    if r[i].className == "Part" then
                    r[i].Transparency = vis
                    end
                end
            end
        end
    end
    if string.sub(msg, 1, 11) == (prefix.."hypertotal") then
        loadstring(game:GetObjects("rbxassetid://1255063809")[1].Source)()
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "Success!";
        Text = "HyperTotal GUI Loaded!";
        })
    end
    if string.sub(msg, 1, 5) == (prefix.."cmds") then
        CMDSFRAME.Visible = true
    end
    if string.sub(msg, 1, 10) == (prefix.."rmeshhats") then
        for i,v in pairs(lplayer.Character:GetChildren()) do
            if (v:IsA("Accessory")) or (v:IsA("Hat")) then
                v.Handle.Mesh:Destroy()
            end
        end
    end
    if string.sub(msg, 1, 10) == (prefix.."blockhats") then
        for i,v in pairs(lplayer.Character:GetChildren()) do
            if (v:IsA("Accessory")) or (v:IsA("Hat")) then
                v.Handle.Mesh:Destroy()
            end
        end
    end
    if string.sub(msg, 1, 10) == (prefix.."rmeshtool") then
        for i,v in pairs(lplayer.Character:GetChildren()) do
            if (v:IsA("Tool")) then
                v.Handle.Mesh:Destroy()
            end
        end
    end
    if string.sub(msg, 1, 10) == (prefix.."blocktool") then
        for i,v in pairs(lplayer.Character:GetChildren()) do
            if (v:IsA("Tool")) then
                v.Handle.Mesh:Destroy()
            end
        end
    end
    if string.sub(msg, 1, 8) == (prefix.."spinner") then
        local p = Instance.new("RocketPropulsion")
        p.Parent = lplayer.Character.HumanoidRootPart
        p.Name = "Spinner"
        p.Target = lplayer.Character["Left Arm"]
        p:Fire()
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "Spinner enabled";
        Text = "Type ;nospinner to disable.";
        })
    end
    if string.sub(msg, 1, 10) == (prefix.."nospinner") then
        lplayer.Character.HumanoidRootPart.Spinner:Destroy()
    end
    if string.sub(msg, 1, 7) == (prefix.."reachd") then
        for i,v in pairs(game:GetService'Players'.LocalPlayer.Character:GetChildren())do
            if v:isA("Tool") then
                local a = Instance.new("SelectionBox",v.Handle)
                a.Adornee = v.Handle
                v.Handle.Size = Vector3.new(0.5,0.5,60)
                v.GripPos = Vector3.new(0,0,0)
                lplayer.Character.Humanoid:UnequipTools()
            end
        end
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "Reach applied!";
        Text = "Applied to equipped sword. Use ;noreach to disable.";
        })
    end
    if string.sub(msg, 1, 7) == (prefix.."reach ") then
        for i,v in pairs(game:GetService'Players'.LocalPlayer.Character:GetChildren())do
            if v:isA("Tool") then
                handleSize = v.Handle.Size
                wait()
                local a = Instance.new("SelectionBox",v.Handle)
                a.Name = "a"
                a.Adornee = v.Handle
                v.Handle.Size = Vector3.new(0.5,0.5,(string.sub(msg, 8)))
                v.GripPos = Vector3.new(0,0,0)
                lplayer.Character.Humanoid:UnequipTools()
            end
        end
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "Reach applied!";
        Text = "Applied to equipped sword. Use ;noreach to disable.";
        })
    end
    if string.sub(msg, 1, 8) == (prefix.."noreach") then
        for i,v in pairs(game:GetService'Players'.LocalPlayer.Character:GetChildren())do
            if v:isA("Tool") then
                v.Handle.a:Destroy()
                v.Handle.Size = handleSize
            end
        end
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "Reach removed!";
        Text = "Removed reach from equipped sword.";
        })
    end
    if string.sub(msg, 1, 7) == (prefix.."rkill ") then
        for i,v in pairs(GetPlayer(string.sub(msg, 8)))do
            lplayer.Character.Humanoid.Name = 1
            local l = lplayer.Character["1"]:Clone()
            l.Parent = lplayer.Character
            l.Name = "Humanoid"
            wait(0.1)
            lplayer.Character["1"]:Destroy()
            game:GetService("Workspace").CurrentCamera.CameraSubject = lplayer.Character
            lplayer.Character.Animate.Disabled = true
            wait(0.1)
            lplayer.Character.Animate.Disabled = false
            lplayer.Character.Humanoid.DisplayDistanceType = "None"
            for i,v in pairs(game:GetService'Players'.LocalPlayer.Backpack:GetChildren())do
            lplayer.Character.Humanoid:EquipTool(v)
            end
            wait(0.1)
            lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character.HumanoidRootPart.CFrame
            wait(0.2)
            lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character.HumanoidRootPart.CFrame
            wait(0.5)
            lplayer.Character.HumanoidRootPart.CFrame = CFrame.new(Vector3.new(-100000,10,-100000))
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Tools needed!";
            Text = "You need a tool in your backpack for this command!";
            })
        end
    end
    if string.sub(msg, 1, 7) == (prefix.."tp me ") then
        for i,v in pairs(GetPlayer(string.sub(msg, 8))) do
            lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character.HumanoidRootPart.CFrame
        end
    end
    if string.sub(msg, 1, 8) == (prefix.."cbring ") then
        if (string.sub(msg, 9)) == "all" or (string.sub(msg, 9)) == "All" or (string.sub(msg, 9)) == "ALL" then
            cbringall = true
        else
            for i,v in pairs(GetPlayer(string.sub(msg, 9))) do
                brplr = v.Name
            end
        end
        cbring = true
    end
    if string.sub(msg, 1, 9) == (prefix.."uncbring") then
        cbring = false
        cbringall = false
    end
    if string.sub(msg, 1, 6) == (prefix.."swap ") then
        for i,v in pairs(GetPlayer(string.sub(msg, 7))) do
            local NOWPLR = game:GetService("Players")[v.Name].Character.HumanoidRootPart.CFrame
            local NOW = lplayer.Character.HumanoidRootPart.CFrame
            lplayer.Character.Humanoid.Name = 1
            local l = lplayer.Character["1"]:Clone()
            l.Parent = lplayer.Character
            l.Name = "Humanoid"
            wait(0.1)
            lplayer.Character["1"]:Destroy()
            game:GetService("Workspace").CurrentCamera.CameraSubject = lplayer.Character
            lplayer.Character.Animate.Disabled = true
            wait(0.1)
            lplayer.Character.Animate.Disabled = false
            lplayer.Character.Humanoid.DisplayDistanceType = "None"
            for i,v in pairs(game:GetService'Players'.LocalPlayer.Backpack:GetChildren())do
            lplayer.Character.Humanoid:EquipTool(v)
            end
            local function tp(player,player2)
            local char1,char2=player.Character,player2.Character
            if char1 and char2 then
            char1:MoveTo(char2.Head.Position)
            end
            end
            wait(0.1)
            lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character.HumanoidRootPart.CFrame
            wait(0.2)
            lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character.HumanoidRootPart.CFrame
            wait(0.5)
            lplayer.Character.HumanoidRootPart.CFrame = NOW
            wait(0.6)
            tp(lplayer, game:GetService("Players")[v.Name])
            wait(0.4)
            lplayer.Character.HumanoidRootPart.CFrame = NOWPLR
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Tools needed!";
            Text = "You need a tool in your backpack for this command!";
            })
        end
    end
    if string.sub(msg, 1, 8) == (prefix.."glitch ") then
        for i,v in pairs(GetPlayer(string.sub(msg, 9))) do
            lplayer.Character.Humanoid.Name = 1
            local l = lplayer.Character["1"]:Clone()
            l.Parent = lplayer.Character
            l.Name = "Humanoid"
            wait(0.1)
            lplayer.Character["1"]:Destroy()
            game:GetService("Workspace").CurrentCamera.CameraSubject = lplayer.Character
            lplayer.Character.Animate.Disabled = true
            wait(0.1)
            lplayer.Character.Animate.Disabled = false
            lplayer.Character.Humanoid.DisplayDistanceType = "None"
            for i,v in pairs(game:GetService'Players'.LocalPlayer.Backpack:GetChildren())do
            lplayer.Character.Humanoid:EquipTool(v)
            end
            lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character["Left Arm"].CFrame
            wait(0.3)
            lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character["Left Arm"].CFrame
            wait(0.4)
            b = Instance.new("BodyForce")
            b.Parent = lplayer.Character.HumanoidRootPart
            b.Name = "Glitch"
            b.Force = Vector3.new(100000000,5000,0)
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Tools needed!";
            Text = "You need a tool in your backpack for this command!";
            })
        end
    end
    if string.sub(msg, 1, 9) == (prefix.."unglitch") then
        lplayer.Character.HumanoidRootPart.Glitch:Destroy()
        lplayer.Character.HumanoidRootPart.CFrame = CFrame.new(10000,0,10000)
        b = Instance.new("BodyForce")
        b.Parent = lplayer.Character.HumanoidRootPart
        b.Name = "unGlitch"
        b.Force = Vector3.new(0,-5000000,0)
        wait(2)
        lplayer.Character.HumanoidRootPart.unGlitch:Destroy()
    end
    if string.sub(msg, 1, 9) == (prefix.."grespawn") then
        lplayer.Character.Humanoid.Health = 0
        wait(1)
        lplayer.Character.Head.CFrame = CFrame.new(1000000,0,1000000)
        lplayer.Character.Torso.CFrame = CFrame.new(1000000,0,1000000)
    end
    if string.sub(msg, 1, 9) == (prefix.."explorer") then
        loadstring(game:GetObjects("rbxassetid://492005721")[1].Source)()
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "Success!";
        Text = "DEX Explorer has loaded.";
        })
    end
    if string.sub(msg, 1, 6) == (prefix.."anim ") then
        local Anim = Instance.new("Animation")
        Anim.AnimationId = "rbxassetid://"..(string.sub(msg, 7))
        local track = lplayer.Character.Humanoid:LoadAnimation(Anim)
        track:Play(.1, 1, 1)
    end
    if string.sub(msg, 1, 8) == (prefix.."animgui") then
        loadstring(game:GetObjects("rbxassetid://1202558084")[1].Source)()
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "Success!";
        Text = "Energize Animations GUI has loaded.";
        })
    end
    if string.sub(msg, 1, 8) == (prefix.."savepos") then
        saved = lplayer.Character.HumanoidRootPart.CFrame
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "Position Saved";
        Text = "Use ;loadpos to return to saved position.";
        })
    end
    if string.sub(msg, 1, 8) == (prefix.."loadpos") then
        lplayer.Character.HumanoidRootPart.CFrame = saved
    end
    if string.sub(msg, 1, 6) == (prefix.."bang ") then
        for i,v in pairs(GetPlayer(string.sub(msg, 7))) do
            local Anim2 = Instance.new("Animation")
            Anim2.AnimationId = "rbxassetid://148840371"
            local track2 = lplayer.Character.Humanoid:LoadAnimation(Anim2)
            track2:Play(.1, 1, 1)
            bplrr = v.Name
            banpl = true
        end
    end
    if string.sub(msg, 1, 7) == (prefix.."unbang") then
        banpl = false
    end
    if string.sub(msg, 1, 10) == (prefix.."bringmod ") then
        local function bringmodw()
        for i,obj in ipairs(game:GetService("Workspace"):GetDescendants()) do
        if obj.Name == (string.sub(msg, 11)) then
        for i,ch in pairs(obj:GetDescendants()) do
        if (ch:IsA("BasePart")) then
        ch.CFrame = lplayer.Character.HumanoidRootPart.CFrame
        ch.CanCollide = false
        ch.Transparency = 0.7
        wait()
        ch.CFrame = lplayer.Character["Left Leg"].CFrame
        wait()
        ch.CFrame = lplayer.Character["Right Leg"].CFrame
        wait()
        ch.CFrame = lplayer.Character["Head"].CFrame
        end
        end
        end
        end
        end
        while wait() do
            bringmodw()
        end
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "BringMod";
        Text = "BringMod enabled.";
        })
    end
    if string.sub(msg, 1, 8) == (prefix.."respawn") then
        local mod = Instance.new('Model', workspace) mod.Name = 're '..lplayer.Name
        local hum = Instance.new('Humanoid', mod)
        local ins = Instance.new('Part', mod) ins.Name = 'Torso' ins.CanCollide = false ins.Transparency = 1
        lplayer.Character = mod
    end
    if string.sub(msg, 1, 9) == (prefix.."shutdown") then
        game:GetService'RunService'.Stepped:Connect(function()
        pcall(function()
            for i,v in pairs(game:GetService'Players':GetPlayers()) do
                if v.Character ~= nil and v.Character:FindFirstChild'Head' then
                    for _,x in pairs(v.Character.Head:GetChildren()) do
                        if x:IsA'Sound' then x.Playing = true x.CharacterSoundEvent:FireServer(true, true) end
                    end
                end
            end
        end)
        end)
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "Attempting Shutdown";
        Text = "Shutdown Attempt has begun.";
        })
    end
    if string.sub(msg, 1, 8) == (prefix.."delobj ") then
        objtodel = (string.sub(msg, 9))
        for i,v in pairs(game:GetService("Workspace"):GetDescendants()) do
            if v.Name == objtodel then
                v:Destroy()
            end
        end
    end
    if string.sub(msg, 1, 8) == (prefix.."getplrs") then
        for i,v in pairs(game:GetService("Players"):GetPlayers())do
            print(v)
        end
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "Printed";
        Text = "Players have been printed to console. (F9)";
        })
    end
    if string.sub(msg, 1, 9) == (prefix.."deldecal") then
        for i,v in pairs(game:GetService("Workspace"):GetDescendants())do
            if (v:IsA("Decal")) then
                v:Destroy()
            end
        end
    end
    if string.sub(msg, 1, 11) == (prefix.."opfinality") then
        loadstring(game:GetObjects("rbxassetid://1294358929")[1].Source)()
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "Success!";
        Text = "OpFinality GUI has loaded.";
        })
    end
    if string.sub(msg, 1, 8) == (prefix.."remotes") then
        remotes = true
        added = true
        game.DescendantAdded:connect(function(rmt)
        if added == true then
        if remotes == true then
        if rmt:IsA("RemoteEvent") then
        print("A RemoteEvent was added!")
        print(" game." .. rmt:GetFullName() .. " | RemoteEvent")
        print(" game." .. rmt:GetFullName() .. " | RemoteEvent", 247, 0, 0, true)
        end end end
        end)
        game.DescendantAdded:connect(function(rmtfnctn)
        if added == true then
        if remotes == true then
        if rmtfnctn:IsA("RemoteFunction") then
        warn("A RemoteFunction was added!")
        warn(" game." .. rmtfnctn:GetFullName() .. " | RemoteFunction")
        print(" game." .. rmtfnctn:GetFullName() .. " | RemoteFunction", 5, 102, 198, true)
        end end end
        end)
       
        game.DescendantAdded:connect(function(bndfnctn)
        if added == true then
        if binds == true then
        if bndfnctn:IsA("BindableFunction") then
        print("A BindableFunction was added!")
        print(" game." .. bndfnctn:GetFullName() .. " | BindableFunction")
        print(" game." .. bndfnctn:GetFullName() .. " | BindableFunction", 239, 247, 4, true)
        end end end
        end)
       
        game.DescendantAdded:connect(function(bnd)
        if added == true then
        if binds == true then
        if bnd:IsA("BindableEvent") then
        warn("A BindableEvent was added!")
        warn(" game." .. bnd:GetFullName() .. " | BindableEvent")
        print(" game." .. bnd:GetFullName() .. " | BindableEvent", 13, 193, 22, true)
        end end end
        end)
       
       
        if binds == true then
        for i,v in pairs(game:GetDescendants()) do
        if v:IsA("BindableFunction") then
        print(" game." .. v:GetFullName() .. " | BindableFunction")
        print(" game." .. v:GetFullName() .. " | BindableFunction", 239, 247, 4, true)
        end end
        for i,v in pairs(game:GetDescendants()) do
        if v:IsA("BindableEvent") then
        warn(" game." .. v:GetFullName() .. " | BindableEvent")
        print(" game." .. v:GetFullName() .. " | BindableEvent", 13, 193, 22, true)
        end end
        else
        print("Off")
        end
        if remotes == true then
        for i,v in pairs(game:GetDescendants()) do
        if v:IsA("RemoteFunction") then
        warn(" game." .. v:GetFullName() .. " | RemoteFunction")
        print(" game." .. v:GetFullName() .. " | RemoteFunction", 5, 102, 198, true)
        end end
        wait()
        for i,v in pairs(game:GetDescendants()) do
        if v:IsA("RemoteEvent") then
        print(" game." .. v:GetFullName() .. " | RemoteEvent")
        print(" game." .. v:GetFullName() .. " | RemoteEvent", 247, 0, 0, true)
        end end
        else
        print("Off")
        end
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "Printing Remotes";
        Text = "Type ;noremotes to disable.";
        })
    end
    if string.sub(msg, 1, 10) == (prefix.."noremotes") then
        remotes = false
        added = false
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "Printing Remotes Disabled";
        Text = "Type ;remotes to enable.";
        })
    end
    if string.sub(msg, 1, 10) == (prefix.."tpdefault") then
        spin = false
        followed = false
        traill = false
        noclip = false
        annoying = false
        hwalk = false
        cbringing = false
    end
    if string.sub(msg, 1, 8) == (prefix.."stopsit") then
        stopsitting = true
    end
    if string.sub(msg, 1, 6) == (prefix.."gosit") then
        stopsitting = false
    end
    if string.sub(msg, 1, 8) == (prefix.."version") then
        print(adminversion)
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "Version";
        Text = adminversion;
        })
    end
    if string.sub(msg, 1, 8) == (prefix.."clicktp") then
        clickgoto = true
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "Click TP";
        Text = "Press E to teleport to mouse position, ;noclicktp to stop";
        })
    end
    if string.sub(msg, 1, 9) == (prefix.."clickdel") then
        clickdel = true
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "Click Delete";
        Text = "Press E to delete part at mouse, ;noclickdel to stop";
        })
    end
    if string.sub(msg, 1, 11) == (prefix.."noclickdel") then
        clickdel = false
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "Click Delete";
        Text = "Click delete has been disabled.";
        })
    end
    if string.sub(msg, 1, 10) == (prefix.."noclicktp") then
        clickgoto = false
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "Click TP";
        Text = "Click TP has been disabled.";
        })
    end
    if string.sub(msg, 1, 8) == (prefix.."toolson") then
        gettingtools = true
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "Tools Enabled";
        Text = "Automatically colleting tools dropped.";
        })
    end
    if string.sub(msg, 1, 9) == (prefix.."toolsoff") then
        gettingtools = false
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "Tools Disabled";
        Text = "Click TP has been disabled.";
        })
    end
    if string.sub(msg, 1, 10) == (prefix.."delcmdbar") then
        ScreenGui:Destroy()
    end
    if string.sub(msg, 1, 6) == (prefix.."reset") then
        lplayer.Character.Head:Destroy()
    end
    if string.sub(msg, 1, 7) == (prefix.."state ") then
        statechosen = string.sub(msg, 8)
        changingstate = true
    end
    if string.sub(msg, 1, 9) == (prefix.."gravity ") then
        game:GetService("Workspace").Gravity = string.sub(msg, 10)
    end
    if string.sub(msg, 1, 10) == (prefix.."looprhats") then
        removingmeshhats = true
    end
    if string.sub(msg, 1, 12) == (prefix.."unlooprhats") then
        removingmeshhats = false
    end
    if string.sub(msg, 1, 10) == (prefix.."looprtool") then
        removingmeshtool = true
    end
    if string.sub(msg, 1, 12) == (prefix.."unlooprtool") then
        removingmeshtool = false
    end
    if string.sub(msg, 1, 10) == (prefix.."givetool ") then
        for i,v in pairs(game:GetService("Players").LocalPlayer.Character:GetDescendants()) do
            if v:IsA("Tool") then
                for i,player in pairs(GetPlayer(string.sub(msg, 11))) do
                    v.Parent = player.Character
                end
            end
        end
    end
    if string.sub(msg, 1, 14) == (prefix.."givealltools ") then
        for i,v in pairs(game:GetService("Players").LocalPlayer.Backpack:GetDescendants()) do
            if v:IsA("Tool") then
                v.Parent = lplayer.Character
                wait()
                for i,player in pairs(GetPlayer(string.sub(msg, 15))) do
                    v.Parent = player.Character
                end
            end
        end
    end
    if string.sub(msg, 1, 5) == (prefix.."age ") then
        for i,player in pairs(GetPlayer(string.sub(msg, 6))) do
            game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(player.Name.." Account Age: "..player.AccountAge.." days!", "All")
        end
    end
    if string.sub(msg, 1, 4) == (prefix.."id ") then
        for i,player in pairs(GetPlayer(string.sub(msg, 5))) do
            game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(player.Name.." Account ID: "..player.UserId, "All")
        end
    end
    if string.sub(msg, 1, 6) == (prefix..".age ") then
        for i,player in pairs(GetPlayer(string.sub(msg, 7))) do
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = player.AccountAge.." Days";
            Text = "Account age of "..player.Name;
            })
        end
    end
    if string.sub(msg, 1, 5) == (prefix..".id ") then
        for i,player in pairs(GetPlayer(string.sub(msg, 6))) do
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = player.UserId.." ID";
            Text = "Account ID of "..player.Name;
            })
        end
    end
    if string.sub(msg, 1, 7) == (prefix.."gameid") then
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "Game ID";
        Text = "Game ID: ".. game.GameId;
        })
    end
    if string.sub(msg, 1, 4) == (prefix.."pgs") then
        local pgscheck = game:GetService("Workspace"):PGSIsEnabled()
        if pgscheck == true then
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "PGSPhysicsSolverEnabled";
            Text = "PGS is Enabled!";
            })
        else
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "PGSPhysicsSolverEnabled";
            Text = "PGS is Disabled!";
            })
        end
    end
    if string.sub(msg, 1, 12) == (prefix.."removeinvis") then
        for i,v in pairs(game:GetService("Workspace"):GetDescendants()) do
            if v:IsA("Part") then
                if v.Transparency == 1 then
                    if v.Name ~= "HumanoidRootPart" then
                        v:Destroy()
                    end
                end
            end
        end
    end
    if string.sub(msg, 1, 10) == (prefix.."removefog") then
        game:GetService("Lighting").FogStart = 0
        game:GetService("Lighting").FogEnd = 9999999999999
    end
    if string.sub(msg, 1, 8) == (prefix.."disable") then
        lplayer.Character.Humanoid.Parent = lplayer
    end
    if string.sub(msg, 1, 7) == (prefix.."enable") then
        lplayer.Humanoid.Parent = lplayer.Character
    end
    if string.sub(msg, 1, 8) == (prefix.."prefix ") then
        prefix = (string.sub(msg, 9, 9))
        wait(0.1)
        change()
        wait(0.1)
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "Prefix changed!";
        Text = "Prefix is now "..prefix..". Use ;resetprefix to reset to ;";
        })
    end
    if string.sub(msg, 1, 12) == (";resetprefix") then
        prefix = ";"
        wait(0.1)
        change()
        wait(0.1)
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "Prefix changed!";
        Text = "Prefix is now "..prefix..". Make sure it's one key!";
        })
    end
    if string.sub(msg, 1, 10) == (prefix.."flyspeed ") then
        speedfly = string.sub(msg, 11)
        wait()
        change()
    end
    if string.sub(msg, 1, 8) == (prefix.."carpet ") then
        for i,v in pairs(GetPlayer(string.sub(msg, 9))) do
            local Anim3 = Instance.new("Animation")
            Anim3.AnimationId = "rbxassetid://282574440"
            local track3 = lplayer.Character.Humanoid:LoadAnimation(Anim3)
            track3:Play(.1, 1, 1)
            bplrr = v.Name
            banpl = true
        end
    end
    if string.sub(msg, 1, 9) == (prefix.."uncarpet") then
        banpl = false
    end
    if string.sub(msg, 1, 7) == (prefix.."stare ") then
        for i,v in pairs(GetPlayer(string.sub(msg, 8))) do
            staring = true
            stareplr = v
        end
    end
    if string.sub(msg, 1, 8) == (prefix.."unstare") then
        staring = false
    end
    if string.sub(msg, 1, 8) == (prefix.."logchat") then
        chatlogs = true
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "LogChat enabled";
        Text = "Now logging all player chat.";
        })
    end
    if string.sub(msg, 1, 10) == (prefix.."unlogchat") then
        chatlogs = false
        game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "LogChat disabled";
        Text = "Stopped logging all player chat.";
        })
    end
    if string.sub(msg, 1, 7) == (prefix.."fixcam") then
        game:GetService("Workspace").CurrentCamera:Destroy()
        wait(0.1)
        game:GetService("Workspace").CurrentCamera.CameraSubject = lplayer.Character.Humanoid
        game:GetService("Workspace").CurrentCamera.CameraType = "Custom"
        lplayer.CameraMinZoomDistance = 0.5
        lplayer.CameraMaxZoomDistance = 400
        lplayer.CameraMode = "Classic"
    end
    if string.sub(msg, 1, 8) == (prefix.."unstate") then
        changingstate = false
    end
end)
 
local function tp()
    for i, player in ipairs(game:GetService("Players"):GetPlayers()) do
        if player.Character and player.Character:FindFirstChild("HumanoidRootPart") then
            if player.Name == brplr then
                player.Character.HumanoidRootPart.CFrame = lplayer.Character.HumanoidRootPart.CFrame + lplayer.Character.HumanoidRootPart.CFrame.lookVector * 2
            end
        end
    end
end
local function tpall()
    for i, player in ipairs(game:GetService("Players"):GetPlayers()) do
        if player.Character and player.Character:FindFirstChild("HumanoidRootPart") then
            player.Character.HumanoidRootPart.CFrame = lplayer.Character.HumanoidRootPart.CFrame + lplayer.Character.HumanoidRootPart.CFrame.lookVector * 3
        end
    end
end
spawn(function()
    while wait(spamdelay) do
        if spamming == true then
            game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(spamtext, "All")
        end
    end
end)
spawn(function()
    while wait(spamdelay) do
        if spammingpm == true then
            game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer("/w "..pmspammed.." @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@", "All")
        end
    end
end)
spawn(function()
    while wait() do
        if cbring == true then
            tp()
        end
    end
end)
spawn(function()
    while wait() do
        if cbringall == true then
            tpall()
        end
    end
end)
 
Mouse.KeyDown:connect(function(Key)
    if Key == prefix then
        CMDBAR:CaptureFocus()
    end
end)
 
CMDBAR.FocusLost:connect(function(enterPressed)
    if enterPressed then
        if string.sub(CMDBAR.Text, 1, 5) == ("kill ") then
            if string.sub(CMDBAR.Text, 6) == "me" then
                lplayer.Character.HumanoidRootPart.CFrame = CFrame.new(100000,0,100000)
            else
                for i,v in pairs(GetPlayer(string.sub(CMDBAR.Text, 6)))do
                    local NOW = lplayer.Character.HumanoidRootPart.CFrame
                    lplayer.Character.Humanoid.Name = 1
                    local l = lplayer.Character["1"]:Clone()
                    l.Parent = lplayer.Character
                    l.Name = "Humanoid"
                    wait(0.1)
                    lplayer.Character["1"]:Destroy()
                    game:GetService("Workspace").CurrentCamera.CameraSubject = lplayer.Character
                    lplayer.Character.Animate.Disabled = true
                    wait(0.1)
                    lplayer.Character.Animate.Disabled = false
                    lplayer.Character.Humanoid.DisplayDistanceType = "None"
                    for i,v in pairs(game:GetService'Players'.LocalPlayer.Backpack:GetChildren())do
                    lplayer.Character.Humanoid:EquipTool(v)
                    end
                    local function tp(player,player2)
                    local char1,char2=player.Character,player2.Character
                    if char1 and char2 then
                    char1:MoveTo(char2.Head.Position)
                    end
                    end
                    wait(0.1)
                    lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character.HumanoidRootPart.CFrame
                    wait(0.2)
                    lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character.HumanoidRootPart.CFrame
                    wait(0.5)
                    lplayer.Character.HumanoidRootPart.CFrame = CFrame.new(Vector3.new(-100000,10,-100000))
                    wait(0.7)
                    tp(lplayer,game:GetService("Players")[v.Name])
                    wait(0.7)
                    lplayer.Character.HumanoidRootPart.CFrame = NOW
                    game:GetService("StarterGui"):SetCore("SendNotification", {
                    Title = "Tools needed!";
                    Text = "You need a tool in your backpack for this command!";
                    })
                end
            end
        end
        if string.sub(CMDBAR.Text, 1, 6) == ("bring ") then
            for i,v in pairs(GetPlayer(string.sub(CMDBAR.Text, 7)))do
                local NOW = lplayer.Character.HumanoidRootPart.CFrame
                lplayer.Character.Humanoid.Name = 1
                local l = lplayer.Character["1"]:Clone()
                l.Parent = lplayer.Character
                l.Name = "Humanoid"
                wait(0.1)
                lplayer.Character["1"]:Destroy()
                game:GetService("Workspace").CurrentCamera.CameraSubject = lplayer.Character
                lplayer.Character.Animate.Disabled = true
                wait(0.1)
                lplayer.Character.Animate.Disabled = false
                lplayer.Character.Humanoid.DisplayDistanceType = "None"
                for i,v in pairs(game:GetService'Players'.LocalPlayer.Backpack:GetChildren())do
                lplayer.Character.Humanoid:EquipTool(v)
                end
                local function tp(player,player2)
                local char1,char2=player.Character,player2.Character
                if char1 and char2 then
                char1.HumanoidRootPart.CFrame = char2.HumanoidRootPart.CFrame
                end
                end
                local function getout(player,player2)
                local char1,char2=player.Character,player2.Character
                if char1 and char2 then
                char1:MoveTo(char2.Head.Position)
                end
                end
                tp(game:GetService("Players")[v.Name], lplayer)
                wait(0.2)
                tp(game:GetService("Players")[v.Name], lplayer)
                wait(0.5)
                lplayer.Character.HumanoidRootPart.CFrame = NOW
                wait(0.5)
                getout(lplayer, game:GetService("Players")[v.Name])
                wait(0.3)
                lplayer.Character.HumanoidRootPart.CFrame = NOW
                game:GetService("StarterGui"):SetCore("SendNotification", {
                Title = "Tools needed!";
                Text = "You need a tool in your backpack for this command!";
                })
            end
        end
        if string.sub(CMDBAR.Text, 1, 5) == ("spin ") then
            for i,v in pairs(GetPlayer(string.sub(CMDBAR.Text, 6))) do
                lplayer.Character.Humanoid.Name = 1
                local l = lplayer.Character["1"]:Clone()
                l.Parent = lplayer.Character
                l.Name = "Humanoid"
                wait(0.1)
                lplayer.Character["1"]:Destroy()
                game:GetService("Workspace").CurrentCamera.CameraSubject = lplayer.Character
                lplayer.Character.Animate.Disabled = true
                wait(0.1)
                lplayer.Character.Animate.Disabled = false
                lplayer.Character.Humanoid.DisplayDistanceType = "None"
                for i,v in pairs(game:GetService'Players'.LocalPlayer.Backpack:GetChildren())do
                lplayer.Character.Humanoid:EquipTool(v)
                end
                lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character["Left Arm"].CFrame
                spinplr = v
                wait(0.5)
                spin = true
                game:GetService("StarterGui"):SetCore("SendNotification", {
                Title = "Tools needed!";
                Text = "You need a tool in your backpack for this command!";
                })
            end
        end
        if string.sub(CMDBAR.Text, 1, 6) == ("unspin") then
            spin = false
        end
        if string.sub(CMDBAR.Text, 1, 7) == ("attach ") then
            for i,v in pairs(GetPlayer(string.sub(CMDBAR.Text, 8))) do
                lplayer.Character.Humanoid.Name = 1
                local l = lplayer.Character["1"]:Clone()
                l.Parent = lplayer.Character
                l.Name = "Humanoid"
                wait(0.1)
                lplayer.Character["1"]:Destroy()
                game:GetService("Workspace").CurrentCamera.CameraSubject = lplayer.Character
                lplayer.Character.Animate.Disabled = true
                wait(0.1)
                lplayer.Character.Animate.Disabled = false
                lplayer.Character.Humanoid.DisplayDistanceType = "None"
                for i,v in pairs(game:GetService'Players'.LocalPlayer.Backpack:GetChildren())do
                lplayer.Character.Humanoid:EquipTool(v)
                end
                lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character["Left Arm"].CFrame
                wait(0.3)
                lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character["Left Arm"].CFrame
                attplr = v
                game:GetService("StarterGui"):SetCore("SendNotification", {
                Title = "Tools needed!";
                Text = "You need a tool in your backpack for this command!";
                })
            end
        end
        if string.sub(CMDBAR.Text, 1, 9) == ("unattach ") then
            for i,v in pairs(GetPlayer(string.sub(CMDBAR.Text, 10))) do
                local function getout(player,player2)
                local char1,char2=player.Character,player2.Character
                if char1 and char2 then
                char1:MoveTo(char2.Head.Position)
                end
                end
                getout(lplayer, game:GetService("Players")[v.Name])
            end
        end
        if string.sub(CMDBAR.Text, 1, 7) == ("follow ") then
            for i,v in pairs(GetPlayer(string.sub(CMDBAR.Text, 8))) do
                followed = true
                flwplr = v
            end
        end
        if string.sub(CMDBAR.Text, 1, 8) == ("unfollow") then
            followed = false
        end
        if string.sub(CMDBAR.Text, 1, 9) == ("freefall ") then
            for i,v in pairs(GetPlayer(string.sub(CMDBAR.Text, 10))) do
                local NOW = lplayer.Character.HumanoidRootPart.CFrame
                lplayer.Character.Humanoid.Name = 1
                local l = lplayer.Character["1"]:Clone()
                l.Parent = lplayer.Character
                l.Name = "Humanoid"
                wait(0.1)
                lplayer.Character["1"]:Destroy()
                game:GetService("Workspace").CurrentCamera.CameraSubject = lplayer.Character
                lplayer.Character.Animate.Disabled = true
                wait(0.1)
                lplayer.Character.Animate.Disabled = false
                lplayer.Character.Humanoid.DisplayDistanceType = "None"
                for i,v in pairs(game:GetService'Players'.LocalPlayer.Backpack:GetChildren())do
                lplayer.Character.Humanoid:EquipTool(v)
                end
                lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character.HumanoidRootPart.CFrame
                wait(0.2)
                lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character.HumanoidRootPart.CFrame
                wait(0.6)
                lplayer.Character.HumanoidRootPart.CFrame = NOW
                wait(0.6)
                lplayer.Character.HumanoidRootPart.CFrame = CFrame.new(0,50000,0)
                game:GetService("StarterGui"):SetCore("SendNotification", {
                Title = "Tools needed!";
                Text = "You need a tool in your backpack for this command!";
                })
            end
        end
        if string.sub(CMDBAR.Text, 1, 6) == ("trail ") then
            for i,v in pairs(GetPlayer(string.sub(CMDBAR.Text, 7))) do
                traill = true
                trlplr = v
            end
        end
        if string.sub(CMDBAR.Text, 1, 7) == ("untrail") then
            traill = false
        end
        if string.sub(CMDBAR.Text, 1, 6) == ("orbit ") then
            if string.sub(CMDBAR.Text, 7) == "all" or string.sub(CMDBAR.Text, 7) == "others" or string.sub(CMDBAR.Text, 7) == "me" then
                lplayer.Character.HumanoidRootPart.CFrame = lplayer.Character.HumanoidRootPart.CFrame
            else
                for i,v in pairs(GetPlayer(string.sub(CMDBAR.Text, 7))) do
                    local o = Instance.new("RocketPropulsion")
                    o.Parent = lplayer.Character.HumanoidRootPart
                    o.Name = "Orbit"
                    o.Target = game:GetService("Players")[v.Name].Character.HumanoidRootPart
                    o:Fire()
                    noclip = true
                end
            end
        end
        if string.sub(CMDBAR.Text, 1, 7) == ("unorbit") then
            lplayer.Character.HumanoidRootPart.Orbit:Destroy()
            noclip = false
        end
        if string.sub(CMDBAR.Text, 1, 6) == ("fling ") then
            if string.sub(CMDBAR.Text, 7) == "all" or string.sub(CMDBAR.Text, 7) == "others" or string.sub(CMDBAR.Text, 7) == "me" then
                lplayer.Character.HumanoidRootPart.CFrame = lplayer.Character.HumanoidRootPart.CFrame
            else
                for i,v in pairs(GetPlayer(string.sub(CMDBAR.Text, 7))) do
                    local y = Instance.new("RocketPropulsion")
                    y.Parent = lplayer.Character.HumanoidRootPart
                    y.CartoonFactor = 1
                    y.MaxThrust = 800000
                    y.MaxSpeed = 1000
                    y.ThrustP = 200000
                    y.Name = "Fling"
                    game:GetService("Workspace").CurrentCamera.CameraSubject = game:GetService("Players")[v.Name].Character.Head
                    y.Target = game:GetService("Players")[v.Name].Character.HumanoidRootPart
                    y:Fire()
                    noclip = true
                end
            end
        end
        if string.sub(CMDBAR.Text, 1, 7) == ("unfling") then
            noclip = false
            lplayer.Character.HumanoidRootPart.Fling:Destroy()
            game:GetService("Workspace").CurrentCamera.CameraSubject = lplayer.Character.Head
            wait(0.4)
            lplayer.Character.HumanoidRootPart.Fling:Destroy()
        end
        if string.sub(CMDBAR.Text, 1, 7) == ("fecheck") then
            if game:GetService("Workspace").FilteringEnabled == true then
                warn("FE is Enabled (Filtering Enabled)")
                game:GetService("StarterGui"):SetCore("SendNotification", {
                    Title = "FE is Enabled";
                    Text = "Filtering Enabled. Enjoy using Reviz Admin!";
                })
            else
                warn("FE is Disabled (Filtering Disabled) Consider using a different admin script.")
                game:GetService("StarterGui"):SetCore("SendNotification", {
                    Title = "FE is Disabled";
                    Text = "Filtering Disabled. Consider using a different admin script.";
                })
            end
        end
        if string.sub(CMDBAR.Text, 1, 5) == ("void ") then
            for i,v in pairs(GetPlayer(string.sub(CMDBAR.Text, 6))) do
                lplayer.Character.Humanoid.Name = 1
                local l = lplayer.Character["1"]:Clone()
                l.Parent = lplayer.Character
                l.Name = "Humanoid"
                wait(0.1)
                lplayer.Character["1"]:Destroy()
                game:GetService("Workspace").CurrentCamera.CameraSubject = lplayer.Character
                lplayer.Character.Animate.Disabled = true
                wait(0.1)
                lplayer.Character.Animate.Disabled = false
                lplayer.Character.Humanoid.DisplayDistanceType = "None"
                for i,v in pairs(game:GetService'Players'.LocalPlayer.Backpack:GetChildren())do
                lplayer.Character.Humanoid:EquipTool(v)
                end
                lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character.HumanoidRootPart.CFrame
                wait(0.2)
                lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character.HumanoidRootPart.CFrame
                wait(0.6)
                lplayer.Character.HumanoidRootPart.CFrame = CFrame.new(999999999999999,0,999999999999999)
                game:GetService("StarterGui"):SetCore("SendNotification", {
                Title = "Tools needed!";
                Text = "You need a tool in your backpack for this command!";
                })
            end
        end
        if string.sub(CMDBAR.Text, 1, 6) == ("noclip") then
            noclip = true
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Noclip enabled";
            Text = "Type ;clip to disable";
            })
        end
        if string.sub(CMDBAR.Text, 1, 4) == ("clip") then
            noclip = false
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Noclip disabled";
            Text = "Type ;noclip to enable";
            })
        end
        if string.sub(CMDBAR.Text, 1, 6) == ("speed ") then
            lplayer.Character.Humanoid.WalkSpeed = (string.sub(CMDBAR.Text, 7))
        end
        if string.sub(CMDBAR.Text, 1, 3) == ("ws ") then
            lplayer.Character.Humanoid.WalkSpeed = (string.sub(CMDBAR.Text, 4))
        end
        if string.sub(CMDBAR.Text, 1, 10) == ("hipheight ") then
            lplayer.Character.Humanoid.HipHeight = (string.sub(CMDBAR.Text, 11))
        end
        if string.sub(CMDBAR.Text, 1, 3) == ("hh ") then
            lplayer.Character.Humanoid.HipHeight = (string.sub(CMDBAR.Text, 4))
        end
        if string.sub(CMDBAR.Text, 1, 10) == ("jumppower ") then
            lplayer.Character.Humanoid.JumpPower = (string.sub(CMDBAR.Text, 11))
        end
        if string.sub(CMDBAR.Text, 1, 3) == ("jp ") then
            lplayer.Character.Humanoid.JumpPower = (string.sub(CMDBAR.Text, 4))
        end
        if string.sub(CMDBAR.Text, 1, 7) == ("default") then
            lplayer.Character.Humanoid.JumpPower = 50
            lplayer.Character.Humanoid.WalkSpeed = 16
            lplayer.Character.Humanoid.HipHeight = 0
        end
        if string.sub(CMDBAR.Text, 1, 6) == ("annoy ") then
            for i,v in pairs(GetPlayer(string.sub(CMDBAR.Text, 7))) do
                annoying = true
                annplr = v
            end
        end
        if string.sub(CMDBAR.Text, 1, 7) == ("unannoy") then
            annoying = false
        end
        if string.sub(CMDBAR.Text, 1, 9) == ("headwalk ") then
            for i,v in pairs(GetPlayer(string.sub(CMDBAR.Text, 10))) do
                hwalk = true
                hdwplr = v
            end
        end
        if string.sub(CMDBAR.Text, 1, 10) == ("unheadwalk") then
            hwalk = false
        end
        if string.sub(CMDBAR.Text, 1, 7) == ("nolimbs") then
            lplayer.Character["Left Leg"]:Destroy()
            lplayer.Character["Left Arm"]:Destroy()
            lplayer.Character["Right Leg"]:Destroy()
            lplayer.Character["Right Arm"]:Destroy()
        end
        if string.sub(CMDBAR.Text, 1, 3) == ("god") then
            lplayer.Character.Humanoid.Name = 1
            local l = lplayer.Character["1"]:Clone()
            l.Parent = lplayer.Character
            l.Name = "Humanoid"
            wait(0.1)
            lplayer.Character["1"]:Destroy()
            game:GetService("Workspace").CurrentCamera.CameraSubject = lplayer.Character
            lplayer.Character.Animate.Disabled = true
            wait(0.1)
            lplayer.Character.Animate.Disabled = false
            lplayer.Character.Humanoid.DisplayDistanceType = "None"
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "FE Godmode enabled";
            Text = "Use ;grespawn or ;respawn to remove.";
            })
        end
        if string.sub(CMDBAR.Text, 1, 8) == ("drophats") then
            for i,v in pairs(lplayer.Character:GetChildren()) do
                if (v:IsA("Accessory")) or (v:IsA("Hat")) then
                    v.Parent = workspace
                end
            end
        end
        if string.sub(CMDBAR.Text, 1, 8) == ("droptool") then
            for i,v in pairs(lplayer.Character:GetChildren()) do
                if (v:IsA("Tool")) then
                    v.Parent = workspace
                end
            end
        end
        if string.sub(CMDBAR.Text, 1, 9) == ("loopdhats") then
            droppinghats = true
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Loop Drop Enabled";
            Text = "Type ;unloopdhats to disable";
            })
        end
        if string.sub(CMDBAR.Text, 1, 11) == ("unloopdhats") then
            droppinghats = false
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Loop Drop Disabled";
            Text = "Type ;loopdhats to enable.";
            })
        end
        if string.sub(CMDBAR.Text, 1, 9) == ("loopdtool") then
            droppingtools = true
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Loop Drop Enabled";
            Text = "Type ;unloopdtool to disable";
            })
        end
        if string.sub(CMDBAR.Text, 1, 11) == ("unloopdtool") then
            droppingtools = false
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Loop Drop Disabled";
            Text = "Type ;loopdtool to enable.";
            })
        end
        if string.sub(CMDBAR.Text, 1, 9) == ("invisible") then -- Credit to Timeless
            Local = game:GetService('Players').LocalPlayer
            Char  = Local.Character
            touched,tpdback = false, false
            box = Instance.new('Part',workspace)
            box.Anchored = true
            box.CanCollide = true
            box.Size = Vector3.new(10,1,10)
            box.Position = Vector3.new(0,10000,0)
            box.Touched:connect(function(part)
                if (part.Parent.Name == Local.Name) then
                    if touched == false then
                        touched = true
                        function apply()
                            if script.Disabled ~= true then
                                no = Char.HumanoidRootPart:Clone()
                                wait(.25)
                                Char.HumanoidRootPart:Destroy()
                                no.Parent = Char
                                Char:MoveTo(loc)
                                touched = false
                            end end
                        if Char then
                            apply()
                        end
                    end
                end
            end)
            repeat wait() until Char
            loc = Char.HumanoidRootPart.Position
            Char:MoveTo(box.Position + Vector3.new(0,.5,0))
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Invisibility enabled!";
            Text = "Reset or use ;respawn to remove.";
            })
        end
        if string.sub(CMDBAR.Text, 1, 5) == ("view ") then
            for i,v in pairs(GetPlayer(string.sub(CMDBAR.Text, 6))) do
                if game:GetService("Players")[v.Name].Character.Humanoid then
                    game:GetService("Workspace").CurrentCamera.CameraSubject = game:GetService("Players")[v.Name].Character.Humanoid
                else
                    game:GetService("Workspace").CurrentCamera.CameraSubject = game:GetService("Players")[v.Name].Character.Head
                end
            end
        end
        if string.sub(CMDBAR.Text, 1, 6) == ("unview") then
            if lplayer.Character.Humanoid then
                game:GetService("Workspace").CurrentCamera.CameraSubject = lplayer.Character.Humanoid
            else
                game:GetService("Workspace").CurrentCamera.CameraSubject = lplayer.Character.Head
            end
        end
        if string.sub(CMDBAR.Text, 1, 5) == ("goto ") then
            for i,v in pairs(GetPlayer(string.sub(CMDBAR.Text, 6))) do
                lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character.HumanoidRootPart.CFrame
            end
        end
        if string.sub(CMDBAR.Text, 1, 3) == ("fly") then
        repeat wait() until lplayer and lplayer.Character and lplayer.Character:FindFirstChild('HumanoidRootPart') and lplayer.Character:FindFirstChild('Humanoid')
        repeat wait() until Mouse
       
        local T = lplayer.Character.HumanoidRootPart
        local CONTROL = {F = 0, B = 0, L = 0, R = 0}
        local lCONTROL = {F = 0, B = 0, L = 0, R = 0}
        local SPEED = speedget
       
        local function fly()
            flying = true
            local BG = Instance.new('BodyGyro', T)
            local BV = Instance.new('BodyVelocity', T)
            BG.P = 9e4
            BG.maxTorque = Vector3.new(9e9, 9e9, 9e9)
            BG.cframe = T.CFrame
            BV.velocity = Vector3.new(0, 0.1, 0)
            BV.maxForce = Vector3.new(9e9, 9e9, 9e9)
            spawn(function()
            repeat wait()
            lplayer.Character.Humanoid.PlatformStand = true
            if CONTROL.L + CONTROL.R ~= 0 or CONTROL.F + CONTROL.B ~= 0 then
            SPEED = 50
            elseif not (CONTROL.L + CONTROL.R ~= 0 or CONTROL.F + CONTROL.B ~= 0) and SPEED ~= 0 then
            SPEED = 0
            end
            if (CONTROL.L + CONTROL.R) ~= 0 or (CONTROL.F + CONTROL.B) ~= 0 then
            BV.velocity = ((workspace.CurrentCamera.CoordinateFrame.lookVector * (CONTROL.F + CONTROL.B)) + ((workspace.CurrentCamera.CoordinateFrame * CFrame.new(CONTROL.L + CONTROL.R, (CONTROL.F + CONTROL.B) * 0.2, 0).p) - workspace.CurrentCamera.CoordinateFrame.p)) * SPEED
            lCONTROL = {F = CONTROL.F, B = CONTROL.B, L = CONTROL.L, R = CONTROL.R}
            elseif (CONTROL.L + CONTROL.R) == 0 and (CONTROL.F + CONTROL.B) == 0 and SPEED ~= 0 then
            BV.velocity = ((workspace.CurrentCamera.CoordinateFrame.lookVector * (lCONTROL.F + lCONTROL.B)) + ((workspace.CurrentCamera.CoordinateFrame * CFrame.new(lCONTROL.L + lCONTROL.R, (lCONTROL.F + lCONTROL.B) * 0.2, 0).p) - workspace.CurrentCamera.CoordinateFrame.p)) * SPEED
            else
            BV.velocity = Vector3.new(0, 0.1, 0)
            end
            BG.cframe = workspace.CurrentCamera.CoordinateFrame
                    until not flying
                    CONTROL = {F = 0, B = 0, L = 0, R = 0}
                    lCONTROL = {F = 0, B = 0, L = 0, R = 0}
                    SPEED = 0
                    BG:destroy()
                    BV:destroy()
                    lplayer.Character.Humanoid.PlatformStand = false
                end)
            end
        Mouse.KeyDown:connect(function(KEY)
            if KEY:lower() == 'w' then
                CONTROL.F = speedfly
            elseif KEY:lower() == 's' then
                CONTROL.B = -speedfly
            elseif KEY:lower() == 'a' then
                CONTROL.L = -speedfly
            elseif KEY:lower() == 'd' then
                CONTROL.R = speedfly
            end
        end)
        Mouse.KeyUp:connect(function(KEY)
            if KEY:lower() == 'w' then
                CONTROL.F = 0
            elseif KEY:lower() == 's' then
                CONTROL.B = 0
            elseif KEY:lower() == 'a' then
                CONTROL.L = 0
            elseif KEY:lower() == 'd' then
                CONTROL.R = 0
            end
        end)
        fly()
        end
        if string.sub(CMDBAR.Text, 1, 5) == ("unfly") then
            flying = false
            lplayer.Character.Humanoid.PlatformStand = false
        end
        if string.sub(CMDBAR.Text, 1, 5) == ("chat ") then
            game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer((string.sub(CMDBAR.Text, 6)), "All")
        end
        if string.sub(CMDBAR.Text, 1, 5) == ("spam ") then
            spamtext = (string.sub(CMDBAR.Text, 6))
            spamming = true
        end
        if string.sub(CMDBAR.Text, 1, 6) == ("unspam") then
            spamming = false
        end
        if string.sub(CMDBAR.Text, 1, 9) == ("spamwait ") then
            spamdelay = (string.sub(CMDBAR.Text, 10))
        end
        if string.sub(CMDBAR.Text, 1, 7) == ("pmspam ") then
            for i,v in pairs(GetPlayer(string.sub(CMDBAR.Text, 8))) do
                pmspammed = v.Name
                spammingpm = true
            end
        end
        if string.sub(CMDBAR.Text, 1, 8) == ("unpmspam") then
            spammingpm = false
        end
        if string.sub(CMDBAR.Text, 1, 8) == ("cfreeze ") then
            for i,v in pairs(GetPlayer(string.sub(CMDBAR.Text, 9))) do
                v.Character["Left Leg"].Anchored = true
                v.Character["Left Arm"].Anchored = true
                v.Character["Right Leg"].Anchored = true
                v.Character["Right Arm"].Anchored = true
                v.Character.Torso.Anchored = true
                v.Character.Head.Anchored = true
            end
        end
        if string.sub(CMDBAR.Text, 1, 10) == ("uncfreeze ") then
            for i,v in pairs(GetPlayer(string.sub(CMDBAR.Text, 11))) do
                v.Character["Left Leg"].Anchored = false
                v.Character["Left Arm"].Anchored = false
                v.Character["Right Leg"].Anchored = false
                v.Character["Right Arm"].Anchored = false
                v.Character.Torso.Anchored = false
                v.Character.Head.Anchored = false
            end
        end
        if string.sub(CMDBAR.Text, 1, 8) == ("unlockws") then
            local a = game:GetService("Workspace"):getChildren()
            for i = 1, #a do
                if a[i].className == "Part" then
                    a[i].Locked = false
                elseif a[i].className == "Model" then
                    local r = a[i]:getChildren()
                    for i = 1, #r do
                        if r[i].className == "Part" then
                        r[i].Locked = false
                        end
                    end
                end
            end
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Success!";
            Text = "Workspace unlocked. Use ;lockws to lock.";
            })
        end
        if string.sub(CMDBAR.Text, 1, 6) == ("lockws") then
            local a = game:GetService("Workspace"):getChildren()
            for i = 1, #a do
                if a[i].className == "Part" then
                    a[i].Locked = true
                elseif a[i].className == "Model" then
                    local r = a[i]:getChildren()
                    for i = 1, #r do
                        if r[i].className == "Part" then
                        r[i].Locked = true
                        end
                    end
                end
            end
        end
        if string.sub(CMDBAR.Text, 1, 6) == ("btools") then
            local Clone_T = Instance.new("HopperBin",lplayer.Backpack)
            Clone_T.BinType = "Clone"
            local Destruct = Instance.new("HopperBin",lplayer.Backpack)
            Destruct.BinType = "Hammer"
            local Hold_T = Instance.new("HopperBin",lplayer.Backpack)
            Hold_T.BinType = "Grab"
        end
        if string.sub(CMDBAR.Text, 1, 6) == ("pstand") then
            lplayer.Character.Humanoid.PlatformStand = true
        end
        if string.sub(CMDBAR.Text, 1, 8) == ("unpstand") then
            lplayer.Character.Humanoid.PlatformStand = false
        end
        if string.sub(CMDBAR.Text, 1, 9) == ("blockhead") then
            lplayer.Character.Head.Mesh:Destroy()
        end
        if string.sub(CMDBAR.Text, 1, 3) == ("sit") then
            lplayer.Character.Humanoid.Sit = true
        end
        if string.sub(CMDBAR.Text, 1, 9) == ("bringobj ") then
            local function bringobjw()
            for i,obj in ipairs(game:GetService("Workspace"):GetDescendants()) do
            if obj.Name == (string.sub(CMDBAR.Text, 10)) then
            obj.CFrame = lplayer.Character.HumanoidRootPart.CFrame
            obj.CanCollide = false
            obj.Transparency = 0.7
            wait()
            obj.CFrame = lplayer.Character["Left Leg"].CFrame
            wait()
            obj.CFrame = lplayer.Character["Right Leg"].CFrame
            wait()
            obj.CFrame = lplayer.Character["Head"].CFrame
            end
            end
            end
            while wait() do
                bringobjw()
            end
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "BringObj";
            Text = "BringObj enabled.";
            })
        end
        if string.sub(CMDBAR.Text, 1, 6) == ("wsvis ") then
            vis = (string.sub(CMDBAR.Text, 7))
            local a = game:GetService("Workspace"):GetDescendants()
            for i = 1, #a do
                if a[i].className == "Part" then
                    a[i].Transparency = vis
                elseif a[i].className == "Model" then
                    local r = a[i]:getChildren()
                    for i = 1, #r do
                        if r[i].className == "Part" then
                        r[i].Transparency = vis
                        end
                    end
                end
            end
        end
        if string.sub(CMDBAR.Text, 1, 10) == ("hypertotal") then
            loadstring(game:GetObjects("rbxassetid://1255063809")[1].Source)()
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Success!";
            Text = "HyperTotal GUI Loaded!";
            })
        end
        if string.sub(CMDBAR.Text, 1, 4) == ("cmds") then
            CMDSFRAME.Visible = true
        end
        if string.sub(CMDBAR.Text, 1, 9) == ("rmeshhats") then
            for i,v in pairs(lplayer.Character:GetChildren()) do
                if (v:IsA("Accessory")) or (v:IsA("Hat")) then
                    v.Handle.Mesh:Destroy()
                end
            end
        end
        if string.sub(CMDBAR.Text, 1, 9) == ("blockhats") then
            for i,v in pairs(lplayer.Character:GetChildren()) do
                if (v:IsA("Accessory")) or (v:IsA("Hat")) then
                    v.Handle.Mesh:Destroy()
                end
            end
        end
        if string.sub(CMDBAR.Text, 1, 9) == ("rmeshtool") then
            for i,v in pairs(lplayer.Character:GetChildren()) do
                if (v:IsA("Tool")) then
                    v.Handle.Mesh:Destroy()
                end
            end
        end
        if string.sub(CMDBAR.Text, 1, 9) == ("blocktool") then
            for i,v in pairs(lplayer.Character:GetChildren()) do
                if (v:IsA("Tool")) then
                    v.Handle.Mesh:Destroy()
                end
            end
        end
        if string.sub(CMDBAR.Text, 1, 7) == ("spinner") then
            local p = Instance.new("RocketPropulsion")
            p.Parent = lplayer.Character.HumanoidRootPart
            p.Name = "Spinner"
            p.Target = lplayer.Character["Left Arm"]
            p:Fire()
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Spinner enabled";
            Text = "Type ;nospinner to disable.";
            })
        end
        if string.sub(CMDBAR.Text, 1, 9) == ("nospinner") then
            lplayer.Character.HumanoidRootPart.Spinner:Destroy()
        end
        if string.sub(CMDBAR.Text, 1, 6) == ("reachd") then
            for i,v in pairs(game:GetService'Players'.LocalPlayer.Character:GetChildren())do
                if v:isA("Tool") then
                    local a = Instance.new("SelectionBox",v.Handle)
                    a.Adornee = v.Handle
                    v.Handle.Size = Vector3.new(0.5,0.5,60)
                    v.GripPos = Vector3.new(0,0,0)
                    lplayer.Character.Humanoid:UnequipTools()
                end
            end
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Reach applied!";
            Text = "Applied to equipped sword. Use ;noreach to disable.";
            })
        end
        if string.sub(CMDBAR.Text, 1, 6) == ("reach ") then
            for i,v in pairs(game:GetService'Players'.LocalPlayer.Character:GetChildren())do
                if v:isA("Tool") then
                    local a = Instance.new("SelectionBox",v.Handle)
                    a.Name = "Reach"
                    a.Adornee = v.Handle
                    v.Handle.Size = Vector3.new(0.5,0.5,(string.sub(CMDBAR.Text, 7)))
                    v.GripPos = Vector3.new(0,0,0)
                    lplayer.Character.Humanoid:UnequipTools()
                end
            end
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Reach applied!";
            Text = "Applied to equipped sword. Use ;noreach to disable.";
            })
        end
        if string.sub(CMDBAR.Text, 1, 7) == ("noreach") then
            for i,v in pairs(game:GetService'Players'.LocalPlayer.Character:GetChildren())do
                if v:isA("Tool") then
                    v.Handle.Reach:Destroy()
                end
            end
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Reach removed!";
            Text = "Removed reach from equipped sword.";
            })
        end
        if string.sub(CMDBAR.Text, 1, 6) == ("rkill ") then
            for i,v in pairs(GetPlayer(string.sub(CMDBAR.Text, 7)))do
                lplayer.Character.Humanoid.Name = 1
                local l = lplayer.Character["1"]:Clone()
                l.Parent = lplayer.Character
                l.Name = "Humanoid"
                wait(0.1)
                lplayer.Character["1"]:Destroy()
                game:GetService("Workspace").CurrentCamera.CameraSubject = lplayer.Character
                lplayer.Character.Animate.Disabled = true
                wait(0.1)
                lplayer.Character.Animate.Disabled = false
                lplayer.Character.Humanoid.DisplayDistanceType = "None"
                for i,v in pairs(game:GetService'Players'.LocalPlayer.Backpack:GetChildren())do
                lplayer.Character.Humanoid:EquipTool(v)
                end
                wait(0.1)
                lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character.HumanoidRootPart.CFrame
                wait(0.2)
                lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character.HumanoidRootPart.CFrame
                wait(0.5)
                lplayer.Character.HumanoidRootPart.CFrame = CFrame.new(Vector3.new(-100000,10,-100000))
                game:GetService("StarterGui"):SetCore("SendNotification", {
                Title = "Tools needed!";
                Text = "You need a tool in your backpack for this command!";
                })
            end
        end
        if string.sub(CMDBAR.Text, 1, 6) == ("tp me ") then
            for i,v in pairs(GetPlayer(string.sub(CMDBAR.Text, 7))) do
                lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character.HumanoidRootPart.CFrame
            end
        end
        if string.sub(CMDBAR.Text, 1, 7) == ("cbring ") then
            if (string.sub(CMDBAR.Text, 8)) == "all" or (string.sub(CMDBAR.Text, 8)) == "All" or (string.sub(CMDBAR.Text, 8)) == "ALL" then
                cbringall = true
            else
                for i,v in pairs(GetPlayer(string.sub(CMDBAR.Text, 8))) do
                    brplr = v.Name
                end
            end
            cbring = true
        end
        if string.sub(CMDBAR.Text, 1, 8) == ("uncbring") then
            cbring = false
            cbringall = false
        end
        if string.sub(CMDBAR.Text, 1, 5) == ("swap ") then
            for i,v in pairs(GetPlayer(string.sub(CMDBAR.Text, 6))) do
                local NOWPLR = game:GetService("Players")[v.Name].Character.HumanoidRootPart.CFrame
                local NOW = lplayer.Character.HumanoidRootPart.CFrame
                lplayer.Character.Humanoid.Name = 1
                local l = lplayer.Character["1"]:Clone()
                l.Parent = lplayer.Character
                l.Name = "Humanoid"
                wait(0.1)
                lplayer.Character["1"]:Destroy()
                game:GetService("Workspace").CurrentCamera.CameraSubject = lplayer.Character
                lplayer.Character.Animate.Disabled = true
                wait(0.1)
                lplayer.Character.Animate.Disabled = false
                lplayer.Character.Humanoid.DisplayDistanceType = "None"
                for i,v in pairs(game:GetService'Players'.LocalPlayer.Backpack:GetChildren())do
                lplayer.Character.Humanoid:EquipTool(v)
                end
                local function tp(player,player2)
                local char1,char2=player.Character,player2.Character
                if char1 and char2 then
                char1:MoveTo(char2.Head.Position)
                end
                end
                wait(0.1)
                lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character.HumanoidRootPart.CFrame
                wait(0.2)
                lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character.HumanoidRootPart.CFrame
                wait(0.5)
                lplayer.Character.HumanoidRootPart.CFrame = NOW
                wait(0.6)
                tp(lplayer, game:GetService("Players")[v.Name])
                wait(0.4)
                lplayer.Character.HumanoidRootPart.CFrame = NOWPLR
                game:GetService("StarterGui"):SetCore("SendNotification", {
                Title = "Tools needed!";
                Text = "You need a tool in your backpack for this command!";
                })
            end
        end
        if string.sub(CMDBAR.Text, 1, 7) == ("glitch ") then
            for i,v in pairs(GetPlayer(string.sub(CMDBAR.Text, 8))) do
                lplayer.Character.Humanoid.Name = 1
                local l = lplayer.Character["1"]:Clone()
                l.Parent = lplayer.Character
                l.Name = "Humanoid"
                wait(0.1)
                lplayer.Character["1"]:Destroy()
                game:GetService("Workspace").CurrentCamera.CameraSubject = lplayer.Character
                lplayer.Character.Animate.Disabled = true
                wait(0.1)
                lplayer.Character.Animate.Disabled = false
                lplayer.Character.Humanoid.DisplayDistanceType = "None"
                for i,v in pairs(game:GetService'Players'.LocalPlayer.Backpack:GetChildren())do
                lplayer.Character.Humanoid:EquipTool(v)
                end
                lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character["Left Arm"].CFrame
                wait(0.3)
                lplayer.Character.HumanoidRootPart.CFrame = game:GetService("Players")[v.Name].Character["Left Arm"].CFrame
                wait(0.4)
                b = Instance.new("BodyForce")
                b.Parent = lplayer.Character.HumanoidRootPart
                b.Name = "Glitch"
                b.Force = Vector3.new(100000000,5000,0)
                game:GetService("StarterGui"):SetCore("SendNotification", {
                Title = "Tools needed!";
                Text = "You need a tool in your backpack for this command!";
                })
            end
        end
        if string.sub(CMDBAR.Text, 1, 8) == ("unglitch") then
            lplayer.Character.HumanoidRootPart.Glitch:Destroy()
            lplayer.Character.HumanoidRootPart.CFrame = CFrame.new(10000,0,10000)
            b = Instance.new("BodyForce")
            b.Parent = lplayer.Character.HumanoidRootPart
            b.Name = "unGlitch"
            b.Force = Vector3.new(0,-5000000,0)
            wait(2)
            lplayer.Character.HumanoidRootPart.unGlitch:Destroy()
        end
        if string.sub(CMDBAR.Text, 1, 8) == ("grespawn") then
            lplayer.Character.Humanoid.Health = 0
            wait(1)
            lplayer.Character.Head.CFrame = CFrame.new(1000000,0,1000000)
            lplayer.Character.Torso.CFrame = CFrame.new(1000000,0,1000000)
        end
        if string.sub(CMDBAR.Text, 1, 8) == ("explorer") then
            loadstring(game:GetObjects("rbxassetid://492005721")[1].Source)()
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Success!";
            Text = "DEX Explorer has loaded.";
            })
        end
        if string.sub(CMDBAR.Text, 1, 5) == ("anim ") then
            local Anim = Instance.new("Animation")
            Anim.AnimationId = "rbxassetid://"..(string.sub(CMDBAR.Text, 6))
            local track = lplayer.Character.Humanoid:LoadAnimation(Anim)
            track:Play(.1, 1, 1)
        end
        if string.sub(CMDBAR.Text, 1, 7) == ("animgui") then
            loadstring(game:GetObjects("rbxassetid://1202558084")[1].Source)()
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Success!";
            Text = "Energize Animations GUI has loaded.";
            })
        end
        if string.sub(CMDBAR.Text, 1, 7) == ("savepos") then
            saved = lplayer.Character.HumanoidRootPart.CFrame
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Position Saved";
            Text = "Use ;loadpos to return to saved position.";
            })
        end
        if string.sub(CMDBAR.Text, 1, 7) == ("loadpos") then
            lplayer.Character.HumanoidRootPart.CFrame = saved
        end
        if string.sub(CMDBAR.Text, 1, 5) == ("bang ") then
            for i,v in pairs(GetPlayer(string.sub(CMDBAR.Text, 6))) do
                local Anim2 = Instance.new("Animation")
                Anim2.AnimationId = "rbxassetid://148840371"
                local track2 = lplayer.Character.Humanoid:LoadAnimation(Anim2)
                track2:Play(.1, 1, 1)
                bplrr = v.Name
                banpl = true
            end
        end
        if string.sub(CMDBAR.Text, 1, 6) == ("unbang") then
            banpl = false
        end
        if string.sub(CMDBAR.Text, 1, 9) == ("bringmod ") then
            local function bringmodw()
            for i,obj in ipairs(game:GetService("Workspace"):GetDescendants()) do
            if obj.Name == (string.sub(CMDBAR.Text, 10)) then
            for i,ch in pairs(obj:GetDescendants()) do
            if (ch:IsA("BasePart")) then
            ch.CFrame = lplayer.Character.HumanoidRootPart.CFrame
            ch.CanCollide = false
            ch.Transparency = 0.7
            wait()
            ch.CFrame = lplayer.Character["Left Leg"].CFrame
            wait()
            ch.CFrame = lplayer.Character["Right Leg"].CFrame
            wait()
            ch.CFrame = lplayer.Character["Head"].CFrame
            end
            end
            end
            end
            end
            while wait() do
                bringmodw()
            end
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "BringMod";
            Text = "BringMod enabled.";
            })
        end
        if string.sub(CMDBAR.Text, 1, 7) == ("respawn") then
            local mod = Instance.new('Model', workspace) mod.Name = 're '..lplayer.Name
            local hum = Instance.new('Humanoid', mod)
            local ins = Instance.new('Part', mod) ins.Name = 'Torso' ins.CanCollide = false ins.Transparency = 1
            lplayer.Character = mod
        end
        if string.sub(CMDBAR.Text, 1, 8) == ("shutdown") then
            game:GetService'RunService'.Stepped:Connect(function()
            pcall(function()
                for i,v in pairs(game:GetService'Players':GetPlayers()) do
                    if v.Character ~= nil and v.Character:FindFirstChild'Head' then
                        for _,x in pairs(v.Character.Head:GetChildren()) do
                            if x:IsA'Sound' then x.Playing = true x.CharacterSoundEvent:FireServer(true, true) end
                        end
                    end
                end
            end)
            end)
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Attempting Shutdown";
            Text = "Shutdown Attempt has begun.";
            })
        end
        if string.sub(CMDBAR.Text, 1, 7) == ("delobj ") then
            objtodel = (string.sub(CMDBAR.Text, 8))
            for i,v in pairs(game:GetService("Workspace"):GetDescendants()) do
                if v.Name == objtodel then
                    v:Destroy()
                end
            end
        end
        if string.sub(CMDBAR.Text, 1, 7) == ("getplrs") then
            for i,v in pairs(game:GetService("Players"):GetPlayers())do
                print(v)
            end
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Printed";
            Text = "Players have been printed to console. (F9)";
            })
        end
        if string.sub(CMDBAR.Text, 1, 8) == ("deldecal") then
            for i,v in pairs(game:GetService("Workspace"):GetDescendants())do
                if (v:IsA("Decal")) then
                    v:Destroy()
                end
            end
        end
        if string.sub(CMDBAR.Text, 1, 10) == ("opfinality") then
            loadstring(game:GetObjects("rbxassetid://1294358929")[1].Source)()
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Success!";
            Text = "OpFinality GUI has loaded.";
            })
        end
        if string.sub(CMDBAR.Text, 1, 7) == ("remotes") then
            remotes = true
            added = true
            game.DescendantAdded:connect(function(rmt)
            if added == true then
            if remotes == true then
            if rmt:IsA("RemoteEvent") then
            print("A RemoteEvent was added!")
            print(" game." .. rmt:GetFullName() .. " | RemoteEvent")
            print(" game." .. rmt:GetFullName() .. " | RemoteEvent", 247, 0, 0, true)
            end end end
            end)
            game.DescendantAdded:connect(function(rmtfnctn)
            if added == true then
            if remotes == true then
            if rmtfnctn:IsA("RemoteFunction") then
            warn("A RemoteFunction was added!")
            warn(" game." .. rmtfnctn:GetFullName() .. " | RemoteFunction")
            print(" game." .. rmtfnctn:GetFullName() .. " | RemoteFunction", 5, 102, 198, true)
            end end end
            end)
           
            game.DescendantAdded:connect(function(bndfnctn)
            if added == true then
            if binds == true then
            if bndfnctn:IsA("BindableFunction") then
            print("A BindableFunction was added!")
            print(" game." .. bndfnctn:GetFullName() .. " | BindableFunction")
            print(" game." .. bndfnctn:GetFullName() .. " | BindableFunction", 239, 247, 4, true)
            end end end
            end)
           
            game.DescendantAdded:connect(function(bnd)
            if added == true then
            if binds == true then
            if bnd:IsA("BindableEvent") then
            warn("A BindableEvent was added!")
            warn(" game." .. bnd:GetFullName() .. " | BindableEvent")
            print(" game." .. bnd:GetFullName() .. " | BindableEvent", 13, 193, 22, true)
            end end end
            end)
           
           
            if binds == true then
            for i,v in pairs(game:GetDescendants()) do
            if v:IsA("BindableFunction") then
            print(" game." .. v:GetFullName() .. " | BindableFunction")
            print(" game." .. v:GetFullName() .. " | BindableFunction", 239, 247, 4, true)
            end end
            for i,v in pairs(game:GetDescendants()) do
            if v:IsA("BindableEvent") then
            warn(" game." .. v:GetFullName() .. " | BindableEvent")
            print(" game." .. v:GetFullName() .. " | BindableEvent", 13, 193, 22, true)
            end end
            else
            print("Off")
            end
            if remotes == true then
            for i,v in pairs(game:GetDescendants()) do
            if v:IsA("RemoteFunction") then
            warn(" game." .. v:GetFullName() .. " | RemoteFunction")
            print(" game." .. v:GetFullName() .. " | RemoteFunction", 5, 102, 198, true)
            end end
            wait()
            for i,v in pairs(game:GetDescendants()) do
            if v:IsA("RemoteEvent") then
            print(" game." .. v:GetFullName() .. " | RemoteEvent")
            print(" game." .. v:GetFullName() .. " | RemoteEvent", 247, 0, 0, true)
            end end
            else
            print("Off")
            end
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Printing Remotes";
            Text = "Type ;noremotes to disable.";
            })
        end
        if string.sub(CMDBAR.Text, 1, 9) == ("noremotes") then
            remotes = false
            added = false
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Printing Remotes Disabled";
            Text = "Type ;remotes to enable.";
            })
        end
        if string.sub(CMDBAR.Text, 1, 9) == ("tpdefault") then
            spin = false
            followed = false
            traill = false
            noclip = false
            annoying = false
            hwalk = false
            cbringing = false
        end
        if string.sub(CMDBAR.Text, 1, 7) == ("stopsit") then
            stopsitting = true
        end
        if string.sub(CMDBAR.Text, 1, 5) == ("gosit") then
            stopsitting = false
        end
        if string.sub(CMDBAR.Text, 1, 7) == ("version") then
            print(adminversion)
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Version";
            Text = adminversion;
            })
        end
        if string.sub(CMDBAR.Text, 1, 7) == ("clicktp") then
            clickgoto = true
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Click TP";
            Text = "Press E to teleport to mouse position";
            })
        end
        if string.sub(CMDBAR.Text, 1, 9) == ("noclicktp") then
            clickgoto = false
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Click TP";
            Text = "Click TP has been disabled.";
            })
        end
        if string.sub(CMDBAR.Text, 1, 7) == ("toolson") then
            gettingtools = true
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Tools Enabled";
            Text = "Automatically colleting tools dropped.";
            })
        end
        if string.sub(CMDBAR.Text, 1, 8) == ("toolsoff") then
            gettingtools = false
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Tools Disabled";
            Text = "Click TP has been disabled.";
            })
        end
        if string.sub(CMDBAR.Text, 1, 9) == ("delcmdbar") then
            ScreenGui:Destroy()
        end
        if string.sub(CMDBAR.Text, 1, 5) == ("reset") then
            lplayer.Character.Head:Destroy()
        end
        if string.sub(CMDBAR.Text, 1, 6) == ("state ") then
            statechosen = string.sub(CMDBAR.Text, 7)
            changingstate = true
        end
        if string.sub(CMDBAR.Text, 1, 8) == ("gravity ") then
            game:GetService("Workspace").Gravity = string.sub(CMDBAR.Text, 9)
        end
        if string.sub(CMDBAR.Text, 1, 9) == ("looprhats") then
        removingmeshhats = true
        end
        if string.sub(CMDBAR.Text, 1, 11) == ("unlooprhats") then
            removingmeshhats = false
        end
        if string.sub(CMDBAR.Text, 1, 9) == ("looprtool") then
            removingmeshtool = true
        end
        if string.sub(CMDBAR.Text, 1, 11) == ("unlooprtool") then
            removingmeshtool = false
        end
        if string.sub(CMDBAR.Text, 1, 9) == ("givetool ") then
            for i,v in pairs(game:GetService("Players").LocalPlayer.Character:GetDescendants()) do
                if v:IsA("Tool") then
                    for i,player in pairs(GetPlayer(string.sub(CMDBAR.Text, 10))) do
                        v.Parent = player.Character
                    end
                end
            end
        end
        if string.sub(CMDBAR.Text, 1, 4) == ("age ") then
            for i,player in pairs(GetPlayer(string.sub(CMDBAR.Text, 5))) do
                game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(player.Name.." Account Age: "..player.AccountAge.." days!", "All")
            end
        end
        if string.sub(CMDBAR.Text, 1, 3) == ("id ") then
            for i,player in pairs(GetPlayer(string.sub(CMDBAR.Text, 4))) do
                game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(player.Name.." Account ID: "..player.UserId, "All")
            end
        end
        if string.sub(CMDBAR.Text, 1, 5) == (".age ") then
            for i,player in pairs(GetPlayer(string.sub(CMDBAR.Text, 6))) do
                game:GetService("StarterGui"):SetCore("SendNotification", {
                Title = player.AccountAge.." Days";
                Text = "Account age of "..player.Name;
                })
            end
        end
        if string.sub(CMDBAR.Text, 1, 4) == (".id ") then
            for i,player in pairs(GetPlayer(string.sub(CMDBAR.Text, 5))) do
                game:GetService("StarterGui"):SetCore("SendNotification", {
                Title = player.UserId.." ID";
                Text = "Account ID of "..player.Name;
                })
            end
        end
        if string.sub(CMDBAR.Text, 1, 6) == ("gameid") then
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "Game ID";
            Text = "Game ID: ".. game.GameId;
            })
        end
        if string.sub(CMDBAR.Text, 1, 3) == ("pgs") then
            local pgscheck = game:GetService("Workspace"):PGSIsEnabled()
            if pgscheck == true then
                game:GetService("StarterGui"):SetCore("SendNotification", {
                Title = "PGSPhysicsSolverEnabled";
                Text = "PGS is Enabled!";
                })
            else
                game:GetService("StarterGui"):SetCore("SendNotification", {
                Title = "PGSPhysicsSolverEnabled";
                Text = "PGS is Disabled!";
                })
            end
        end
        if string.sub(CMDBAR.Text, 1, 11) == ("removeinvis") then
            for i,v in pairs(game:GetService("Workspace"):GetDescendants()) do
                if v:IsA("Part") then
                    if v.Transparency == 1 then
                        if v.Name ~= "HumanoidRootPart" then
                            v:Destroy()
                        end
                    end
                end
            end
        end
        if string.sub(CMDBAR.Text, 1, 9) == ("removefog") then
            game:GetService("Lighting").FogStart = 0
            game:GetService("Lighting").FogEnd = 9999999999999
        end
        if string.sub(CMDBAR.Text, 1, 7) == ("disable") then
            lplayer.Character.Humanoid.Parent = lplayer
        end
        if string.sub(CMDBAR.Text, 1, 6) == ("enable") then
            lplayer.Humanoid.Parent = lplayer.Character
        end
        if string.sub(CMDBAR.Text, 1, 13) == ("givealltools ") then
            for i,v in pairs(game:GetService("Players").LocalPlayer.Backpack:GetDescendants()) do
                if v:IsA("Tool") then
                    v.Parent = lplayer.Character
                    wait()
                    for i,player in pairs(GetPlayer(string.sub(CMDBAR.Text, 14))) do
                        v.Parent = player.Character
                    end
                end
            end
        end
        if string.sub(CMDBAR.Text, 1, 9) == ("flyspeed ") then
            speedfly = string.sub(CMDBAR.Text, 10)
            wait()
            change()
        end
        if string.sub(CMDBAR.Text, 1, 7) == ("carpet ") then
            for i,v in pairs(GetPlayer(string.sub(CMDBAR.Text, 8))) do
                local Anim3 = Instance.new("Animation")
                Anim3.AnimationId = "rbxassetid://282574440"
                local track3 = lplayer.Character.Humanoid:LoadAnimation(Anim3)
                track3:Play(.1, 1, 1)
                bplrr = v.Name
                banpl = true
            end
        end
        if string.sub(CMDBAR.Text, 1, 8) == ("uncarpet") then
            banpl = false
        end
        if string.sub(CMDBAR.Text, 1, 6) == ("stare ") then
            for i,v in pairs(GetPlayer(string.sub(CMDBAR.Text, 7))) do
                staring = true
                stareplr = v
            end
        end
        if string.sub(CMDBAR.Text, 1, 7) == ("unstare") then
            staring = false
        end
        if string.sub(CMDBAR.Text, 1, 7) == ("logchat") then
            chatlogs = true
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "LogChat enabled";
            Text = "Now logging all player chat.";
            })
        end
        if string.sub(CMDBAR.Text, 1, 9) == ("unlogchat") then
            chatlogs = false
            game:GetService("StarterGui"):SetCore("SendNotification", {
            Title = "LogChat disabled";
            Text = "Stopped logging all player chat.";
            })
        end
        if string.sub(CMDBAR.Text, 1, 6) == ("fixcam") then
            game:GetService("Workspace").CurrentCamera:Destroy()
            wait(0.1)
            game:GetService("Workspace").CurrentCamera.CameraSubject = lplayer.Character.Humanoid
            game:GetService("Workspace").CurrentCamera.CameraType = "Custom"
            lplayer.CameraMinZoomDistance = 0.5
            lplayer.CameraMaxZoomDistance = 400
            lplayer.CameraMode = "Classic"
        end
        if string.sub(CMDBAR.Text, 1, 7) == ("unstate") then
            changingstate = false
        end
        CMDBAR.Text = ""
    end
end)
 
wait(0.3)
game:GetService("StarterGui"):SetCore("SendNotification", {
    Title = "Loaded successfully!";
    Text = "Reviz Admin V2 by illremember";
})
wait(0.1)
print("Reviz Admin V2 loaded!")
if game:GetService("Workspace").FilteringEnabled == true then
    warn("FE is Enabled (Filtering Enabled)")
    game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "FE is Enabled";
        Text = "Filtering Enabled. Enjoy using Reviz Admin!";
    })
else
    warn("FE is Disabled (Filtering Disabled) Consider using a different admin script.")
    game:GetService("StarterGui"):SetCore("SendNotification", {
        Title = "FE is Disabled";
        Text = "Filtering Disabled. Consider using a different admin script.";
    })
end
 
local intro = Instance.new("ScreenGui")
local Frame = Instance.new("Frame")
local ImageLabel = Instance.new("ImageLabel")
intro.Parent = game:GetService("CoreGui")
Frame.Parent = intro
Frame.BackgroundColor3 = Color3.new(1, 1, 1)
Frame.BackgroundTransparency = 1
Frame.Size = UDim2.new(1, 0, 0, 300)
Frame.Position = UDim2.new(0, 0, -0.4, 0)
ImageLabel.Parent = Frame
ImageLabel.BackgroundColor3 = Color3.new(1, 1, 1)
ImageLabel.BackgroundTransparency = 1
ImageLabel.Position = UDim2.new(0, 0, 0, 0)
ImageLabel.Size = UDim2.new(1, 0, 1, 0)
ImageLabel.Image = "http://www.roblox.com/asset/?id=1542162618"
Frame:TweenPosition(UDim2.new(0, 0, 0.2, 0), "Out", "Elastic", 3)
wait(3.01)
Frame:TweenPosition(UDim2.new(0, 0, 1.5, 0), "Out", "Elastic", 5)
wait(5.01)
intro:Destroy()
end)
 
Aimbot.Name = "Aimbot"
Aimbot.Parent = Main
Aimbot.BackgroundColor3 = Color3.new(1, 0, 1)
Aimbot.Position = UDim2.new(0.709731519, 0, 0.701970458, 0)
Aimbot.Size = UDim2.new(0, 173, 0, 59)
Aimbot.Font = Enum.Font.Cartoon
Aimbot.Text = "Aimbot"
Aimbot.TextColor3 = Color3.new(1, 1, 1)
Aimbot.TextScaled = true
Aimbot.TextSize = 14
Aimbot.MouseButton1Down:connect(function()
local plrs = game:GetService("Players")
local TeamBased = true ; local teambasedswitch = "o"
local presskeytoaim = true; local aimkey = "e"
local raycast = false
 
local espupdatetime = 5; autoesp = false
 
 
 
local lockaim = true; local lockangle = 5
 
 
 
--function findwat(folder, what)
--      for i, smth in pairs(folder:GetChildren()) do
--              if string.find(string.lower(tostring(smth)), string.lower(what)) then
--                      return smth
--              end
--      end
--end
--
--local plrs = findwat(game, "Players")
 
 
 
 
local Gui = Instance.new("ScreenGui")
local Move = Instance.new("Frame")
local Main = Instance.new("Frame")
local EspStatus = Instance.new("TextLabel")
local st1 = Instance.new("TextLabel")
local st1_2 = Instance.new("TextLabel")
local st1_3 = Instance.new("TextLabel")
local Name = Instance.new("TextLabel")
--Properties:
Gui.Name = "Gui"
Gui.Parent = plrs.LocalPlayer:WaitForChild("PlayerGui")
 
Move.Name = "Move"
Move.Parent = Gui
Move.BackgroundColor3 = Color3.new(0.0431373, 1, 0.0745098)
Move.BackgroundTransparency = 0.40000000596046
Move.BorderSizePixel = 0
Move.Position = UDim2.new(0.005, 0,0.018, 0)
Move.Size = UDim2.new(0.28141585, 0, 0.0320388414, 0)
 
Main.Name = "Main"
Main.Parent = Move
Main.BackgroundColor3 = Color3.new(0.176471, 0.176471, 0.176471)
Main.BackgroundTransparency = 0.69999998807907
Main.Position = UDim2.new(0, 0, 0.995670795, 0)
Main.Size = UDim2.new(1.0000006, 0, 9.79697132, 0)
 
EspStatus.Name = "EspStatus"
EspStatus.Parent = Main
EspStatus.BackgroundColor3 = Color3.new(1, 1, 1)
EspStatus.BackgroundTransparency = 1
EspStatus.Size = UDim2.new(0.272955924, 0, 0.161862016, 0)
EspStatus.Font = Enum.Font.ArialBold
EspStatus.Text = "Press T to update Esp"
EspStatus.TextColor3 = Color3.new(0.0431373, 1, 0.0745098)
EspStatus.TextScaled = true
EspStatus.TextSize = 14
EspStatus.TextWrapped = true
 
st1.Name = "st1"
st1.Parent = Main
st1.BackgroundColor3 = Color3.new(1, 1, 1)
st1.BackgroundTransparency = 1
st1.Position = UDim2.new(0.271787882, 0, 0, 0)
st1.Size = UDim2.new(0.728211343, 0, 0.161862016, 0)
st1.Font = Enum.Font.ArialBold
st1.Text = "Press "..aimkey.." to lock on a person inside ur view"
st1.TextColor3 = Color3.new(0.0431373, 1, 0.0745098)
st1.TextScaled = true
st1.TextSize = 14
st1.TextWrapped = true
 
st1_2.Name = "st1"
st1_2.Parent = Main
st1_2.BackgroundColor3 = Color3.new(1, 1, 1)
st1_2.BackgroundTransparency = 1
st1_2.Position = UDim2.new(0, 0, 0.375590861, 0)
st1_2.Size = UDim2.new(0.999999881, 0, 0.161862016, 0)
st1_2.Font = Enum.Font.ArialBold
st1_2.Text = "Press L to enable esp loop"
st1_2.TextColor3 = Color3.new(0.0431373, 1, 0.0745098)
st1_2.TextScaled = true
st1_2.TextSize = 14
st1_2.TextWrapped = true
 
st1_3.Name = "st1"
st1_3.Parent = Main
st1_3.BackgroundColor3 = Color3.new(1, 1, 1)
st1_3.BackgroundTransparency = 1
st1_3.Position = UDim2.new(0, 0, 0.18558608, 0)
st1_3.Size = UDim2.new(0.999999881, 0, 0.161862016, 0)
st1_3.Font = Enum.Font.ArialBold
st1_3.Text = "Press O to change team based mode"
st1_3.TextColor3 = Color3.new(0.0431373, 1, 0.0745098)
st1_3.TextScaled = true
st1_3.TextSize = 14
st1_3.TextWrapped = true
local teambasedstatus = st1_3:Clone()
teambasedstatus.Parent = st1_3
teambasedstatus.TextScaled = true
teambasedstatus.Position = UDim2.new(0, 0,0.694, 0)
teambasedstatus.Text = tostring(TeamBased)
 
Name.Name = "Name"
Name.Parent = Move
Name.BackgroundColor3 = Color3.new(1, 1, 1)
Name.BackgroundTransparency = 1
Name.Size = UDim2.new(0.838, 0, 0.980000019, 0)
Name.Font = Enum.Font.Arial
Name.Text = "FPS gui v1.0"
Name.TextColor3 = Color3.new(0, 0, 0)
Name.TextScaled = true
Name.TextSize = 14
Name.TextWrapped = true
Name.TextXAlignment = Enum.TextXAlignment.Left
-- Scripts:
 
 
local plrsforaim = {}
 
local lplr = game:GetService("Players").LocalPlayer
Move.Draggable = true
Gui.ResetOnSpawn = false
Gui.Name = "Chat"
Gui.DisplayOrder = 999
 
        Gui.Parent = plrs.LocalPlayer.PlayerGui
 
 
f = {}
local espforlder
 
f.addesp = function()
        --print("ESP ran")
        if espforlder then
        else
                espforlder = Instance.new("Folder")
                espforlder.Parent = game.Workspace.CurrentCamera
        end
        for i, v in pairs(espforlder:GetChildren()) do
                v:Destroy()
        end
        for _, plr in pairs(plrs:GetChildren()) do
                if plr.Character and plr.Character.Humanoid.Health > 0 and plr.Name ~= lplr.Name then
                        if TeamBased == true then
                                if plr.Team.Name ~= plrs.LocalPlayer.Team.Name  then
                                        local e = espforlder:FindFirstChild(plr.Name)
                                        if not e then
                                                --print("Added esp for team based")
                                                local bill = Instance.new("BillboardGui", espforlder)
                                                bill.Name = plr.Name
                                                bill.AlwaysOnTop = true
                                                bill.Size = UDim2.new(1,0,1,0)
                                                bill.Adornee = plr.Character.Head
                                                local Frame = Instance.new('Frame',bill)
                                                Frame.Active = true
                                                Frame.BackgroundColor3 = Color3.new(0/255,255/255,0/255)
                                                Frame.BackgroundTransparency = 0
                                                Frame.BorderSizePixel = 0
                                                Frame.AnchorPoint = Vector2.new(.5, .5)
                                                Frame.Position = UDim2.new (0.5,0,0.5,0)
                                                Frame.Size = UDim2.new (1,0,1,0)
                                                Frame.Rotation = 0
                                                plr.Character.Humanoid.Died:Connect(function()
                                                        bill:Destroy()
                                                end)
                                        end
                                end
                        else
                                local e = espforlder:FindFirstChild(plr.Name)
                                if not e then
                                        --print("Added esp")
                                        local bill = Instance.new("BillboardGui", espforlder)
                                        bill.Name = plr.Name
                                        bill.AlwaysOnTop = true
                                        bill.Size = UDim2.new(1,0,1,0)
                                        bill.Adornee = plr.Character.Head
                                        local Frame = Instance.new('Frame',bill)
                                        Frame.Active = true
                                        Frame.BackgroundColor3 = Color3.new(0/255,255/255,0/255)
                                        Frame.BackgroundTransparency = 0
                                        Frame.BorderSizePixel = 0
                                        Frame.AnchorPoint = Vector2.new(.5, .5)
                                        Frame.Position = UDim2.new (0.5,0,0.5,0)
                                        Frame.Size = UDim2.new (1,0,1,0)
                                        Frame.Rotation = 0
                                        plr.Character.Humanoid.Died:Connect(function()
                                                bill:Destroy()
                                        end)
                                end
                        end
                       
                       
                end
        end
end
local cam = game.Workspace.CurrentCamera
 
local mouse = lplr:GetMouse()
local switch = false
local key = "k"
local aimatpart = nil
mouse.KeyDown:Connect(function(a)
        if a == "t" then
                print("worked1")
                f.addesp()
        elseif a == "u" then
                if raycast == true then
                        raycast = false
                else
                        raycast = true
                end
        elseif a == "l" then
                if autoesp == false then
                        autoesp = true
                else
                        autoesp = false
                end
        end
        if a == "j" then
                if mouse.Target then
                        mouse.Target:Destroy()
                end
        end
        if a == key then
                if switch == false then
                        switch = true
                else
                        switch = false
                        if aimatpart ~= nil then
                                aimatpart = nil
                        end
                end
        elseif a == teambasedswitch then
                if TeamBased == true then
                        TeamBased = false
                        teambasedstatus.Text = tostring(TeamBased)
                else
                        TeamBased = true
                        teambasedstatus.Text = tostring(TeamBased)
                end
        elseif a == aimkey then
                if not aimatpart then
                        local maxangle = math.rad(20)
                        for i, plr in pairs(plrs:GetChildren()) do
                                if plr.Name ~= lplr.Name and plr.Character and plr.Character.Head and plr.Character.Humanoid and plr.Character.Humanoid.Health > 1 then
                                        if TeamBased == true then
                                                if plr.Team.Name ~= lplr.Team.Name then
                                                        local an = checkfov(plr.Character.Head)
                                                        if an < maxangle then
                                                                maxangle = an
                                                                aimatpart = plr.Character.Head
                                                        end
                                                end
                                        else
                                                local an = checkfov(plr.Character.Head)
                                                        if an < maxangle then
                                                                maxangle = an
                                                                aimatpart = plr.Character.Head
                                                        end
                                                        print(plr)
                                        end
                                        plr.Character.Humanoid.Died:Connect(function()
                                                if aimatpart.Parent == plr.Character or aimatpart == nil then
                                                        aimatpart = nil
                                                end
                                        end)
                                end
                        end
                else
                        aimatpart = nil
                end
        end
end)
 
function getfovxyz (p0, p1, deg)
        local x1, y1, z1 = p0:ToOrientation()
        local cf = CFrame.new(p0.p, p1.p)
        local x2, y2, z2 = cf:ToOrientation()
        --local d = math.deg
        if deg then
                --return Vector3.new(d(x1-x2), d(y1-y2), d(z1-z2))
        else
                return Vector3.new((x1-x2), (y1-y2), (z1-z2))
        end
end
 
function getaimbotplrs()
        plrsforaim = {}
        for i, plr in pairs(plrs:GetChildren()) do
                if plr.Character and plr.Character.Humanoid and plr.Character.Humanoid.Health > 0 and plr.Name ~= lplr.Name and plr.Character.Head then
                       
                        if TeamBased == true then
                                if plr.Team.Name ~= lplr.Team.Name then
                                        local cf = CFrame.new(game.Workspace.CurrentCamera.CFrame.p, plr.Character.Head.CFrame.p)
                                        local r = Ray.new(cf, cf.LookVector * 10000)
                                        local ign = {}
                                        for i, v in pairs(plrs.LocalPlayer.Character:GetChildren()) do
                                                if v:IsA("BasePart") then
                                                        table.insert(ign , v)
                                                end
                                        end
                                        local obj = game.Workspace:FindPartOnRayWithIgnoreList(r, ign)
                                        if obj.Parent == plr.Character and obj.Parent ~= lplr.Character then
                                                table.insert(plrsforaim, obj)
                                        end
                                end
                        else
                                local cf = CFrame.new(game.Workspace.CurrentCamera.CFrame.p, plr.Character.Head.CFrame.p)
                                local r = Ray.new(cf, cf.LookVector * 10000)
                                local ign = {}
                                for i, v in pairs(plrs.LocalPlayer.Character:GetChildren()) do
                                        if v:IsA("BasePart") then
                                                table.insert(ign , v)
                                        end
                                end
                                local obj = game.Workspace:FindPartOnRayWithIgnoreList(r, ign)
                                if obj.Parent == plr.Character and obj.Parent ~= lplr.Character then
                                        table.insert(plrsforaim, obj)
                                end
                        end
                       
                       
                end
        end
end
 
function aimat(part)
        cam.CFrame = CFrame.new(cam.CFrame.p, part.CFrame.p)
end
function checkfov (part)
        local fov = getfovxyz(game.Workspace.CurrentCamera.CFrame, part.CFrame)
        local angle = math.abs(fov.X) + math.abs(fov.Y)
        return angle
end
 
game:GetService("RunService").RenderStepped:Connect(function()
        if aimatpart then
                aimat(aimatpart)
                if aimatpart.Parent == plrs.LocalPlayer.Character then
                        aimatpart = nil
                end
        end
       
       
--      if switch == true then
--              local maxangle = 99999
--             
--              --print("Loop")
--              if true and raycast == false then
--                      for i, plr in pairs(plrs:GetChildren()) do
--                              if plr.Name ~= lplr.Name and plr.Character and plr.Character.Head and plr.Character.Humanoid and plr.Character.Humanoid.Health > 1 then
--                                      if TeamBased then
--                                              if plr.Team.Name ~= lplr.Team.Name or plr.Team.TeamColor ~= lplr.Team.TeamColor then
--                                                      local an = checkfov(plr.Character.Head)
--                                                      if an < maxangle then
--                                                              maxangle = an
--                                                              aimatpart = plr.Character.Head
--                                                              if an < lockangle then
--                                                                      break
--                                                              end
--                                                      end
--                                              end
--                                      else
--                                              local an = checkfov(plr.Character.Head)
--                                                      if an < maxangle then
--                                                              maxangle = an
--                                                              aimatpart = plr.Character.Head
--                                                              if an < lockangle then
--                                                                      break
--                                                              end
--                                                      end
--                                      end
--                                     
--                                     
--                                     
--                                     
--                              end
--                      end
--              elseif raycast == true then
--                     
--              end
               
                if raycast == true and switch == false and not aimatpart then
                        getaimbotplrs()
                        aimatpart = nil
                        local maxangle = 999
                        for i, v in ipairs(plrsforaim) do
                                if v.Parent ~= lplr.Character then
                                        local an = checkfov(v)
                                        if an < maxangle and v ~= lplr.Character.Head then
                                                maxangle = an
                                                aimatpart = v
                                                print(v:GetFullName())
                                                v.Parent.Humanoid.Died:connect(function()
                                                        aimatpart = nil
                                                end)
                                        end
                                end
                        end
               
        end
end)
delay(0, function()
        while wait(espupdatetime) do
                if autoesp == true then
                        pcall(function()
                        f.addesp()
                        end)
                end
        end
end)
warn("loaded")
end)
 
JailbreakGui.Name = "Jailbreak Gui"
JailbreakGui.Parent = Main
JailbreakGui.BackgroundColor3 = Color3.new(1, 0, 1)
JailbreakGui.Position = UDim2.new(0.362416089, 0, 0.701970458, 0)
JailbreakGui.Size = UDim2.new(0, 173, 0, 59)
JailbreakGui.Font = Enum.Font.Cartoon
JailbreakGui.Text = "Jailbreak Gui"
JailbreakGui.TextColor3 = Color3.new(1, 1, 1)
JailbreakGui.TextScaled = true
JailbreakGui.TextSize = 14
JailbreakGui.MouseButton1Down:connect(function()
-- Objects
 
local AnisJailbreakGui = Instance.new("ScreenGui")
local Main = Instance.new("Frame")
local Top = Instance.new("Frame")
local Title = Instance.new("TextLabel")
local Exit = Instance.new("TextButton")
local FreeGrageMobile = Instance.new("TextButton")
local InfNitro = Instance.new("TextButton")
local InfDonite = Instance.new("TextButton")
local AutoRob = Instance.new("TextButton")
local NoDoors = Instance.new("TextButton")
local Btools = Instance.new("TextButton")
local InfJump = Instance.new("TextButton")
local Open = Instance.new("TextButton")
 
-- Properties
 
AnisJailbreakGui.Name = "Anis Jailbreak Gui"
AnisJailbreakGui.Parent = game.CoreGui
AnisJailbreakGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
 
Main.Name = "Main"
Main.Parent = AnisJailbreakGui
Main.BackgroundColor3 = Color3.new(0.0980392, 0.0980392, 0.0980392)
Main.Position = UDim2.new(0.287649363, 0, 0.229729727, 0)
Main.Size = UDim2.new(0, 592, 0, 404)
Main.Visible = false
 
Top.Name = "Top"
Top.Parent = Main
Top.BackgroundColor3 = Color3.new(0.0980392, 0.0980392, 0.0980392)
Top.Position = UDim2.new(-0.00120195746, 0, -0.001039505, 0)
Top.Size = UDim2.new(0, 592, 0, 390)
 
Title.Name = "Title"
Title.Parent = Top
Title.BackgroundColor3 = Color3.new(0, 0, 0)
Title.Size = UDim2.new(0, 592, 0, 56)
Title.Font = Enum.Font.SourceSans
Title.Text = "Anis Jailbreak Gui"
Title.TextColor3 = Color3.new(1, 1, 1)
Title.TextScaled = true
Title.TextSize = 14
 
Exit.Name = "Exit"
Exit.Parent = Title
Exit.BackgroundColor3 = Color3.new(1, 0, 0)
Exit.Position = UDim2.new(0.908783793, 0, 0.0535714291, 0)
Exit.Size = UDim2.new(0, 54, 0, 50)
Exit.Font = Enum.Font.SourceSans
Exit.Text = "X"
Exit.TextColor3 = Color3.new(0, 0, 0)
Exit.TextScaled = true
Exit.TextSize = 14
Exit.MouseButton1Down:connect(function()
Open.Visible = true
Main.Visible = false
end)
 
FreeGrageMobile.Name = "Free Grage Mobile"
FreeGrageMobile.Parent = Top
FreeGrageMobile.BackgroundColor3 = Color3.new(0.105882, 0.105882, 0.105882)
FreeGrageMobile.Position = UDim2.new(0.0688665211, 0, 0.209887147, 0)
FreeGrageMobile.Size = UDim2.new(0, 230, 0, 50)
FreeGrageMobile.Font = Enum.Font.SourceSans
FreeGrageMobile.Text = "Garage Mobile"
FreeGrageMobile.TextColor3 = Color3.new(0, 0, 0)
FreeGrageMobile.TextScaled = true
FreeGrageMobile.TextSize = 14
FreeGrageMobile.MouseButton1Down:connect(function()
game:GetService("Players").LocalPlayer.UserId = 2837719
end)
 
InfNitro.Name = "Inf Nitro"
InfNitro.Parent = Top
InfNitro.BackgroundColor3 = Color3.new(0.105882, 0.105882, 0.105882)
InfNitro.Position = UDim2.new(0.0671773329, 0, 0.456041098, 0)
InfNitro.Size = UDim2.new(0, 230, 0, 50)
InfNitro.Font = Enum.Font.SourceSans
InfNitro.Text = "Inf Nitro"
InfNitro.TextColor3 = Color3.new(0, 0, 0)
InfNitro.TextScaled = true
InfNitro.TextSize = 14
InfNitro.MouseButton1Down:connect(function()
loadstring(game:HttpGet("https://pastebin.com/raw/VQkvwLBP"))()
end)
 
InfDonite.Name = "Inf Donite"
InfDonite.Parent = Top
InfDonite.BackgroundColor3 = Color3.new(0.105882, 0.105882, 0.105882)
InfDonite.Position = UDim2.new(0.536771953, 0, 0.209887147, 0)
InfDonite.Size = UDim2.new(0, 234, 0, 50)
InfDonite.Font = Enum.Font.SourceSans
InfDonite.Text = "Inf Donuts"
InfDonite.TextColor3 = Color3.new(0, 0, 0)
InfDonite.TextScaled = true
InfDonite.TextSize = 14
InfDonite.MouseButton1Down:connect(function()
while wait(5) do
game:GetService('Workspace').TouchTrigger.Donut.Position = game:GetService("Players").LocalPlayer.Character.Head.Position
end
end)
 
AutoRob.Name = "Auto-Rob"
AutoRob.Parent = Top
AutoRob.BackgroundColor3 = Color3.new(0.105882, 0.105882, 0.105882)
AutoRob.Position = UDim2.new(0.536771834, 0, 0.456041098, 0)
AutoRob.Size = UDim2.new(0, 234, 0, 50)
AutoRob.Font = Enum.Font.SourceSans
AutoRob.Text = "Auto-Rob"
AutoRob.TextColor3 = Color3.new(0, 0, 0)
AutoRob.TextScaled = true
AutoRob.TextSize = 14
AutoRob.MouseButton1Down:connect(function()
loadstring(game:GetObjects("rbxassetid://1461971147")[1].Source)()
end)
 
NoDoors.Name = "No-Doors"
NoDoors.Parent = Top
NoDoors.BackgroundColor3 = Color3.new(0.105882, 0.105882, 0.105882)
NoDoors.Position = UDim2.new(0.0671772286, 0, 0.686810255, 0)
NoDoors.Size = UDim2.new(0, 230, 0, 50)
NoDoors.Font = Enum.Font.SourceSans
NoDoors.Text = "No-Doors"
NoDoors.TextColor3 = Color3.new(0, 0, 0)
NoDoors.TextScaled = true
NoDoors.TextSize = 14
NoDoors.MouseButton1Down:connect(function()
game.Workspace.Doors:remove()
end)
 
Btools.Name = "Btools"
Btools.Parent = Top
Btools.BackgroundColor3 = Color3.new(0.105882, 0.105882, 0.105882)
Btools.Position = UDim2.new(0.536771834, 0, 0.686810255, 0)
Btools.Size = UDim2.new(0, 234, 0, 49)
Btools.Font = Enum.Font.SourceSans
Btools.Text = "Btools"
Btools.TextColor3 = Color3.new(0, 0, 0)
Btools.TextScaled = true
Btools.TextSize = 14
Btools.MouseButton1Down:connect(function()
game.StarterGui:SetCoreGuiEnabled(Enum.CoreGuiType.Backpack, true)
for index, child in pairs(game:GetService("Workspace"):GetChildren()) do
   if child.ClassName == "Part" then
       child.Locked = false
   end
   if child.ClassName == "MeshPart" then
       child.Locked = false
   end
   if child.ClassName == "UnionOperation" then
       child.Locked = false
   end
   if child.ClassName == "Model" then
       for index, chil in pairs(child:GetChildren()) do
           if chil.ClassName == "Part" then
               chil.Locked = false
           end
           if chil.ClassName == "MeshPart" then
               chil.Locked = false
           end
           if chil.ClassName == "UnionOperation" then
               chil.Locked = false
           end
           if chil.ClassName == "Model" then
               for index, childe in pairs(chil:GetChildren()) do
                   if childe.ClassName == "Part" then
                       childe.Locked = false
                   end
                   if childe.ClassName == "MeshPart" then
                       childe.Locked = false
                   end
                   if childe.ClassName == "UnionOperation" then
                       childe.Locked = false
                   end
                   if childe.ClassName == "Model" then
                       for index, childeo in pairs(childe:GetChildren()) do
                           if childeo.ClassName == "Part" then
                               childeo.Locked = false
                           end
                           if childeo.ClassName == "MeshPart" then
                               childeo.Locked = false
                           end
                           if childeo.ClassName == "UnionOperation" then
                               childeo.Locked = false
                           end
                           if childeo.ClassName == "Model" then
                           end
                       end
                   end
               end
           end
       end
   end
end
c = Instance.new("HopperBin", game:GetService("Players").LocalPlayer.Backpack)
c.BinType = Enum.BinType.Hammer
c = Instance.new("HopperBin", game:GetService("Players").LocalPlayer.Backpack)
c.BinType = Enum.BinType.Clone
c = Instance.new("HopperBin", game:GetService("Players").LocalPlayer.Backpack)
c.BinType = Enum.BinType.Grab
end)
 
 
InfJump.Name = "Inf Jump"
InfJump.Parent = Top
InfJump.BackgroundColor3 = Color3.new(0.105882, 0.105882, 0.105882)
InfJump.Position = UDim2.new(0.278325886, 0, 0.909887195, 0)
InfJump.Size = UDim2.new(0, 261, 0, 49)
InfJump.Font = Enum.Font.SourceSans
InfJump.Text = "Inf Jump"
InfJump.TextColor3 = Color3.new(0, 0, 0)
InfJump.TextScaled = true
InfJump.TextSize = 14
InfJump.MouseButton1Down:connect(function()
game:GetService("UserInputService").JumpRequest:connect(function()
                game:GetService"Players".LocalPlayer.Character:FindFirstChildOfClass'Humanoid':ChangeState("Jumping")          
        end)
end)
 
Open.Name = "Open"
Open.Parent = AnisJailbreakGui
Open.BackgroundColor3 = Color3.new(0.105882, 0.105882, 0.105882)
Open.Position = UDim2.new(0.661771894, 0, 0.946691811, 0)
Open.Size = UDim2.new(0, 138, 0, 50)
Open.Font = Enum.Font.SourceSans
Open.Text = "Open"
Open.TextColor3 = Color3.new(0, 0, 0)
Open.TextScaled = true
Open.TextSize = 14
Open.MouseButton1Down:connect(function()
Main.Visible = true
Open.Visible = false
end)
end)
 
Gravity.Name = "Gravity"
Gravity.Parent = Main
Gravity.BackgroundColor3 = Color3.new(1, 0, 1)
Gravity.Position = UDim2.new(0.36409393, 0, 0.42610839, 0)
Gravity.Size = UDim2.new(0, 173, 0, 59)
Gravity.Font = Enum.Font.Cartoon
Gravity.Text = "Gravity"
Gravity.TextColor3 = Color3.new(1, 1, 1)
Gravity.TextScaled = true
Gravity.TextSize = 14
Gravity.MouseButton1Down:connect(function()
game.Workspace.Gravity = 30
end)
 
InfJump.Name = "Inf Jump"
InfJump.Parent = Main
InfJump.BackgroundColor3 = Color3.new(1, 0, 1)
InfJump.Position = UDim2.new(-2.98023224e-08, 0, 0.42610839, 0)
InfJump.Size = UDim2.new(0, 173, 0, 59)
InfJump.Font = Enum.Font.Cartoon
InfJump.Text = "Inf Jump"
InfJump.TextColor3 = Color3.new(1, 1, 1)
InfJump.TextScaled = true
InfJump.TextSize = 14
InfJump.MouseButton1Down:connect(function()
game:GetService("UserInputService").JumpRequest:connect(function()
                game:GetService"Players".LocalPlayer.Character:FindFirstChildOfClass'Humanoid':ChangeState("Jumping")          
        end)
end)
 
QToTeleport.Name = "Q To Teleport"
QToTeleport.Parent = Main
QToTeleport.BackgroundColor3 = Color3.new(1, 0, 1)
QToTeleport.Position = UDim2.new(-2.98023224e-08, 0, 0.701970458, 0)
QToTeleport.Size = UDim2.new(0, 173, 0, 59)
QToTeleport.Font = Enum.Font.Cartoon
QToTeleport.Text = "Q To Teleport"
QToTeleport.TextColor3 = Color3.new(1, 1, 1)
QToTeleport.TextScaled = true
QToTeleport.TextSize = 14
QToTeleport.MouseButton1Down:connect(function()
plr = game.Players.LocalPlayer
 
hum = plr.Character.HumanoidRootPart
 
mouse = plr:GetMouse()
 
 
 
mouse.KeyDown:connect(function(key)
 
if key == "q" then
 
if mouse.Target then
 
hum.CFrame = CFrame.new(mouse.Hit.x, mouse.Hit.y + 5, mouse.Hit.z)
 
end
 
end
end)
end)
 
Exit.Name = "Exit"
Exit.Parent = Main
Exit.BackgroundColor3 = Color3.new(1, 0, 0)
Exit.Position = UDim2.new(0.927852333, 0, 0, 0)
Exit.Size = UDim2.new(0, 43, 0, 39)
Exit.Font = Enum.Font.Cartoon
Exit.Text = "X"
Exit.TextColor3 = Color3.new(0, 0, 0)
Exit.TextScaled = true
Exit.TextSize = 14
Exit.MouseButton1Down:connect(function()
Open.Visible = true
Main.Visible = false
end)
 
Open.Name = "Open"
Open.Parent = AnisForCommandAndMore
Open.BackgroundColor3 = Color3.new(1, 0, 1)
Open.Position = UDim2.new(-1.18889147e-06, 0, 0.366093308, 0)
Open.Size = UDim2.new(0, 115, 0, 43)
Open.Font = Enum.Font.Cartoon
Open.Text = "Open"
Open.TextColor3 = Color3.new(1, 1, 1)
Open.TextScaled = true
Open.TextSize = 30
Open.MouseButton1Down:connect(function()
Main.Visible = true
Open.Visible = false
end)