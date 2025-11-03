## Damka (Checkers) – Console Application

A C# console-based Damka (Checkers) game. The project includes core game logic (board, moves, players, sessions) and a console UI. It can be opened with Visual Studio or built and run using the .NET CLI.

### 🎬 DamkaGame Demo
https://github.com/francisziv/DamkaGame/blob/main/DamkaGame-demo.mp4

### Features

- Classic Damka rules with piece movement and captures
- Turn management and game session handling
- Console-based UI

### Project Structure

- `Damka-Project/`
  - `Logical/` – core game logic (`GameBoard`, `GameManager`, `GameSession`, `Player`, `Move`, `Coin`, `PointOnBoard`)
  - `UI/` – console UI entry (`ConsoleGame`)
  - `Enums/` – enums (`eBoardStyle`, `eGameState`)
  - `Program.cs` – application entry point
  - `Ex02.csproj` – C# project file
- `DamkaGame.sln` – solution file for Visual Studio
- `Ex02.ConsoleUtils.dll` – console utilities dependency

### Requirements

- Windows 10/11
- One of the following:
  - Visual Studio 2022 (or newer) with .NET desktop workload
  - .NET SDK (6 or later recommended) for CLI usage

### Getting Started

#### Option 1: Visual Studio

1. Open the solution:
   - Double-click `DamkaGame.sln` (or open via File → Open → Project/Solution).
2. Set startup project (if needed): Right-click `Damka-Project` → Set as Startup Project.
3. Build and run: Press `F5` (Debug) or `Ctrl+F5` (Run without debugging).

#### Option 2: .NET CLI (PowerShell)

From the repository root (`damkaGame`):

```powershell
# Restore, build, and run the console app
dotnet restore "Damka-Project/Ex02.csproj"
dotnet build   "Damka-Project/Ex02.csproj" -c Release
dotnet run     --project "Damka-Project/Ex02.csproj"
```

If you prefer running via the solution:

```powershell
dotnet build "DamkaGame.sln" -c Release
dotnet run --project "Damka-Project/Ex02.csproj"
```

### Usage

- Follow on-screen prompts in the console UI to start a new game.
- Input is via keyboard; the UI guides move selection and game flow.

### Notes

- If the project targets an older .NET Framework, use Visual Studio to build and run.
- `Ex02.ConsoleUtils.dll` is shipped alongside and should be resolved by the project; ensure it remains next to the solution/project.

### License

This project is provided as-is for educational purposes. Add a license if you intend to distribute.
