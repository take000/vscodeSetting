# vscodeSetting
## 拡張機能インストール
C/C++
Bracket Pair Colorizer 2

## c_cpp_properties.json
```json
{
    "configurations": [
        {
            "name": "Win32",
            "includePath": [
                "${workspaceFolder}/**",
                "C:/Program Files/mingw-w64/x86_64-8.1.0-posix-seh-rt_v6-rev0/mingw64/lib/gcc/x86_64-w64-mingw32/8.1.0/include/c++/x86_64-w64-mingw32/"
            ],
            "defines": [
                "_DEBUG",
                "UNICODE",
                "_UNICODE"
            ],
            "windowsSdkVersion": "10.0.18362.0",
            "compilerPath": "C:/Program Files/mingw-w64/x86_64-8.1.0-posix-seh-rt_v6-rev0/mingw64/bin/g++.exe",
            "cStandard": "c11",
            "cppStandard": "c++17",
            "intelliSenseMode": "gcc-x64"
        }
    ],
    "version": 4
}
```

## tasks.json
```json
{
    // See https://go.microsoft.com/fwlink/?LinkId=733558
    // for the documentation about the tasks.json format
    "version": "2.0.0",
    "tasks": [
        {
            "label": "build",
            "type": "shell",
            "command": "g++",
            "args": [
                "${fileBasename}",
                "-o",
                "${fileBasenameNoExtension}.exe",
                ";",
                "./${fileBasenameNoExtension}.exe"
            ],
            "group": {
                "kind": "build",
                "isDefault": true
            }
        }
    ]
}
```

## keybindings.json
```json 
[
    {
        "key": "shift+enter",
        "command": "workbench.action.terminal.focus",
        "when": "editorTextFocus"
    },
    {
        "key": "shift+enter",
        "command": "workbench.action.focusFirstEditorGroup",
        "when": "terminalFocus"
    }
]
```

## settings.json
```json
{
    "C_Cpp.clang_format_style": "{BasedOnStyle: LLVM, UseTab: Never, IndentWidth: 4, TabWidth: 4,BreakBeforeBraces: Allman,AllowShortIfStatementsOnASingleLine: false,IndentCaseLabels: false,ColumnLimit: 0,AccessModifierOffset: -4,BreakBeforeBraces: Attach}",
    "editor.formatOnSave": true,
    "editor.formatOnType": true,
}
```
