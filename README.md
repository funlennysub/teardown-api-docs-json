## Teardown API Docs

Full version can be found [here](https://teardowngame.com/modding/api.html)

#### JSON has info such as:

* Category<br>
  > Body
* Definition<br>
  > `list = GetBodyShapes(handle)`
* Arguments
  > handle (number) – Body handle
* Return value
  > list (table) – Indexed table of shape handles
* Description
  > Return handles to all shapes owned by a body
* Example

```lua
local shapes = GetBodyShapes(body)
for i=1,#shapes do
  local shape = shapes[i]
end
```

* All lists (`il` tags) with each element on a new line

#### JSON doesn't have info such as:

* Tables
* `init`; `tick`; `update`; `draw` functions
