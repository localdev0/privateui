## Get Stuff
```lua
local lib = {}
local UIColor = Color3.fromRGB(83, 113, 241)

function lib:CreateWindow(title)
	local UI = Instance.new("ScreenGui")
	local Main = Instance.new("Frame")
	local UICorner = Instance.new("UICorner")
	local TopBar = Instance.new("Frame")
	local Title = Instance.new("TextLabel")
	local Icon = Instance.new("ImageLabel")
	local Line = Instance.new("Frame")
	local Navigation = Instance.new("ScrollingFrame")
	local UIListLayout = Instance.new("UIListLayout")
	local UIPadding = Instance.new("UIPadding")
	local Line_2 = Instance.new("Frame")
	local Line_3 = Instance.new("Frame")
	local Content = Instance.new("Frame")
	local PlayerName = Instance.new("TextLabel")
	
	UI.Name = title
	UI.Parent = game:GetService("Players").LocalPlayer.PlayerGui or game:GetService("CoreGui")
	UI.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
	UI.DisplayOrder = 999999999
	UI.ResetOnSpawn = false

	Main.Name = "Main"
	Main.Parent = UI
	Main.BackgroundColor3 = Color3.fromRGB(10, 10, 10)
	Main.BorderColor3 = Color3.fromRGB(0, 0, 0)
	Main.BorderSizePixel = 0
	Main.Position = UDim2.new(0, 387, 0, 150)
	Main.Size = UDim2.new(0, 597, 0, 353)

	UICorner.CornerRadius = UDim.new(0, 6)
	UICorner.Parent = Main

	TopBar.Name = "TopBar"
	TopBar.Parent = Main
	TopBar.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	TopBar.BackgroundTransparency = 1.000
	TopBar.BorderColor3 = Color3.fromRGB(0, 0, 0)
	TopBar.BorderSizePixel = 0
	TopBar.Size = UDim2.new(0, 597, 0, 50)

	Title.Name = "Title"
	Title.Parent = TopBar
	Title.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	Title.BackgroundTransparency = 1.000
	Title.BorderColor3 = Color3.fromRGB(0, 0, 0)
	Title.BorderSizePixel = 0
	Title.Position = UDim2.new(0.102177553, 0, 0.25, 0)
	Title.Size = UDim2.new(0, 180, 0, 26)
	Title.Font = Enum.Font.Gotham
	Title.Text = title
	Title.TextColor3 = Color3.fromRGB(255, 255, 255)
	Title.TextSize = 24.000
	Title.TextXAlignment = Enum.TextXAlignment.Left

	Icon.Name = "Icon"
	Icon.Parent = TopBar
	Icon.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	Icon.BackgroundTransparency = 1.000
	Icon.BorderColor3 = Color3.fromRGB(0, 0, 0)
	Icon.BorderSizePixel = 0
	Icon.Position = UDim2.new(0.0100502511, 0, 0.0599999987, 0)
	Icon.Size = UDim2.new(0, 55, 0, 41)
	Icon.Image = "rbxassetid://70944899239586"
	Icon.ImageColor3 = UIColor

	Line.Name = "Line"
	Line.Parent = Main
	Line.BackgroundColor3 = Color3.fromRGB(51, 51, 51)
	Line.BackgroundTransparency = 0.500
	Line.BorderColor3 = Color3.fromRGB(0, 0, 0)
	Line.BorderSizePixel = 0
	Line.Position = UDim2.new(0, 0, 0.141643062, 0)
	Line.Size = UDim2.new(0, 597, 0, 1)

	Navigation.Name = "Navigation"
	Navigation.Parent = Main
	Navigation.Active = true
	Navigation.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	Navigation.BackgroundTransparency = 1.000
	Navigation.BorderColor3 = Color3.fromRGB(0, 0, 0)
	Navigation.BorderSizePixel = 0
	Navigation.Position = UDim2.new(0, 0, 0.144475922, 0)
	Navigation.Size = UDim2.new(0, 141, 0, 245)
	Navigation.ScrollBarImageColor3 = Color3.fromRGB(0, 0, 0)
	Navigation.CanvasSize = UDim2.new(0, 0, 7, 0)
	Navigation.ScrollBarThickness = 0

	UIListLayout.Parent = Navigation
	UIListLayout.HorizontalAlignment = Enum.HorizontalAlignment.Center
	UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder
	UIListLayout.Padding = UDim.new(0, 4)

	UIPadding.Parent = Navigation
	UIPadding.PaddingTop = UDim.new(0, 8)
	
	Line_2.Name = "Line"
	Line_2.Parent = Main
	Line_2.BackgroundColor3 = Color3.fromRGB(51, 51, 51)
	Line_2.BackgroundTransparency = 0.500
	Line_2.BorderColor3 = Color3.fromRGB(0, 0, 0)
	Line_2.BorderSizePixel = 0
	Line_2.Position = UDim2.new(0.236378625, 0, 0.144475922, 0)
	Line_2.Size = UDim2.new(0, 1, 0, 245)

	Line_3.Name = "Line"
	Line_3.Parent = Main
	Line_3.BackgroundColor3 = Color3.fromRGB(51, 51, 51)
	Line_3.BackgroundTransparency = 0.500
	Line_3.BorderColor3 = Color3.fromRGB(0, 0, 0)
	Line_3.BorderSizePixel = 0
	Line_3.Position = UDim2.new(0, 0, 0.838526905, 0)
	Line_3.Size = UDim2.new(0, 597, 0, 1)

	Content.Name = "Content"
	Content.Parent = Main
	Content.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	Content.BackgroundTransparency = 1.000
	Content.BorderColor3 = Color3.fromRGB(0, 0, 0)
	Content.BorderSizePixel = 0
	Content.Position = UDim2.new(0.237855941, 0, 0.144475922, 0)
	Content.Size = UDim2.new(0, 455, 0, 245)
	
	PlayerName.Name = "PlayerName"
	PlayerName.Parent = Main
	PlayerName.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	PlayerName.BackgroundTransparency = 1.000
	PlayerName.BorderColor3 = Color3.fromRGB(0, 0, 0)
	PlayerName.BorderSizePixel = 0
	PlayerName.Position = UDim2.new(0.0251256283, 0, 0.879886687, 0)
	PlayerName.Size = UDim2.new(0, 180, 0, 26)
	PlayerName.Font = Enum.Font.Gotham
	PlayerName.Text = "Welcome, "..game:GetService("Players").LocalPlayer.Name or game:GetService("Players").LocalPlayer.DisplayName
	PlayerName.TextColor3 = Color3.fromRGB(255, 255, 255)
	PlayerName.TextSize = 20.000
	PlayerName.TextTransparency = 0.700
	PlayerName.TextXAlignment = Enum.TextXAlignment.Left

	local function IGDWXD_script()
		local script = Instance.new('LocalScript', Main)

		local TweenService = game:GetService("TweenService")
		local UserInputService = game:GetService("UserInputService")

		local gui = script.Parent

		local dragging
		local dragInput
		local dragStart
		local startPos

		local tweenInfo = TweenInfo.new(0.16, Enum.EasingStyle.Linear, Enum.EasingDirection.Out)

		local function update(input)
			local delta = input.Position - dragStart
			local targetPos = UDim2.new(
				startPos.X.Scale, 
				startPos.X.Offset + delta.X, 
				startPos.Y.Scale, 
				startPos.Y.Offset + delta.Y
			)

			local tween = TweenService:Create(gui, tweenInfo, {Position = targetPos})
			tween:Play()
		end

		gui.InputBegan:Connect(function(input)
			if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
				dragging = true
				dragStart = input.Position
				startPos = gui.Position

				input.Changed:Connect(function()
					if input.UserInputState == Enum.UserInputState.End then
						dragging = false
					end
				end)
			end
		end)

		gui.InputChanged:Connect(function(input)
			if input.UserInputType == Enum.UserInputType.MouseMovement or input.UserInputType == Enum.UserInputType.Touch then
				dragInput = input
			end
		end)

		UserInputService.InputChanged:Connect(function(input)
			if input == dragInput and dragging then
				update(input)
			end
		end)

		local function toggleGuiVisibility(input)
			if input.UserInputType == Enum.UserInputType.Keyboard and input.KeyCode == Enum.KeyCode.LeftControl then
				gui.Visible = not gui.Visible
			end
		end

		UserInputService.InputBegan:Connect(function(input, gameProcessed)
			if not gameProcessed then
				toggleGuiVisibility(input)
			end
		end)
	end
	coroutine.wrap(IGDWXD_script)()
	
	local ActiveTab = nil
	local SelectedTab = nil

	function lib:CreateTab(title)
		local TabActive_2 = Instance.new("ImageButton")
		local UICorner_3 = Instance.new("UICorner")
		local UIGradient_2 = Instance.new("UIGradient")
		local Title_3 = Instance.new("TextLabel")
		local Items = Instance.new("ScrollingFrame")
		local UIPadding_2 = Instance.new("UIPadding")
		local UIListLayout_2 = Instance.new("UIListLayout")

		TabActive_2.Name = "TabActive"
		TabActive_2.Parent = Navigation
		TabActive_2.BackgroundColor3 = UIColor
		TabActive_2.BackgroundTransparency = 1.000
		TabActive_2.BorderSizePixel = 0
		TabActive_2.Size = UDim2.new(0, 129, 0, 32)
		TabActive_2.AutoButtonColor = false

		UICorner_3.CornerRadius = UDim.new(0, 6)
		UICorner_3.Parent = TabActive_2

		UIGradient_2.Color = ColorSequence.new({
			ColorSequenceKeypoint.new(0.00, Color3.fromRGB(255, 255, 255)),
			ColorSequenceKeypoint.new(1.00, Color3.fromRGB(87, 102, 125))
		})
		UIGradient_2.Rotation = 180
		UIGradient_2.Parent = TabActive_2

		Title_3.Name = "Title"
		Title_3.Parent = TabActive_2
		Title_3.BackgroundTransparency = 1.000
		Title_3.Size = UDim2.new(0, 122, 0, 32)
		Title_3.Font = Enum.Font.Gotham
		Title_3.Text = title
		Title_3.TextColor3 = Color3.fromRGB(51, 51, 51)
		Title_3.TextSize = 18.000
		Title_3.TextXAlignment = Enum.TextXAlignment.Left
		Title_3.Position = UDim2.new(0.0542635657, 0, 0, 0)

		Items.Name = title
		Items.Parent = Content
		Items.BackgroundTransparency = 1.000
		Items.Size = UDim2.new(0, 455, 0, 245)
		Items.ScrollBarThickness = 0
		Items.Visible = false
		Items.CanvasSize = UDim2.new(0, 0, 15, 0)

		UIPadding_2.Parent = Items
		UIPadding_2.PaddingTop = UDim.new(0, 2)

		UIListLayout_2.Parent = Items
		UIListLayout_2.HorizontalAlignment = Enum.HorizontalAlignment.Center
		UIListLayout_2.SortOrder = Enum.SortOrder.LayoutOrder
		UIListLayout_2.Padding = UDim.new(0, 6)

		if not ActiveTab then
			ActiveTab = TabActive_2
			SelectedTab = Items
			TabActive_2.BackgroundTransparency = 0
			Title_3.TextColor3 = Color3.fromRGB(0, 0, 0)
			Items.Visible = true
			Items.Size = UDim2.new(0, 455, 0, 70)
			Items:TweenSize(UDim2.new(0, 455, 0, 245), Enum.EasingDirection.Out, Enum.EasingStyle.Quad, 0.55, true)
		end

		TabActive_2.MouseButton1Click:Connect(function()
			if ActiveTab ~= TabActive_2 then
				ActiveTab.BackgroundTransparency = 1
				ActiveTab.Title.TextColor3 = Color3.fromRGB(51, 51, 51)
				SelectedTab.Visible = false

				ActiveTab = TabActive_2
				SelectedTab = Items
				TabActive_2.BackgroundTransparency = 0
				Title_3.TextColor3 = Color3.fromRGB(0, 0, 0)
				Items.Visible = true
				Items.Size = UDim2.new(0, 455, 0, 70)
				Items:TweenSize(UDim2.new(0, 455, 0, 245), Enum.EasingDirection.Out, Enum.EasingStyle.Quad, 0.55, true)
			end
		end)

		return Items
	end
	
	function lib:CreateSection(title,TabParent)
		local Section = Instance.new("TextLabel")
		
		Section.Name = "Section"
		Section.Parent = TabParent
		Section.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		Section.BackgroundTransparency = 1.000
		Section.BorderColor3 = Color3.fromRGB(0, 0, 0)
		Section.BorderSizePixel = 0
		Section.Position = UDim2.new(0.0241758246, 0, 0, 0)
		Section.Size = UDim2.new(0, 433, 0, 23)
		Section.Font = Enum.Font.Gotham
		Section.Text = title
		Section.TextColor3 = Color3.fromRGB(51, 51, 51)
		Section.TextSize = 18.000
		Section.TextXAlignment = Enum.TextXAlignment.Left
	end
	
	function lib:CreateButton(title, TabParent, callback)
		local Button = Instance.new("ImageButton")
		local UICorner_17 = Instance.new("UICorner")
		local Title_13 = Instance.new("TextLabel")
		local MouseIcon = Instance.new("ImageLabel")
		local UIAspectRatioConstraint_3 = Instance.new("UIAspectRatioConstraint")
		local TweenService = game:GetService("TweenService")

		Button.Name = "Button"
		Button.Parent = TabParent
		Button.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
		Button.BorderColor3 = Color3.fromRGB(0, 0, 0)
		Button.BorderSizePixel = 0
		Button.Position = UDim2.new(0.0230769236, 0, 0.0452674888, 0)
		Button.Size = UDim2.new(0, 434, 0, 38)
		Button.AutoButtonColor = false

		UICorner_17.Parent = Button

		Title_13.Name = "Title"
		Title_13.Parent = Button
		Title_13.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		Title_13.BackgroundTransparency = 1.000
		Title_13.BorderColor3 = Color3.fromRGB(0, 0, 0)
		Title_13.BorderSizePixel = 0
		Title_13.Position = UDim2.new(0.00115207373, 0, 0, 0)
		Title_13.Size = UDim2.new(0, 432, 0, 38)
		Title_13.Font = Enum.Font.Gotham
		Title_13.Text = title
		Title_13.TextColor3 = Color3.fromRGB(255, 255, 255)
		Title_13.TextSize = 19.000
		Title_13.TextWrapped = true

		MouseIcon.Name = "MouseIcon"
		MouseIcon.Parent = Button
		MouseIcon.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		MouseIcon.BackgroundTransparency = 1.000
		MouseIcon.BorderColor3 = Color3.fromRGB(0, 0, 0)
		MouseIcon.BorderSizePixel = 0
		MouseIcon.Position = UDim2.new(0.935483873, 0, 0.210526317, 0)
		MouseIcon.Size = UDim2.new(0, 35, 0, 21)
		MouseIcon.Image = "rbxassetid://12804017021"
		MouseIcon.ImageColor3 = UIColor

		UIAspectRatioConstraint_3.Parent = MouseIcon

		local function setButtonColor(color)
			local tweenInfo = TweenInfo.new(0.2, Enum.EasingStyle.Quad, Enum.EasingDirection.Out)
			local goal = { BackgroundColor3 = color }
			local tween = TweenService:Create(Button, tweenInfo, goal)
			tween:Play()
		end

		Button.MouseEnter:Connect(function()
			setButtonColor(Color3.fromRGB(4, 4, 4))
		end)

		Button.MouseLeave:Connect(function()
			setButtonColor(Color3.fromRGB(0, 0, 0))
		end)

		Button.TouchTap:Connect(function()
			if callback then
				callback()
			end
		end)

		Button.MouseButton1Click:Connect(function()
			if callback then
				callback()
			end
		end)

		return Button
	end
	
	function lib:CreateToggle(title, TabParent, default, callback)
		local Toggle = Instance.new("ImageButton")
		local UICorner_6 = Instance.new("UICorner")
		local Title_5 = Instance.new("TextLabel")
		local Checkbox_2 = Instance.new("Frame")
		local UICorner_7 = Instance.new("UICorner")
		local UIStroke_2 = Instance.new("UIStroke")
		local UIAspectRatioConstraint_2 = Instance.new("UIAspectRatioConstraint")

		Toggle.Name = "Toggle"
		Toggle.Parent = TabParent
		Toggle.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
		Toggle.BorderSizePixel = 0
		Toggle.Size = UDim2.new(0, 434, 0, 38)
		Toggle.AutoButtonColor = false

		UICorner_6.Parent = Toggle

		Title_5.Name = "Title"
		Title_5.Parent = Toggle
		Title_5.BackgroundTransparency = 1
		Title_5.Size = UDim2.new(0, 133, 0, 38)
		Title_5.Font = Enum.Font.Gotham
		Title_5.Text = title
		Title_5.TextColor3 = Color3.fromRGB(255, 255, 255)
		Title_5.TextSize = 19
		Title_5.TextTransparency = default and 0 or 0.6
		Title_5.TextXAlignment = Enum.TextXAlignment.Left
		Title_5.Position = UDim2.new(0.0289180074, 0, 0, 0)

		Checkbox_2.Name = "Checkbox"
		Checkbox_2.Parent = Toggle
		Checkbox_2.BackgroundColor3 = default and UIColor or Color3.fromRGB(10, 10, 10)
		Checkbox_2.BorderSizePixel = 0
		Checkbox_2.Position = UDim2.new(0.914, 0, 0.132, 0)
		Checkbox_2.Size = UDim2.new(0, 30, 0, 31)

		UICorner_7.CornerRadius = UDim.new(0, 4)
		UICorner_7.Parent = Checkbox_2

		UIStroke_2.Parent = Checkbox_2

		UIAspectRatioConstraint_2.Parent = Checkbox_2
		UIAspectRatioConstraint_2.AspectRatio = 1.11

		local state = default
		local TweenService = game:GetService("TweenService")

		local function updateToggle()
			local titleTween = TweenService:Create(Title_5, TweenInfo.new(0.3), {
				TextTransparency = state and 0 or 0.6
			})
			local checkboxTween = TweenService:Create(Checkbox_2, TweenInfo.new(0.3), {
				BackgroundColor3 = state and UIColor or Color3.fromRGB(10, 10, 10)
			})

			titleTween:Play()
			checkboxTween:Play()

			if callback then
				callback(state)
			end
		end

		Toggle.MouseButton1Click:Connect(function()
			state = not state
			updateToggle()
		end)

		updateToggle()
	end
	
	function lib:CreateSlider(title, TabParent, min, max, default, callback)
		local Slider = Instance.new("ImageButton")
		local UICorner_8 = Instance.new("UICorner")
		local Title_6 = Instance.new("TextLabel")
		local SliderBack = Instance.new("Frame")
		local UICorner_9 = Instance.new("UICorner")
		local Draggable = Instance.new("Frame")
		local UICorner_10 = Instance.new("UICorner")
		local Value = Instance.new("TextLabel")

		Slider.Name = "Slider"
		Slider.Parent = TabParent
		Slider.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
		Slider.BorderColor3 = Color3.fromRGB(0, 0, 0)
		Slider.BorderSizePixel = 0
		Slider.Position = UDim2.new(0.0230769236, 0, 0.111111112, 0)
		Slider.Size = UDim2.new(0, 434, 0, 38)
		Slider.AutoButtonColor = false

		UICorner_8.Parent = Slider

		Title_6.Name = "Title"
		Title_6.Parent = Slider
		Title_6.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		Title_6.BackgroundTransparency = 1.000
		Title_6.BorderColor3 = Color3.fromRGB(0, 0, 0)
		Title_6.BorderSizePixel = 0
		Title_6.Position = UDim2.new(0.0289180074, 0, 0, 0)
		Title_6.Size = UDim2.new(0, 133, 0, 38)
		Title_6.Font = Enum.Font.Gotham
		Title_6.Text = title
		Title_6.TextColor3 = Color3.fromRGB(255, 255, 255)
		Title_6.TextSize = 19.000
		Title_6.TextWrapped = true
		Title_6.TextXAlignment = Enum.TextXAlignment.Left

		SliderBack.Name = "SliderBack"
		SliderBack.Parent = Slider
		SliderBack.BackgroundColor3 = Color3.fromRGB(10, 10, 10)
		SliderBack.BorderColor3 = Color3.fromRGB(0, 0, 0)
		SliderBack.BorderSizePixel = 0
		SliderBack.Position = UDim2.new(0.523041487, 0, 0.395, 0)
		SliderBack.Size = UDim2.new(0, 200, 0, 8)

		UICorner_9.CornerRadius = UDim.new(0, 15)
		UICorner_9.Parent = SliderBack

		Draggable.Name = "Draggable"
		Draggable.Parent = SliderBack
		Draggable.BackgroundColor3 = UIColor
		Draggable.BorderColor3 = Color3.fromRGB(0, 0, 0)
		Draggable.BorderSizePixel = 0
		Draggable.Position = UDim2.new(-0.00195861817, 0, -0.0413534977, 0)
		Draggable.Size = UDim2.new(0, 164, 0, 8)

		UICorner_10.CornerRadius = UDim.new(0, 15)
		UICorner_10.Parent = Draggable

		Value.Name = "Value"
		Value.Parent = Slider
		Value.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		Value.BackgroundTransparency = 1.000
		Value.BorderColor3 = Color3.fromRGB(0, 0, 0)
		Value.BorderSizePixel = 0
		Value.Position = UDim2.new(0.434447974, 0, 0, 0)
		Value.Size = UDim2.new(0, 32, 0, 38)
		Value.Font = Enum.Font.Gotham
		Value.Text = "100.0"
		Value.TextColor3 = Color3.fromRGB(255, 255, 255)
		Value.TextSize = 19.000
		Value.TextTransparency = 0.200
		Value.TextXAlignment = Enum.TextXAlignment.Right

		local UIS = game:GetService("UserInputService")
		local TweenService = game:GetService("TweenService")

		local currentValue = min
		local isDragging = false
		local touchID = nil

		local function UpdateSliderPosition()
			local percentage = math.clamp((currentValue - min) / (max - min), 0, 1)
			Value.Text = string.format("%.1f", currentValue)

			local targetSize = UDim2.new(percentage, 0, 1, 0)
			local tween = TweenService:Create(Draggable, TweenInfo.new(0.3, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {Size = targetSize})
			tween:Play()
			callback(currentValue)
		end

		local function StartDragging(input)
			isDragging = true
			if input.UserInputType == Enum.UserInputType.Touch then
				touchID = input.UserInputIndex
			end
		end

		local function UpdateDragging(input)
			if not isDragging then return end

			local inputPosition
			if input.UserInputType == Enum.UserInputType.MouseMovement or
				input.UserInputType == Enum.UserInputType.Touch then
				inputPosition = input.Position.X
			end

			if inputPosition then
				local sliderX = SliderBack.AbsolutePosition.X
				local sliderWidth = SliderBack.AbsoluteSize.X
				local newPercentage = math.clamp((inputPosition - sliderX) / sliderWidth, 0, 1)
				currentValue = min + (newPercentage * (max - min))
				currentValue = math.round(currentValue * 10) / 10
				UpdateSliderPosition()
			end
		end

		local function StopDragging(input)
			if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
				isDragging = false
				touchID = nil
			end
		end

		Slider.MouseButton1Down:Connect(StartDragging)
		UIS.InputChanged:Connect(UpdateDragging)
		UIS.InputEnded:Connect(StopDragging)

		currentValue = default
		UpdateSliderPosition()
	end
	
	function lib:CreateDropdown(title, TabParent, options, default, callback)
		local Dropdown = Instance.new("ImageButton")
		local UICorner_14 = Instance.new("UICorner")
		local Title_10 = Instance.new("TextLabel")
		local OptionHolder_2 = Instance.new("ScrollingFrame")
		local UIListLayout_4 = Instance.new("UIListLayout")
		local UIPadding_4 = Instance.new("UIPadding")

		Dropdown.Name = "Dropdown"
		Dropdown.Parent = TabParent
		Dropdown.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
		Dropdown.BorderColor3 = Color3.fromRGB(0, 0, 0)
		Dropdown.BorderSizePixel = 0
		Dropdown.Position = UDim2.new(0.0230769236, 0, 0.0452674888, 0)
		Dropdown.Size = UDim2.new(0, 434, 0, 38)
		Dropdown.AutoButtonColor = false

		UICorner_14.Parent = Dropdown

		Title_10.Name = "Title"
		Title_10.Parent = Dropdown
		Title_10.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		Title_10.BackgroundTransparency = 1.000
		Title_10.BorderColor3 = Color3.fromRGB(0, 0, 0)
		Title_10.BorderSizePixel = 0
		Title_10.Position = UDim2.new(0.00115207373, 0, 0, 0)
		Title_10.Size = UDim2.new(0, 432, 0, 38)
		Title_10.Font = Enum.Font.Gotham
		Title_10.Text = title
		Title_10.TextColor3 = Color3.fromRGB(255, 255, 255)
		Title_10.TextSize = 19.000
		Title_10.TextWrapped = true

		OptionHolder_2.Name = "OptionHolder"
		OptionHolder_2.Parent = Dropdown
		OptionHolder_2.Active = true
		OptionHolder_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		OptionHolder_2.BackgroundTransparency = 0.950
		OptionHolder_2.BorderColor3 = Color3.fromRGB(0, 0, 0)
		OptionHolder_2.BorderSizePixel = 0
		OptionHolder_2.Position = UDim2.new(0.0197014175, 0, 0.267605215, 0)
		OptionHolder_2.Size = UDim2.new(0, 418, 0, 0)
		OptionHolder_2.ScrollBarImageColor3 = Color3.fromRGB(0, 0, 0)
		OptionHolder_2.CanvasSize = UDim2.new(0, 0, 1.1, 0)
		OptionHolder_2.ScrollBarThickness = 0

		UIListLayout_4.Parent = OptionHolder_2
		UIListLayout_4.HorizontalAlignment = Enum.HorizontalAlignment.Center
		UIListLayout_4.SortOrder = Enum.SortOrder.LayoutOrder
		UIListLayout_4.Padding = UDim.new(0, 4)

		UIPadding_4.Parent = OptionHolder_2
		UIPadding_4.PaddingTop = UDim.new(0, 6)

		local function openDropdown()
			Dropdown:TweenSize(UDim2.new(0, 434, 0, 142), "Out", "Quad", 0.2, true)
			OptionHolder_2:TweenSize(UDim2.new(0, 418, 0, 92), "Out", "Quad", 0.2, true)
		end

		local function closeDropdown()
			Dropdown:TweenSize(UDim2.new(0, 434, 0, 38), "Out", "Quad", 0.2, true)
			OptionHolder_2:TweenSize(UDim2.new(0, 418, 0, 0), "Out", "Quad", 0.2, true)
		end

		Dropdown.MouseButton1Click:Connect(function()
			if OptionHolder_2.Size.Y.Scale == 0 then
				openDropdown()
			else
				closeDropdown()
			end
		end)
		
		local TweenService = game:GetService("TweenService")
		
		for _, option in ipairs(options) do
			local OptionButton_2 = Instance.new("ImageButton")
			local UICorner_15 = Instance.new("UICorner")
			local Title_11 = Instance.new("TextLabel")
			local UIStroke_5 = Instance.new("UIStroke")

			OptionButton_2.Name = "OptionButton"
			OptionButton_2.Parent = OptionHolder_2
			OptionButton_2.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
			OptionButton_2.BorderColor3 = Color3.fromRGB(0, 0, 0)
			OptionButton_2.BorderSizePixel = 0
			OptionButton_2.Size = UDim2.new(0, 408, 0, 34)
			OptionButton_2.AutoButtonColor = false
			OptionButton_2.ImageTransparency = 1

			UICorner_15.Parent = OptionButton_2
			
			UIStroke_5.Parent = OptionButton_2
			UIStroke_5.Color = UIColor
			UIStroke_5.Transparency = 1.000
			UIStroke_5.Thickness = 0.500

			Title_11.Name = "Title"
			Title_11.Parent = OptionButton_2
			Title_11.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
			Title_11.BackgroundTransparency = 1.000
			Title_11.BorderColor3 = Color3.fromRGB(0, 0, 0)
			Title_11.BorderSizePixel = 0
			Title_11.Size = UDim2.new(0, 408, 0, 34)
			Title_11.Font = Enum.Font.Gotham
			Title_11.Text = option
			Title_11.TextColor3 = Color3.fromRGB(255, 255, 255)
			Title_11.TextSize = 19.000
			Title_11.TextWrapped = true

			UIStroke_5.Parent = OptionButton_2
			UIStroke_5.Transparency = 1
			
			local hoverTweenInfo = TweenInfo.new(0.7, Enum.EasingStyle.Quint, Enum.EasingDirection.Out)
			local normalTweenInfo = TweenInfo.new(0.7, Enum.EasingStyle.Quint, Enum.EasingDirection.Out)

			local hoverTween = TweenService:Create(UIStroke_5, hoverTweenInfo, {
				Thickness = 1, 
				Transparency = 0
			})
			local normalTween = TweenService:Create(UIStroke_5, normalTweenInfo, {
				Thickness = 0,
				Transparency = 1
			})

			OptionButton_2.MouseEnter:Connect(function()
				hoverTween:Play()
			end)

			OptionButton_2.MouseLeave:Connect(function()
				normalTween:Play()
			end)

			OptionButton_2.MouseButton1Click:Connect(function()
				callback(option)
				closeDropdown()
			end)
		end
	end

	return lib
end
```
## Create Title
```lua
lib:CreateWindow("Thunder.lol")
```
## Create Tab
```lua
local tab1 = lib:CreateTab("Catching")
local tab2 = lib:CreateTab("Player")
```
## Create Section
```lua
local sec1 = lib:CreateSection("Magnets",tab1)
```
## Create Button
```lua
lib:CreateButton("Promote",tab1,function(callback)
	print("Clicked")
end)
```
## Create Toggle
```lua
lib:CreateToggle("Magnets",tab1,false,function(state)
	print(state)
end)
```
## Create Slider
```lua
lib:CreateSlider("Magnet Range",tab1,0,25,0,function(value)
	print(value)
end)
```
## Create Dropdown
```lua
local options = {"test", "ing"}
lib:CreateDropdown("Magnet Mode",tab1,options,options[1],function(Selected)
	print(Selected)
end)
```
