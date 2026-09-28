# Agent Clan HQ

A game-style village where you can watch your team ("clan") of agents work. Each agent is a building, like in Clash of Clans. The Town Hall in the middle is the whole clan.

Right now the agents are **pretend**. They do make-believe jobs so you can see how the page works. Later you can connect real agents.

## What you see on the page

| Thing on the page | What it means |
|---|---|
| Building | One agent. Tap it to open its info window. |
| Smoke and yellow windows | The agent is working. |
| Bubble over a building | **Zzz** = resting, **?** = thinking, **!** = stuck, **+20** = just finished a job. |
| Green bar over a building | How much of the current job is finished. |
| Gold stars | The building's level. Agents earn 20 XP per good job; 100 XP = next level. |
| Gold / Elixir / Gem at the top | Tasks done, total XP, and success rate for the whole clan. |
| Town Hall | Tap it to see the leaderboard (score = tasks done × success rate). |
| Clan chat | Everything that happened, newest at the top. |
| Red post office | The Mail Scout. Its bubble shows how many emails need you. |

## Step by step

### Step 1: Open the page
1. Download `index.html` from this repository to your computer.
2. Double-click it. It opens in your web browser (Chrome, Edge, Safari...).
3. Watch the robots work!

### Step 2: Name your own clan members
1. Open `index.html` in a text editor (Notepad on Windows, TextEdit on Mac, or [VS Code](https://code.visualstudio.com/), which is free and nicer).
2. Find the part that says `STEP 1: YOUR CLAN MEMBERS`.
3. Change a name, like `"Scout"` to `"Max"`. Keep the quote marks.
4. Save the file and refresh the browser (press F5). Your change shows up.

Each line looks like this:

```js
{ name: "Scout", role: "Researcher", shape: "tower", color: "#2E86DE", skill: 0.92 },
```

- `name`: the agent's name
- `role`: its job
- `shape`: the kind of building: `"house"`, `"tower"` or `"hut"`
- `color`: its roof color ([pick a color code here](https://htmlcolorcodes.com/))
- `skill`: how good it is, from 0 to 1 (0.9 means it gets 9 out of 10 jobs right)

### Step 3: Give them jobs
Find `STEP 2: THE KINDS OF JOBS`. Each job type has a list of tasks in quote marks. Add your own, separated by commas.

### Step 4: Add agents without editing code
Type a name and a job in the boxes under the map, pick a building type, and press **Build**. (These go away when you refresh. To keep one forever, add it in Step 2 instead.)

### The Mail Scout (a real agent)
The red post office is the **Mail Scout**. It isn't pretend. Claude reads your email and writes a report: what to do today, what's waiting for your reply, and emails that mention your name. Tap the post office to read it. The red bubble shows how many things need you.

To update it, ask Claude: *"Mail Scout, check my mail."* Your real report goes only to your private page on claude.ai. This file on GitHub keeps an example report, so your work emails never go into the repository.

### Step 5 (later): Connect more real agents
Right now the `tick()` function makes up the work. To show real agents, a grown-up helper or Claude can change the page so it reads each agent's real status (for example from a file or a small server) instead of making it up. Ask Claude: *"Connect my Agent Clan HQ page to my real agents"* and tell it what your agents are and where they run.

## Tips
- If something breaks, press Ctrl+Z (undo) in your editor, save, and refresh.
- Change one small thing at a time and refresh to see what happened. That's how coders learn!
