# RunCMDatBackGround

A C# utility to execute Windows command-line scripts in the background without visible console windows.

![C#](https://img.shields.io/badge/C%23-239120?logo=c-sharp&logoColor=white)

## Features
- Execute batch files/cmd commands silently
- Hide console windows during execution
- Simple .NET Framework implementation
- Lightweight single-project solution

## Installation
1. Clone the repository:
   ```
   git clone https://github.com/irhdab/RunCMDatBackGround.git
   ```
2. Open `cmdhide.sln` in Visual Studio
3. Build the solution (Ctrl+Shift+B)

## Usage
```
// Example code to run a command
ProcessStartInfo startInfo = new ProcessStartInfo();
startInfo.FileName = "cmd.exe";
startInfo.Arguments = "/C your_script.bat";
startInfo.WindowStyle = ProcessWindowStyle.Hidden;
Process.Start(startInfo);
```

Run compiled executable:
```
cmdhide.exe "your_command_here"
```

## Project Structure
```
RunCMDatBackGround/
├── cmdhide/          # Main C# project
│   ├── Program.cs    # Entry point
│   └── ...           # Other source files
├── cmdhide.sln       # Visual Studio solution
└── README.md         # This documentation
```

## Contributing
Contributions are welcome! Please:
1. Fork the repository
2. Create a feature branch
3. Submit a pull request
