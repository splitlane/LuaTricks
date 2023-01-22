_=getmetatable''_.__call=function()return _.__call end


('')''''''''''''




--Explanation

--[[
    tables = dictionary, and the only data structure in lua.
    if you have one string or table argument to a function call, you don't need parenthesis.
        ex: func('hi') -> func'hi'
        ex: func({1, 2, 3}) -> func{1, 2, 3}
]]

--[[
    1. setting the variable _ to the metatable

    you can take the metatable (special table that stores behavior of an object) of a string.
    since tables are objects, we can modify it and it'll be modified everywhere.
    side note: you can't just use setmetatable since error.
]]
_=getmetatable''

--[[
    2. setting the call behavior to

    metatables have different behaviors, and you can modify them.
    you can set the call behavior of a string to make it so that when a string is called, it calls the __call behavior instead of erroring.
]]
_.__call=

--[[
    3. making a self-returning function
    
    we can create an anonymous function (lambda) where it returns itself once called.
    this allows for stringing function calls.
        ex: func(a)(b)(c)
        side note: this is called currying
    all this does is return the string metatable's __call behavior (itself) when called.
]]
function()return _.__call end

--[[
    4. calling strings

    we can finally call strings now!
    however, we need parenthesis for the first string since that'll result in a syntax error without them.
    when the first string is called with another string, it returns the self-returning function.
]]
('')''''''''''''
