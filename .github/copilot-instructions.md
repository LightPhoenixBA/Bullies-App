# Copilot Instructions

## Purpose
Provide concise, repo-specific guidance for AI-assisted code generation usable from desktop or mobile.

## Project summary
- Solution: `Bullies.slnx`
- Stack: Blazor WebAssembly + API (preferred), .NET 10
- Also contains a .NET MAUI project — prefer MAUI equivalents over Xamarin.Forms

## Developer preferences
- Language: C# (default for generated code)
- Follow existing project style and patterns; keep code minimal and idiomatic
- Prefer `async/await` for async work
- Include unit tests for new logic; use existing test projects and patterns

## Access patterns
- Expect some users to access GitHub/Copilot from a web browser on mobile (phone). Keep examples short, avoid long terminal sessions, and favor single-file patches or clear PR instructions.
- Repo is hosted on GitHub: `https://github.com/LightPhoenixBA/Bullies-App`

## Output rules for Copilot
- Target Blazor solutions first (use Blazor components/pages), avoid Razor Pages or MVC unless requested
- When creating or modifying files, produce small, focused diffs and mention manual steps required
- Use `powershell.exe` commands if providing terminal snippets
- Prefer Visual Studio workflows (mention actions like opening solution, running tests via Test Explorer, or using __CommandName__ where relevant)

## Repo specifics
- Active branch: `master`
- Remote origin: `https://github.com/LightPhoenixBA/Bullies-App`

## Commit & PR guidance
- Provide concise commit messages describing intent
- Include test coverage notes and migration impact in PR descriptions

## When unsure
- Ask whether changes should target the Blazor client, API, or MAUI app before making larger changes.