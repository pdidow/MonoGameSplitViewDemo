MonoGame Split Viewport Demo
A demonstration project showing how to implement split viewports in MonoGame, featuring a main game view alongside an information panel. This setup is particularly useful for games that need to display real-time statistics, inventory systems, or other information separate from the main game view.
Features

Split screen implementation with customizable viewport ratios
Main game viewport (75% of screen width)
Information panel viewport (25% of screen width)
Custom border rendering for the info panel
Real-time environmental information display
Proper viewport management and rendering

Technical Implementation
The project demonstrates several key MonoGame concepts:

Multiple viewport management
SpriteBatch state management
Custom texture creation for borders
Text rendering with SpriteFont
Proper GraphicsDevice viewport switching

Project Structure
The main game class handles:

Viewport creation and management
Content loading (textures and fonts)
Separate drawing methods for game and info panel
Custom border rendering system

Getting Started
Prerequisites

MonoGame Framework (latest version)
Visual Studio 2019 or later
.NET 6.0 or later

Setup

Clone the repository
Open the solution in Visual Studio
Restore NuGet packages
Build and run the project

Required Content
Make sure your Content project includes:

A SpriteFont file named "Inkfree_20"
A texture file named "GameTexture"

Usage
The viewport split is handled automatically on startup. The game view takes up 75% of the screen width, while the info panel occupies the remaining 25%.
To modify the viewport ratio, adjust the calculation in the Initialize method:
csharp
