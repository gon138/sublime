[
  { "keys": ["f12"], "command": "htmlprettify"},
  { "keys": ["f1"], "command": "fold" },
  { "keys": ["f2"], "command": "unfold" },
  { "keys": ["ctrl+l"], "command": "show_overlay", "args": {"overlay": "goto", "text": "@"} },
  
  { "keys": ["ctrl+space"], "command": "auto_complete" },
  { "keys": ["ctrl+space"], "command": "replace_completion_with_auto_complete", "context":
    [
      { "key": "last_command", "operator": "equal", "operand": "insert_best_completion" },
      { "key": "auto_complete_visible", "operator": "equal", "operand": false },
      { "key": "setting.tab_completion", "operator": "equal", "operand": true }
    ]
  },
  { "keys": ["ctrl+d"], "command": "run_macro_file", "args": {"file": "Packages/Default/Delete Line.sublime-macro"} },
  { "keys": ["ctrl+shift+c"], "command": "toggle_comment", "args": { "block": false } },
  { "keys": ["ctrl+shift+c"], "command": "toggle_comment", "args": { "block": true } },
  { "keys": ["ctrl+shift+f"], "command": "reindent" , "args": {"single_line": false}},
  { "keys": ["alt+up"], "command": "swap_line_up" },
  { "keys": ["alt+down"], "command": "swap_line_down" },
  { "keys": ["ctrl+alt+j"], "command": "join_lines" },
  { "keys": ["ctrl+alt+down"], "command": "duplicate_line" },
  { "keys": ["shift+ctrl+r"], "command": "show_overlay", "args": {"overlay": "goto", "show_files": true} },
  { "keys": ["ctrl+shift+s"], "command": "save_all" },
  { "keys": ["ctrl+l"], "command": "show_overlay", "args": {"overlay": "goto", "text": ":"} },
  { "keys": ["shift+ctrl+f4"], "command": "close_all" },
  { "keys": ["shift+ctrl+y"], "command": "lower_case" },
  { "keys": ["shift+ctrl+x"], "command": "upper_case" },
  { "keys": ["ctrl+pagedown"], "command": "next_view" },
  { "keys": ["ctrl+pageup"], "command": "prev_view" },
  {   
    "keys": ["ctrl+r"], "command": "browser_refresh", "args": {  
        "auto_save": true,  
        "delay": 0.0,  
        "activate_browser": false,  
        "browser_name" : "all"  
    }  
  },
  {
    "keys": ["ctrl+k"], "command": "open_file", "args":
                {
                    "file": "${packages}/User/Default ($platform).sublime-keymap"
                }
  },
  { "keys": ["tab"], "command": "move", "args": {"by": "characters", "forward": true}, "context":
    [
        { "key": "following_text", "operator": "regex_contains", "operand": "^[)\"\\]}]", "match_all": true },
        { "key": "auto_complete_visible", "operator": "equal", "operand": false }
    ]   
  }
]
