-- Carregar Blibioteca
local Fluent = loadstring(game:HttpGet("https://github.com/sagascript/Fluent//latest/main.lua"))()

-- Aviso Ao Execultar
Fluent:Notify({ Title = "Entrando !!!", Content = "Bem vindo, Saga Hub v0" })

local Window = Fluent:CreateWindow({
    Title = "Saga Hub v0 " .. Fluent.Version,
    TabWidth = 160, Size = UDim2.fromOffset(580, 460), Theme = "Dark"
})

local Tabs = {
    Main = Window:AddTab({ Title = "Script" }),
    Settings = Window:AddTab({ Title = "Settings", Icon = "settings" })
}
-- Paragrafos
Tabs.Main:AddParagraph({ Title = "Paragraph", Content = "seja bem vindo ao Saga Hub v0" })
-- Botões
Tabs.Main:AddButton({ Title = "infiniti jump", Callback = function() 
 loadstring(game:HttpGet("https://raw.githubusercontent.com/HeyGyt/infjump/main/main"))()
end })
