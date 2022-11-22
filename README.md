# Naming Conventions
- Variables in the main scope (that have not been indented) should be written as **PascalCase**
- Variables in another scope (that have been indented) should be written as **camelCase**
- Paramter variables are also considered to be in another scope so they should be written as **camelCase**
- Avoid single character names. Always have a descriptive name so the reader knows what this varibale contains/is about.
	- An exception can be made in loops where the ``i``teration and ``v``alue names can be used.
	- Another exception is when you don't need a certain variable in loops: then this variable should be named ``_``

# Functions
- Functions should always be written as **PascalCase**
- Functions should always be written in the following style:
```lua
-- Good Example:
function MyFunction()

end

-- Bad Example
function myFunction()

end

myFunction = function()

end
```

# Blocks
- Single line blocks are okay for **small** statements. (< 80 characters)
```lua
-- Good Example:
local result = if (lang == "es") then "Hola, Mundo!" else "Hello, World" end

-- Bad Example:
local result = if (lang == "es" and shouldUseFormatting) then string.format("%s, %s", "Hola", "Mundo") else string.format("%s, %s", "Hello", "World") end
```
- Control Structures (if, then, while, do, repeat, ...) are supposed to be multi-line:
- Control Structures should also be written with curly braces ``()`` when possible:
```lua
-- Good Example:
if (condition) then
	-- Block content here
end

while (condition) then
	-- Block content here
end

-- Bad Example:
if (condition)
then
	-- Block content here
end

while (condition)
do
	-- Block content here
end
```
