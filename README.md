


<div align="center">

![Logo](https://media.discordapp.net/attachments/1047624099565949079/1113601108565303407/1zKKPGX.png)


<div>&nbsp;</div>


[![Discord server](https://img.shields.io/discord/1047610578740465684?label=Discord&logo=Discord&logoColor=white&style=for-the-badge)](https://discord.gg/r5VaTq5V "A Discord server where people can discuss Adonis related stuff and talk.") 
![Commits](https://img.shields.io/github/commit-activity/t/synnyyy/refine?style=for-the-badge)
![Forks](https://img.shields.io/github/forks/synnyyy/refine?style=for-the-badge)
![Stars](https://img.shields.io/github/stars/synnyyy/refine?style=for-the-badge)
![License](https://img.shields.io/endpoint?label=License&logoColor=blue&style=for-the-badge&url=https%3A%2F%2Fpastebin.com%2Fraw%2F54sUYpzT)



</div>


# 🚀 What is Refine?
Refine is a powerful module designed for Roblox exploit script developers. It aims to enhance code efficiency and readability by providing a streamlined scripting experience. With Refine, developers can focus on implementing functionality while reducing repetitive tasks and improving productivity.

## 📚 Table of Contents

- [Installation & Usage](#installation-&-usage)
- [Features](#features)
  - [Accessing ROBLOX Services](#accessing-roblox-services)
  - [Useful Functions](#functions)
- [Community and Support](#community-and-support)
- [Contributing](#contributing)



### 🛠️ Installation & Usage

To start using the Refine library, follow these steps:

1) Load the Refine library by using the loadstring function with the provided URL. Place this code at the beginning of your script:
```lua
local Refine = loadstring(game:HttpGet("https://raw.githubusercontent.com/synnyyy/refine/main/project.lua", true))()
Refine:Load() -- Loads the Refine module.
```
2) You are now set.


### 🔒 Accessing Roblox Services

To efficiently access Roblox services and ensure security, you can utilize the Refine library's `Services` feature. By doing so, you can easily define and cache the services you need for your script. Here's an example:

```lua
-- Accessing Roblox services using Refine

local ReplicatedStorage = Refine.Services.ReplicatedStorage
local HttpService = Refine.Services.HttpService
local Network = Refine.Services.NetworkService
```
In the above example, we declare and assign the desired Roblox services using the Refine library. By using Refine.Services, you can directly access various services such as `ReplicatedStorage`, `HttpService` and `Network` 

> ⚡ These service objects are cached for efficiency, ensuring better performance in your script.

## 🧰 Functions
Refine provides a comprehensive set of 40+ built-in functions that are designed to make your scripting tasks easier. These functions cover a wide range of functionalities and are readily available for you to use. 

Here's an overview of the functions included in Refine:


#### Load
This loads the Refine Module.
```lua
Refine:Load()
```



#### GetPlayer
This gets the player or specified player instance (by name)
```lua
Refine:GetPlayer(target)
```
- **Arguments**
    - `target` (optional): Gets another specified player instance by name. If not provided, the current player instance is returned.

- **Returns**
    - `Instance` or `nil` if not found.

  

#### GetPlayerCharacter
This function gets the player's or specified player's character.
```lua
Refine:GetPlayerCharacter(target)
```
- **Arguments**
    - `target` (optional): Gets another player's character. If not specified, it will return the current player's character.

- **Returns**
    - `Instance` or `nil` if not found.


#### GetPlayerRoot
This function gets the player's or specified player's HumanoidRootPart.
```lua
Refine:GetPlayerRoot(target)
```
- **Arguments**
    - `target` (optional): Gets another player's HRP. If not specified, it will return the current player's HRP.

- **Returns**
    - `Instance` or `nil` if not found.

#### GetPlayerHumanoid
This function gets the player's or specified player's Humanoid.
```lua
Refine:GetPlayerHumanoid(target)
```
- **Arguments**
    - `target` (optional): Gets another player's humanoid. If not specified, it will return the current player's humanoid.

- **Returns**
    - `Instance` or `nil` if not found.

#### GetPlayerCFrame
This function returns the player's or specified player's CFrame.
```lua
Refine:GetPlayerCFrame(target)
```
- **Arguments**
    - `target` (optional): Gets another player's CFrame. If not specified, it will return the current player's CFrame.

- **Returns**
    - `CFrame` or `nil` if not found.

> Aliases include `GetCFR` and `GetPlayerCFrame`

#### GetPlayerPosition
This function returns the player's or specified player's Position.
```lua
Refine:GetPlayerPosition(target)
```
- **Arguments**
    - `target` (optional): Gets another player's position. If not specified, it will return the current player's position.

- **Returns**
    - `CFrame.Position` or `nil` if not found.

> Aliases include `GetPos` and `GetPlayerPosition`.


#### TeleportPlayer
This function teleports the local player to the specified position.
```lua
Refine:TeleportPlayer(x, y, z)
```
- **Arguments**
    - `x` : Determines X Position.
    - `y` : Determines Y Position.
    - `z` : Determines Z Position.

#### TweenPlayer
This function tweens the local player to the specified position.
```lua
Refine:TweenPlayer(x, y, z, time)
```
- **Arguments**
    - `x` : Determines X Position.
    - `y` : Determines Y Position.
    - `z` : Determines Z Position.
    - `time` : Time taken to reach to the specified position.

#### Pathfind
This function uses natural pathfinding in order to get to the specified position.
```lua
Refine:Pathfind(x, y, z)
```
- **Arguments**
    - `x` : Determines X Position.
    - `y` : Determines Y Position.
    - `z` : Determines Z Position.

#### SetWalkspeed
This function sets the walkspeed of the local player to the specified `speed` value.
```lua
Refine:SetWalkSpeed(speed)
```
- **Arguments**
    - `speed` : Determines the speed.

#### SetJumpPower
This function sets the jump power of the local player to the specified `power` value.
```lua
Refine:SetJumpPower(power)
```
- **Arguments**
    - `power` : Determines the jump power.

#### ResetPlayer
This function kills the player.
```lua
Refine:ResetPlayer()
```

#### GetPlayerHealth
This function gets the player health or a specified player's health.
```lua
Refine:GetPlayerHealth(target)
```
- **Arguments**
    - `target` (optional): Gets another player's health. If not specified, it will return the current player's health.

- **Returns**
    - `integer` or `nil` if not found.

#### IsPlayerAlive
This function gets the player health or a specified player's health.
```lua
Refine:IsPlayerAlive(target)
```
- **Arguments**
    - `target` (optional): Lets you know if a player is alive. If not specified, will return if the local player is alive or not.

- **Returns**
    - `bool`






