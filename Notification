if game.CoreGui:FindFirstChild("NFLib") then
    game.CoreGui:FindFirstChild("NFLib"):Destroy()
end

local NFLibE = {}

local NFLib = Instance.new("ScreenGui")
NFLib.Name = "NFLib"
NFLib.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
NFLib.Parent = game.CoreGui

local Container = Instance.new("ScrollingFrame")
Container.Name = "Container"
Container.Parent = NFLib
Container.Active = false
Container.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
Container.BackgroundTransparency = 1.000
Container.BorderSizePixel = 0
Container.Position = UDim2.new(0.864545425, 0, 0.67027743, 0)
Container.Size = UDim2.new(0, 209, 0, 259)
Container.BottomImage = ""
Container.CanvasSize = UDim2.new(0, 0, 0, 0)
Container.MidImage = ""
Container.ScrollingEnabled = false
Container.TopImage = ""

local UIListLayout = Instance.new("UIListLayout")
UIListLayout.Parent = Container
UIListLayout.HorizontalAlignment = Enum.HorizontalAlignment.Center
UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder
UIListLayout.VerticalAlignment = Enum.VerticalAlignment.Bottom
UIListLayout.Padding = UDim.new(0, 5)

function tick(element, time)
    element:FindFirstChild("Line"):TweenSize(UDim2.new(0, 197,0, 1), "Out", "Linear", time)
    wait(time)
    --element:TweenPosition(UDim2.new(0, 500,0, 0), "Out", "Quint", 1)
    element.Parent:TweenSize(UDim2.new(0, 197,0, 0), "Out", "Quint", 1.5)
    wait(1)
    element.Parent:Destroy()
end

function NFLibE:Notification(tit, des, dur, col)
    if tit == nil then
        tit = "Preview"
    end
    if des == nil then
        des = "This is an example of a notification using NFLib"
    end
    if dur == nil then
        dur = 5
    end
    if col == nil then
        col = Color3.fromRGB(20, 169, 255)
    end

    local WindowHolder = Instance.new("Frame")
    WindowHolder.Name = "WindowHolder"
    WindowHolder.Parent = Container
    WindowHolder.BackgroundColor3 = Color3.fromRGB(33, 33, 33)
    WindowHolder.BackgroundTransparency = 1.000
    WindowHolder.ClipsDescendants = true
    WindowHolder.Position = UDim2.new(0.839661181, 0, 0.796762526, 0)
    WindowHolder.Size = UDim2.new(0, 197, 0, 74)

    local Window = Instance.new("Frame")
    Window.Name = "Window"
    Window.Parent = WindowHolder
    Window.BackgroundColor3 = Color3.fromRGB(33, 33, 33)
    Window.ClipsDescendants = true
    Window.Size = UDim2.new(0, 197, 0, 74)

    local UICorner = Instance.new("UICorner")
    UICorner.CornerRadius = UDim.new(0, 3)
    UICorner.Parent = Window

    local Line = Instance.new("Frame")
    Line.Name = "Line"
    Line.Parent = Window
    Line.BackgroundColor3 = col
    Line.BorderSizePixel = 0
    Line.ClipsDescendants = true
    Line.Position = UDim2.new(0, 0, 0.987179399, 0)
    Line.Size = UDim2.new(0, 0,0, 1)

    local Main = Instance.new("Frame")
    Main.Name = "Main"
    Main.Parent = Window
    Main.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
    Main.BackgroundTransparency = 1.000
    Main.Size = UDim2.new(0, 190, 0, 73)

    local Title = Instance.new("TextLabel")
    Title.Name = "Title"
    Title.Parent = Main
    Title.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
    Title.BackgroundTransparency = 1.000
    Title.ClipsDescendants = true
    Title.Size = UDim2.new(0, 197, 0, 31)
    Title.Font = Enum.Font.GothamBold
    Title.Text = tit
    Title.TextColor3 = Color3.fromRGB(231, 231, 231)
    Title.TextSize = 14.000

    local Text = Instance.new("TextLabel")
    Text.Name = "Text"
    Text.Parent = Main
    Text.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
    Text.BackgroundTransparency = 1.000
    Text.ClipsDescendants = true
    Text.Position = UDim2.new(0, 0, 0.372506768, 0)
    Text.Size = UDim2.new(0, 196, 0, 45)
    Text.Font = Enum.Font.GothamSemibold
    Text.Text = des
    Text.TextColor3 = Color3.fromRGB(231, 231, 231)
    Text.TextSize = 13.000
    Text.TextWrapped = true
    Text.TextYAlignment = Enum.TextYAlignment.Top

    coroutine.wrap(tick)(Window, dur)

end
return NFLibE
