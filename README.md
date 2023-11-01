# BlazorLuaTest
This code is an experiment to see if Lua can be run in Blazor using NeoLua.

## Why did I do this experiment?
This experiment was spurred on by a desire to test the potential for using Lua in a low code data capture application I maintain as a way to enable richer functionality without the requirement to maintain that functionality as part of the main application code.

## Does it work?
Yes.
![Video demo showing a print to the screen and then a loop of prints to the screen](demo.webm)

## Getting this running
You should just be able to clone this and run in Visual Studio 17.7.6 or higher, it should have no dependancies that aren't covered by nuget.

## Where I might experiment further
Due to my potential use case (low code platform), a key requirement is sandboxing while still allowing access to APIs to allow interoperation with the existing functionality in the platform - This is likely where further experiments will go.

## Issues
- Infinite loops lock up the application, although because it's running client side it's the users issue, which might be fine
- Syntax highlighting isn't working in Ace Editor