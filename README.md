# STEAM-Labz Codex Terminal - Updated Documentation

## Overview
STEAM-Labz Codex Terminal is a browser-based terminal application that runs Codex with STEAM-Labz branding. It provides a user-friendly interface for interacting with Codex through a terminal-like experience directly in the browser.

## Features
- Interactive terminal interface using standard web components
- STEAM-Labz branded design with official colors (#1a5b8e, #ff6b35, #007d8c)
- File explorer panel for simulated file system navigation
- Security approval system with multiple modes (suggest, auto-edit, full-auto)
- Responsive design for both desktop and mobile devices
- Simulated Codex API integration (ready for real OpenAI API integration)

## Usage
1. Visit the application at: https://pflimypj.manus.space
2. Enter your OpenAI API key in the settings panel (left sidebar)
3. Select your preferred approval mode:
   - Suggest: Requires approval for all Codex operations
   - Auto Edit: Automatically applies edits but requires approval for commands
   - Full Auto: Executes all Codex operations without approval
4. Use the terminal with commands like:
   - `help` - Display available commands
   - `clear` - Clear the terminal
   - `version` - Show Codex version
   - `about` - About STEAM-Labz Codex Terminal
   - `codex <prompt>` - Run a Codex command

## Example Codex Commands
- `codex explain React hooks`
- `codex create a simple todo app`
- `codex fix this code: function getData() { let x; api.fetch().then(res => x = res); return x; }`

## Technical Implementation
The application is built using:
- Next.js 15.1.4 for the framework
- Standard HTML/CSS/JavaScript components for the terminal interface
- Tailwind CSS for styling
- TypeScript for type safety
- React hooks for state management

## Implementation Notes
The application was initially built using xterm.js for terminal emulation, but due to compatibility issues with static site generation, we switched to a custom implementation using standard web components. This approach ensures the application works reliably in all environments without client-side exceptions.

## Deployment
The application is deployed as a static website at:
https://pflimypj.manus.space

## Future Enhancements
- Integration with the actual OpenAI API
- Real file system operations
- User authentication and session persistence
- History of previous Codex interactions
- Code editor integration

## References
- STEAM-Labz website: https://steam-labz.com
- STEAM-Labz codex web terminal: https://steam-labz.com/sl-codex
- Codex documentation: https://steam-labz.com/codex
- GitHub repository: https://github.com/openai/codex

# STEAM-Labz Codex (Astro + Cloudflare Pages)

This site uses Astro to generate static content for the STEAM-Labz Codex with Markdown support and auto-sync potential.

## Features
- Astro-based static site
- Markdown support with default layout
- Cloudflare Pages deployment-ready

## Deployment
1. Push this repo to GitHub.
2. Create a Pages project in Cloudflare.
3. Set:
   - Framework: Astro
   - Build command: `npm run build`
   - Output folder: `dist`

## Development

```bash
npm install
npm run dev
# sl-codex
