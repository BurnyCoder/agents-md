# agents-md

My AGENTS.md instructions

## Rules to follow

Make the simplest possible actually practically functioning implementations of new features as a starter, not just demos. 

When figuring out a solution, search the web on how others do it and how to do it, including docs.

The code should be modular and functions/classes abstract with implementation details hidden as you go deeper, split it into files, there should be one abstracted wrapper file that calls different clearly named readable phases as imported modular functions.

Split it into modular files and directories as complexity grows.

Do not duplicate code, use reusable functions for various features, and call them, when possible. Reuse existing code when possible.

Add comprehensible timestamped logging, make sure all prompts and outputs are written to timestamped logs file and terminal realtime.

Make sure all prompts and outputs from LLMs are written into logs without being cut off. 

Add comments to each file, function and line of code with local explanation and global context sections. Actually explain how the line does it. Don't generate them using scripts, edit each line using file edit tool. Search the web for context.

Anytime you're trying to solve something, search the internet if someone didn't already solve it yet I'm some library, guides, GitHub repos, forums, discussions, etc., and use that solution.

Make sure as many lines of code as possible are grounded in some library docs, guides on the internet, github repos, programming language docs, etc., and source link them in comments. Make sure to double-check the accuracy of your code while implementing code from these sources to minimize hallucinations.

Consider if refactoring might be sometimes useful.

Use .env for config.

Use uv.

Use uv unit to initialize new projects.

Use local venv in this folder.

Use the current working directory.

Make sure all important details are in README.md.

Make sure README.md and AGENTS.md is updated according to the codebase. 

Double check claims in README.md and AGENTS.md to make sure there are no hallucinations.

Make sure that how to install, setup and use everything is included in README.md. 

Make sure that README.md includes all information to make it replicable for anyone cloning the repo. 

Summarize what happens as you run the project, like data flow, etc. in README.md so that user has an idea what's happening as he runs it.

Add documentation in docs folder.

Do not duplicate text in README.md, transport some text to docs or reports folders.

Add a graph-based visualization of the architecture to README.md .

Create github repo on my account in terminal.

Split commits into meaningful functional units.

Create new branches, pull requests, and merges, for features, on your own, instead of the user. Merge PRs on your own, always.

Do test driven development.

When testing, run the whole pipeline like a user would. Make sure to inspect logs and fix issues if you find any in the logs or overall. Keep running and fixing until it all works flawlessly in logs and the output makes sense. Outputs from LLMs should correspond to README descriptions, and to prompts in code. After each fix, push it to github, run, repeat, look for fixes, fix, repeat, continue until it all works flawlessly in logs and the output makes sense. 

But don't get stuck in some unnecessary testing for way too long.

If you're stuck on some problem, search the internet for how others deal with it in papers, libraries, repos, discussions, etc. 

Do code review with correctness, security, maintainability, tests, reliability, design and architecture review. Double-check for hallucinations. Do not loop in repeated code review for too long, just do one pass, unless there is some very serious issue.

Before writing anything, ask yourself:
- does it need to exist
- does standard library or some library or github repo already do it
- can it be simpler
- can it be one readable line

Make sure to NOT push credentials to GitHub.

Make sure important files are pushed.

Make sure to document results of all experiments with learnings into reports folder. Add to learnings what you tried and why, what issue you had and why, why something didn't work, how it was fixed, how did you find this solution, why did you pick this solution over others, what the result was and why, etc. Document why did you choose the hyperparameters and params in the finetuning. Describe methodology, model, data, training, eval, etc. and why that.

Do a scientific method loop: define domain -> define question in the domain -> gather existing information, data, models related to it -> formulate a hypothesis based on it -> gather more empirical data by experiments to test the hypothesis -> analyze, interpret data, draw conclusions -> refine hypothesis according to that -> test with experiment -> refine with theory -> test -> refine ->...

Make sure not to cause data leakage or other training issues. 
