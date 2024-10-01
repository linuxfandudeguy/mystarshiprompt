![Screenshot 2024-10-01 7 28 55 PM](https://github.com/user-attachments/assets/61511b14-4381-45b6-aaa5-019dbcabc940)

```toml
format = """
[](#3B4252)\
$python\
$username\
[](bg:#434C5E fg:#3B4252)\
$directory\
[](fg:#434C5E bg:#4C566A)\
$git_branch\
$git_status\
[](fg:#4C566A bg:#86BBD8)\
$c\
$elixir\
$elm\
$golang\
$haskell\
$java\
$julia\
$nodejs\
$nim\
$rust\
[](fg:#86BBD8 bg:#06969A)\
$docker_context\
[](fg:#06969A bg:#33658A)\
$time\
[ ](fg:#33658A)\
"""
command_timeout = 5000

[username]
show_always = true
style_user = "bg:#3B4252"
style_root = "bg:#3B4252"
format = '[$user ]($style)'

[directory]
style = "bg:#434C5E"
format = "[📁 $path ]($style)"
truncation_length = 3
truncation_symbol = "…/"

[directory.substitutions]
"Documents" = "📄 "
"Downloads" = "📥 "
"Music" = "🎶 "
"Pictures" = "🖼️ "

[c]
symbol = "🎨" # Palette emoji for programming language context
style = "bg:#86BBD8"
format = '[$symbol ($version) ]($style)'

[docker_context]
symbol = "🐳" # Whale emoji for Docker
style = "bg:#06969A"
format = '[$symbol $context ]($style) $path'

[elixir]
symbol = "🦄" # Unicorn emoji for Elixir
style = "bg:#86BBD8"
format = '[$symbol ($version) ]($style)'

[elm]
symbol = "🍂" # Leaf emoji for Elm
style = "bg:#86BBD8"
format = '[$symbol ($version) ]($style)'

[git_branch]
symbol = "🌿" # Herb emoji for Git branch
style = "bg:#4C566A"
format = '[$symbol $branch ]($style)'

[git_status]
style = "bg:#4C566A"
format = '[$all_status$ahead_behind ]($style)'

[golang]
symbol = "🐹" # Hamster emoji for Go
style = "bg:#86BBD8"
format = '[$symbol ($version) ]($style)'

[haskell]
symbol = "🎓" # Graduation cap emoji for Haskell
style = "bg:#86BBD8"
format = '[$symbol ($version) ]($style)'

[java]
symbol = "☕" # Coffee emoji for Java
style = "bg:#86BBD8"
format = '[$symbol ($version) ]($style)'

[julia]
symbol = "🧪" # Test tube emoji for Julia
style = "bg:#86BBD8"
format = '[$symbol ($version) ]($style)'

[nodejs]
symbol = "🟢" # Green circle for Node.js
style = "bg:#86BBD8"
format = '[$symbol ($version) ]($style)'

[nim]
symbol = "🐍" # Snake emoji for Nim
style = "bg:#86BBD8"
format = '[$symbol ($version) ]($style)'

[python]
symbol = "🐍" # Snake emoji for Python
style = "bg:#3B4252"
format = '[($virtualenv)]($style)'

[rust]
symbol = "🦀" # Crab emoji for Rust
style = "bg:#86BBD8"
format = '[$symbol ($version) ]($style)'

[time]
disabled = false
time_format = "%R" # Hour:Minute Format
style = "bg:#33658A"
format = '[$symbol $time ]($style)' # Clock emoji for time
```
