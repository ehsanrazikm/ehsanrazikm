# Agent Clan HQ

A web page where you can watch your team ("clan") of agents work, and see how well each one is doing.

Right now the agents are **pretend**. They do make-believe jobs so you can see how the page works. Later you can connect real agents.

## What you see on the page

| Thing on the page | What it means |
|---|---|
| Robot face | Each agent. The eyes move when it's working, look sleepy when it's resting, and it shakes when it's stuck. |
| Colored label | What the agent is doing: **Working**, **Thinking**, **Resting**, or **Stuck**. |
| Progress bar | How much of the current job is finished. |
| Tasks done | How many jobs it has finished. |
| Success | Out of all its jobs, how many went right (in percent). |
| Avg time | How many seconds a job takes, on average. |
| Last 10 | Green square = job went well. Red square = job failed. |
| Lv and XP | Agents earn 20 XP for each good job. 100 XP = next level. |
| Leaderboard | Who is doing best. Score = tasks done × success rate. |
| Clan diary | A list of everything that happened, newest at the top. |

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
{ name: "Scout", role: "Researcher", color: "#2E86DE", skill: 0.92 },
```

- `name`: the agent's name
- `role`: its job
- `color`: its color ([pick a color code here](https://htmlcolorcodes.com/))
- `skill`: how good it is, from 0 to 1 (0.9 means it gets 9 out of 10 jobs right)

### Step 3: Give them jobs
Find `STEP 2: THE KINDS OF JOBS`. Each job type has a list of tasks in quote marks. Add your own, separated by commas.

### Step 4: Add agents without editing code
Type a name and a job in the boxes at the top of the page and press **Add agent**. (These go away when you refresh. To keep one forever, add it in Step 2 instead.)

### Step 5 (later): Connect real agents
Right now the `tick()` function makes up the work. To show real agents, a grown-up helper or Claude can change the page so it reads each agent's real status (for example from a file or a small server) instead of making it up. Ask Claude: *"Connect my Agent Clan HQ page to my real agents"* and tell it what your agents are and where they run.

## Tips
- If something breaks, press Ctrl+Z (undo) in your editor, save, and refresh.
- Change one small thing at a time and refresh to see what happened. That's how coders learn!
