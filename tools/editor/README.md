## GamePlay Editor

Cross-platform editor for GamePlay.

## Developer Setup

-  Windows (64-bit)
  * Install Windows 10
  * Install Visual Studio 2015 (https://www.visualstudio.com/en-us/products/visual-studio-community-vs.aspx)
  * Install DirectX SDK (https://www.microsoft.com/en-ca/download/details.aspx?id=6812)
  * Intall Qt 5.6 (http://download.qt.io/official_releases/qt/5.6/5.6.0/) : windows-x86-msvc2015_64
  * Note: Install Qt to default installer path
  
- MacOS X (64-bit)
  * Install MacOS X El Capitan
  * Install XCode 7+ (https://developer.apple.com/xcode/download/) 
  * Intall Qt 5.6  (http://download.qt.io/official_releases/qt/5.6/5.6.0/) : mac-x64-clang
  * Note: Install Qt to default installer path

- Linux (64-bit)
  * Install Ubuntu 15.10 Desktop
  * Intall Qt 5.6 (http://download.qt.io/official_releases/qt/5.6/5.6.0/) : linux-x64
  * Note: Install Qt to default installer path

## Qt Creator (Option A - Linux, MacOS X, Windows)
- Clone gameplay3d.io repo (https://github.com/gameplay3d/GamePlay-nextgen.git)
- Run install.sh or install.bat script
- Open Qt Creator and open the following projects:
	*  GamePlay-nextgen/gameplay/gameplay.pro
	*  GamePlay-nextgen/tools/editor/gameplay-editor.pro
- Configure output paths from big path to "Debug", "Release", "Profile" on both projects
- Build project gameplay
- Build project gameplay-editor
- Set Working directory for project gameplay-editor to "%{buildDir}/.."
- Run gameplay-editor

## Visual Studio 2015 (Option B - Windows only)
- Clone gameplay3d.io repo (https://github.com/gameplay3d/GamePlay-nextgen.git)
- Run install.sh or install.bat script
- Open Visual Studio 2015
- Open menu Tools->Extensions and Updates...
- Search for Qt5Package and install extension.
- Restart Visual Studio 2015
- Open menu QT5->Qt Options
- Add Name=Qt5.6  Path=C:\Qt\Qt5.6.0\5.6\msvc2015_64
- Open GamePlay-nextgen\gameplay.sln
- Build project gameplay-editor (which depends on gameplay)
- Run project gameplay-editor
