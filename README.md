
# Redz UI Library V5 | Ramake 

Uma biblioteca moderna de UI para Roblox, feita em Lua.  
Permite criar **painéis, abas, botões, toggles, sliders, dropdowns e muito mais**, com suporte a **temas customizáveis** e **animações fluidas**.

---

## 📦 Início Rápido

```lua
local redzlib = loadstring(game:HttpGet("URL_DA_LIB_AQUI"))()

-- Criar janela principal
local Window = redzlib:MakeWindow({
    Title = "Meu Hub",
    SubTitle = "powered by redzlib",
    SaveFolder = "MeuHub.json"
})

-- Criar aba
local Tab = Window:MakeTab({ Name = "Principal", Icon = "home" })
```

---

## 🍒 Exemplos de Componentes

### Seção
```lua
Tab:AddSection("Configurações Gerais")
```

### Parágrafo
```lua
Tab:AddParagraph({
    Title = "Aviso",
    Text = "Use com responsabilidade!"
})
```

### Botão
```lua
Tab:AddButton({
    Name = "Executar",
    Description = "Clica aqui para rodar",
    Callback = function()
        print("Botão clicado!")
    end
})
```

### Toggle
```lua
Tab:AddToggle({
    Name = "Ativar Sistema",
    Default = false,
    Callback = function(value)
        print("Toggle:", value)
    end
})
```

### Dropdown
```lua
Tab:AddDropdown({
    Name = "Escolha uma opção",
    Options = {"A", "B", "C"},
    Default = "A",
    Callback = function(option)
        print("Selecionado:", option)
    end
})
```

### Slider
```lua
Tab:AddSlider({
    Name = "Volume",
    Min = 0,
    Max = 100,
    Default = 50,
    Callback = function(value)
        print("Volume:", value)
    end
})
```

---

## Temas

```lua
redzlib:SetTheme("Dark")    -- Dark padrão
redzlib:SetTheme("Purple")  -- Roxo estilizado
redzlib:SetTheme("Darker")  -- Escuro total
```

---

## Notificações

```lua
redzlib:Notify({
    Title = "Sucesso!",
    Description = "Operação concluída.",
    Duration = 5,
    Type = "Info" -- Info, Success, Warning, Error
})
```

## Notify Opcional Image
```Lua
-- normal; 
redzlib:Notify({
    Title = "Sucesso!",
    Description = "Operação concluída.",
    Duration = 5,
    Type = "Success"
})
 -- Image
redzlib:Notify({
    Title = "Sucesso!",
    Description = "Operação concluída.",
    Image = "rbxassetid://",
    Duration = 5,
    Type = "Success"
})
```


---

## 🛠️ Recursos

- ✅ UI totalmente animada com TweenService  
- ✅ Suporte a múltiplos temas  
- ✅ Sistema de salvar configurações (`SaveFolder`)  
- ✅ Notificações integradas  
- ✅ Keybind para minimizar janela  

---

## 📌 Créditos
Criado por **redz9999 & magnus rs**.  
