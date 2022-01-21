# BlazorWasmHotReloadFailure
Changing the Base Href of a default blazor wasm project causes it to not be debuggable.

This repo is the reproduction for: https://github.com/dotnet/aspnetcore/issues/39554

Steps to recreate this repository:
1. Create a new Blazor WASM project in VS 2022
2. Change the Base Href in the Index and the launch props.
3. Try to lauch the project.
4. It will 404 finding the hot reload script and fail to run the project.
