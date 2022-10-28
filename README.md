# vscode Settings

When you use vscode for any projects, it will, usually, automatically create a hidden folder called `.vscode` in your project directory.  
Inside of this folder, there is usually two json files, namely, `c_cpp_properties.json` and `settings.json`.  
The example given here is a cpp project, therefore, there is the `c_cpp_properties.json` file.  

## Customizing Local Editor Font Size

settings.json
```json
{
    "python.autoComplete.extraPaths": [
        "/opt/ros/melodic/lib/python2.7/dist-packages"
    ],
    "window.zoomLevel": 1.5
}
```

## Customizing Functionality

Please also visit [vim](https://github.com/BruceChanJianLe/vim) repository for some cool vim shortcut to be written in `settings.json`.  
```json
{
    "python.defaultInterpreterPath": "/usr/bin/python3",
    "editor.lineNumbers": "relative",
    "cmake.configureOnOpen": true,
    "cmake.buildDirectory": "${workspaceFolder}/build-vscode",
    "testMate.cpp.log.userId": "82cdd95340a0c3075fb44e7c043c393e1bdb7a70",
    "testMate.cpp.log.logSentry": "disable_3",
    "vim.leader": "<space>",
    "vim.vimrc.enable": true,
    "vim.vimrc.path": "/home/chanjl/.vimrc",
    "scm.defaultViewMode": "tree",
    "vim.normalModeKeyBindingsNonRecursive": [
            {
                "before": ["<leader>", "w"],
                "commands": ["workbench.action.files.saveFiles"]
            },
            {
                "before": ["<leader>", "x"],
                "commands": ["workbench.action.files.saveFiles","workbench.action.closeActiveEditor"]
            },
            {
                "before": ["<leader>", "r"],
                "after": ["%s///gc<Left><Left><Left>"]
            },
            {
                "before": ["<leader>", "<leader>", "r"],
                "after": ["%s///g<Left><Left>"]
            },
            {
                "before": ["<leader>", "e"],
                "after": [":e!"]
            },
            {
                "before": ["<leader>", "q"],
                "commands": ["workbench.action.closeActiveEditor"]
            },
            {
                "before": ["<leader>", "z"],
                "commands": ["workbench.action.toggleEditorWidths"] 
            },
            {
                "before": ["<leader>", "h"],
                "commands": ["workbench.action.navigateLeft"]
            },
            {
                "before": ["<leader>", "j"],
                "commands": ["workbench.action.navigateDown"]
            },
            {
                "before": ["<leader>", "k"],
                "commands": ["workbench.action.navigateUp"]
            },
            {
                "before": ["<leader>", "l"],
                "commands": ["workbench.action.navigateRight"]
            },
            {
                "before": ["<leader>", ","],
                "commands": ["workbench.action.previousEditorInGroup"]
            },
            {
                "before": ["<leader>", "."],
                "commands": ["workbench.action.nextEditorInGroup"]
            },
            {
                "before": ["<leader>", "s"],
                "commands": ["workbench.action.editor.changeLanguageMode"]
            },
            {
                "before": ["<leader>", "<leader>", "h"],
                "commands": ["workbench.action.compareEditor.focusSecondarySide"]
            },
            {
                "before": ["<leader>", "<leader>", "l"],
                "commands": ["workbench.action.compareEditor.focusPrimarySide"]
            }
    ],
    "C_Cpp.default.intelliSenseMode": "clang-x86",
    "clangd.path": "/home/chanjl/.config/Code/User/globalStorage/llvm-vs-code-extensions.vscode-clangd/install/10.0.0/clangd_10.0.0/bin/clangd",
    "editor.renderWhitespace": "all",
    "C_Cpp.updateChannel": "Insiders",
    "window.zoomLevel": 0,
    "ros.distro": "melodic",
    "xml.symbols.maxItemsComputed": 10000,
    "vim.commandLineModeKeyBindings": [
    ]
}
```

## Searching for Unknown Commands

To search for a command, for example, `"workbench.action.toggleEditorWidths"`, you are encouraged to use `Ctrl+Shift+p` and key in the command to search. Then click on the setting icons to review the actual command. You can also use the keyboard shortcut feature to search for the unknown commands. (file -> preference -> keyboard shortcuts).

## Locating Settings.json

settings.json can be found `$HOME/.config/Code/User/settings.json`.
