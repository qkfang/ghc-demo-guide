demo1:

Build a website for lego robotics team
the website should use react and only 3 pages: home, about, robotics.
use port 3001, and use current folder as project root

go npm install
set PORT=3001 && npm start


> i dont like the red button, change it to blue


demo1b: instruction
.GitHub\copilot-instructions.md

the background of the website must be light gray (#f5f5f5)
---
applyTo: '*.html'
---

must include a <meta> tag with name="author"
must include a <meta> tag with name="description"



demo2: figma

website
https://www.figma.com/design/eZQZjcT4yMO1UcXbttvNtI/Lego-Website?node-id=1-629&t=eZgnBbB7yoFTBn1o-4


make a html webpage based on this design. must include images, and keep it simple
https://www.figma.com/design/eZQZjcT4yMO1UcXbttvNtI/Lego-Website?node-id=1-629&t=eZgnBbB7yoFTBn1o-4

npx figma-developer-mcp --figma-api-key=figd_85DgxTNr8nKUWdL3AIS6grHZo-xxxxx
figd_117PxOZil83_10kmm_djFY-JSouPdtJHuBtSyM5qTz

.vscode\mcp.json
{
  "servers": {
    "figma": {
      "command": "npx",
      "args": ["-y", "figma-developer-mcp", "--stdio"],
      "env": {
        "FIGMA_API_KEY": "${input:figma_api}"
      }
    }
  },
  "inputs": [
    {
      "id": "figma_api",
      "type": "promptString",
      "description": "Figma API Key",
      "password": true
    }
  ]
}



demo3:
https://github.com/copilot/spaces
what ghc spaces can you see?
use ghc spaces to write python to move lego robot forward 10cm

.vscode\mcp.json
{
  "servers": {
    "github": {
      "type": "http",
      "url": "https://api.githubcopilot.com/mcp/",
      "headers": {
        "X-MCP-Toolsets": "default,copilot_spaces"
      }
    }
  }
}



demo4: GitHub MCP Server
.vscode\mcp.json
{
	"servers": {
		"github": {
			"type": "http",
			"url": "https://api.githubcopilot.com/mcp/"
		},
	}
}

what issue do i have in my GitHub repo
create a new issue title: make the website prettier



demo5: lego robot
move forward 10 cm
move forward 10cm and backword 20cm
open grabber and then close grabber, finally turn around 
do a zig zag move backward 50cm



demo6: spec kit

powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"

cd C:\demo\ghc-demo\demo-project-speckit

specify init legorobot

/speckit.constitution keep it simple and only create html web pages. 
/speckit.specify Build a simple html web for lego robotics team
/speckit.plan the website has a home page
/speckit.tasks
/speckit.implement


