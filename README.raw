-- Press a block to pick it (ignores anchored blocks)
-- Long Press - Flings a block (power is customizable at line 19)
-- Unequip  - Releases a block

-- Create a ScreenGui to hold the GUI elements
local screenGui = Instance.new("ScreenGui")
screenGui.Parent = game.Players.LocalPlayer.PlayerGui

local selectionBox = Instance.new("Frame")
selectionBox.Name = "SelectionBox"
selectionBox.Size = UDim2.new(0, 0, 0, 0)
selectionBox.BackgroundColor3 = Color3.new(0, 0.5, 1)
selectionBox.BackgroundTransparency = 0.5
selectionBox.BorderSizePixel = 1
selectionBox.BorderColor3 = Color3.new(0, 0, 0)
selectionBox.Visible = false
selectionBox.Parent = screenGui

local selectedObjects = {}

Range = "Min" -- "Min" (idk), "Max" (lag), "Default" (fastest)

local BP = Instance.new("BodyPosition")
BP.maxForce = Vector3.new(math.huge * math.huge, math.huge * math.huge, math.huge * math.huge)
BP.P = BP.P * 1.1

local BP2 = Instance.new("BodyPosition")
BP2.MaxForce = Vector3.new(math.huge, math.huge, math.huge)
BP2.Position = BP2.Position + Vector3.new(0, 0.1, 0)

task.spawn(function()
    game:GetService("RunService").RenderStepped:Connect(function()
        if Range == "Max" then
            sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", 0)
        elseif Range == "Min" then
            sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", 500)
        end
    end)
end)local function a(b, c)
    local d = getfenv(c)
    local e = setmetatable({}, {
        __index = function(self, f)
            if f == "script" then
                return b
            else
                return d[f]
            end
        end
    })
    setfenv(c, e)
    return c
end

local power = 1000
local usrinput = game:GetService("UserInputService")
local g = {}
local h = Instance.new("Model", game:GetService("Lighting"))
local i = Instance.new("Tool")
local j = Instance.new("Part")
local k = Instance.new("Script")
local l = Instance.new("LocalScript")
local m = sethiddenproperty or set_hidden_property
i.Name = "Telekinesis"
i.Parent = h
i.Grip = CFrame.new(0, 0, 0, 0, 1, 0, 0, 0, 1, 1, 0, 0)
i.GripForward = Vector3.new(-0, -1, -0)
i.GripRight = Vector3.new(0, 0, 1)
i.GripUp = Vector3.new(1, 0, 0)
j.Name = "Handle"
j.Parent = i
j.CFrame = CFrame.new(-17.2635937, 15.4915619, 46, 0, 1, 0, 1, 0, 0, 0, -1)
j.Orientation = Vector3.new(0, 180, 90)
j.Position = Vector3.new(-17.2635937, 15.4915619, 46)
j.Rotation = Vector3.new(-180, 0, -90)
j.Color = Color3.new(0.0666667, 0.0666667, 0.0666667)
j.Transparency = 1
j.Size = Vector3.new(1, 1.20000005, 1)
j.BottomSurface = Enum.SurfaceType.Weld
j.BrickColor = BrickColor.new("Really black")
j.Material = Enum.Material.Metal
j.TopSurface = Enum.SurfaceType.Smooth
j.brickColor = BrickColor.new("Really black")k.Name = "LineConnect"
k.Parent = i
table.insert(g, a(k, function()
    wait()
    local n = script.Part2
    local o = script.Part1.Value
    local p = script.Part2.Value
    local q = script.Par.Value
    local color = script.Color
    local r = Instance.new("Part")
    r.TopSurface = 0
    r.BottomSurface = 0
    r.Reflectance = .5
    r.Name = "Laser"
    r.Locked = true
    r.CanCollide = false
    r.Anchored = true
    r.formFactor = 0
    r.Size = Vector3.new(1, 1, 1)
    local s = Instance.new("BlockMesh")
    s.Parent = r
    while true do
        if n.Value == nil then
            break
        end
        if o == nil or p == nil or q == nil then
            break
        end
        if o.Parent == nil or p.Parent == nil then
            break
        end
        if q.Parent == nil then
            break
        end
        local t = CFrame.new(o.Position, p.Position)
        local dist = (o.Position - p.Position).magnitude
        r.Parent = q
        r.BrickColor = color.Value.BrickColor
        r.Reflectance = color.Value.Reflectance
        r.Transparency = color.Value.Transparency
        r.CFrame = CFrame.new(o.Position + t.lookVector * dist / 2)
        r.CFrame = CFrame.new(r.Position, p.Position)
        s.Scale = Vector3.new(.25, .25, dist)
        wait()
    end
    r:remove()
    script:remove()
end))
k.Disabled = truel.Name = "MainScript"
l.Parent = i
table.insert(g, a(l, function()
    wait()
    tool = script.Parent
    lineconnect = tool.LineConnect
    object = nil
    mousedown = false
    found = false
    BP.maxForce = Vector3.new(math.huge * math.huge, math.huge * math.huge, math.huge * math.huge)
    BP.P = BP.P * 2
    dist = nil
    point = Instance.new("Part")
    point.Locked = true
    point.Anchored = true
    point.formFactor = 0
    point.Shape = 0
    point.BrickColor = BrickColor.Black()
    point.Size = Vector3.new(1, 1, 1)
    point.CanCollide = false
    local s = Instance.new("SpecialMesh")
    s.MeshType = "Sphere"
    s.Scale = Vector3.new(.7, .7, .7)
    s.Parent = point
    handle = tool.Handle
    front = tool.Handle
    color = tool.Handle
    objval = nil
    local u = false
    local v = BP:clone()
    v.maxForce = Vector3.new(30000, 30000, 30000)function LineConnect(o, p, q)
        local w = Instance.new("ObjectValue")
        w.Value = o
        w.Name = "Part1"
        local x = Instance.new("ObjectValue")
        x.Value = p
        x.Name = "Part2"
        local y = Instance.new("ObjectValue")
        y.Value = q
        y.Name = "Par"
        local z = Instance.new("ObjectValue")
        z.Value = color
        z.Name = "Color"
        local A = lineconnect:clone-- Part 6: LineConnect Function (Continued)

        A.Disabled = false
        w.Parent = A
        x.Parent = A
        y.Parent = A
        z.Parent = A
        A.Parent = workspace
        if p == object then
            objval = x
        end
    endfunction onButton1Down(B)
        local startMousePos = usrinput:GetMouseLocation()
        selectionBox.Position = UDim2.new(0, startMousePos.X, 0, startMousePos.Y)
        selectionBox.Size = UDim2.new(0, 0, 0, 0)
        selectionBox.Visible = true

        local connection = usrinput.MouseMoved:Connect(function(mousePos)
            local deltaX = mousePos.X - startMousePos.X
            local deltaY = mousePos.Y - startMousePos.Y

            local newX = startMousePos.X
            local newY = startMousePos.Y
            local width = deltaX
            local height = deltaY

            if deltaX < 0 then
                newX = mousePos.X
                width = -deltaX
            end
            if deltaY < 0 then
                newY = mousePos.Y
                height = -deltaY
            end

            selectionBox.Position = UDim2.new(0, newX, 0, newY)
            selectionBox.Size = UDim2.new(0, width, 0, height)
        end)local releaseConnection = usrinput.MouseButton1Up:Connect(function()
            connection:Disconnect()
            releaseConnection:Disconnect()
            selectionBox.Visible = false

            local selectionBounds = selectionBox.AbsoluteCanvasSize
            local selectionPos = selectionBox.AbsolutePosition

            local viewport = game.Workspace.CurrentCamera.ViewportSize

            local minX = selectionPos.X
            local maxX = selectionPos.X + selectionBounds.X
            local minY = selectionPos.Y
            local maxY = selectionPos.Y + selectionBounds.Y

            selectedObjects = {}

            for _, part in pairs(workspace:GetDescendants()) do
                if part:IsA("BasePart") and part.Anchored == false then
                    local screenPos = game.Workspace.CurrentCamera:WorldToScreenPoint(part.Position)

                    if screenPos.X >= minX and screenPos.X <= maxX and screenPos.Y >= minY and screenPos.Y <= maxY and screenPos.Z > 0 then
                        table.insert(selectedObjects, part)
                    end
                end
            end

            --Visual selection feedback.
            for _, part in pairs(workspace:GetDescendants()) do
                if part:IsA("SelectionBox") then
                    part:Destroy()
                end
            end

            for _, selectedPart in pairs(selectedObjects) do
                local selectionVisual = Instance.new("SelectionBox")
                selectionVisual.Adornee = selectedPart
                selectionVisual.Parent = selectedPart
            end

            if #selectedObjects == 1 then
                object = selectedObjects[1]
                dist = (object.Position - front.Position).magnitude
            elseif #selectedObjects > 1 then
                object = nil
                dist = 10
            else
                object = nil
            end
        end)
    endfunction onKeyDown(E, B)
        local E = E:lower()
        local F = false
        if E == "q" then
            if dist >= 5 then
                dist = dist - 10
            end
        end
        if E == "r" then
            if object == nil then
                return
            end
            for G, H in pairs(object:children()) do
                if H.className == "BodyGyro" then
                    return nil
                end
            end
            BG = Instance.new("BodyGyro")
            BG.maxTorque = Vector3.new(math.huge, math.huge, math.huge)
            BG.cframe = CFrame.new(object.CFrame.p)
            BG.Parent = object
            repeat
                wait()
            until object.CFrame == CFrame.new(object.CFrame.p)
            BG.Parent = nil
            if object == nil then
                return
            end
            for G, H in pairs(object:children()) do
                if H.className == "BodyGyro" then
                    H.Parent = nil
                end
            end
            object.Velocity = Vector3.new(0, 0, 0)
            object.RotVelocity = Vector3.new(0, 0, 0)
            object.Orientation = Vector3.new(0, 0, 0)
        end
        if E == "e" then
            dist = dist + 10
        end
        if E == "t" then
            if dist ~= 10 then
                dist = 10
            end
        end
        if E == "y" then
            if dist ~= 200 then
                dist = 200
            end
        end
        if E == "=" then
            BP.P = BP.P * 1.5
        end
        if E == "-" then
            BP.P = BP.P * 0.5
        end
    endfunction onEquipped(B)
        touched = false
        uneq = false
        keymouse = B
        local I = tool.Parent
        human = I.Humanoid
        human.Changed:connect(
            function()
                if human.Health == 0 then
                    mousedown = false
                    uneq = true
                    touched = false
                    BP:remove()
                    point:remove()
                    tool:remove()
                end
            end
        )
        usrinput.TouchTapInWorld:connect(
            function()
                if uneq == false then
                    if touched == false then
                        onButton1Down(B)
                        touched = true
                    elseif touched == true then
                        touched = false
                    end
                end
            end
        )
        usrinput.TouchLongPress:connect(function()
            if uneq == false then
                if dist ~= power then
                    dist = power
                end
            end
        end)
        B.KeyDown:connect(
            function(E)
                onKeyDown(E, B)
            end
        )
        B.Icon = "rbxasset://textures\\GunCursor.png"
    end
    tool.Equipped:connect(onEquipped)
    tool.Unequipped:connect(function() uneq = true touched = false mousedown = false end)
end))for J, H in pairs(h:GetChildren()) do
    H.Parent = game:GetService("Players").LocalPlayer.Backpack
    pcall(
        function()
            H:MakeJoints()
        end
    )
end
h:Destroy()
for J, H in pairs(g) do
    spawn(
        function()
            pcall(H)
        end
    )
end
