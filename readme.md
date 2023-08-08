# Alfred

> [Alfred](https://www.alfredapp.com) workflows I use

## Workflows

- [Search websites](search-websites) - Searches on popular websites. I use [Web Searches](https://github.com/nikitavoloboev/alfred-web-searches) and [Searchio](https://github.com/deanishe/alfred-searchio) for all other searches.
- [Search Files](search-files) - A lot of [file filters](https://www.alfredapp.com/help/workflows/inputs/file-filter/) to find files quickly
- [Search Selection](search-selection) - Search selected text on various websites with hotkeys.
- [Search Content](search-content) - Actions to search through the insides of PDF and MindNode documents as well as Contacts.
- [WiFi Tools](wifi-tools) - Check WiFi connection / Restart WiFi / Toggle it on/off.
- [Go play](go-play) - Create [Go Playground](https://play.golang.org) from selected Go code for sharing.
- [Useful utilities](useful-utilities) - Only has one utility, to search selected text in Alfred.
- [Month numbers](month-numbers) - Search for a month and copy the month number to your clipboard.
- [Clean Folders](clean-folders) - Trash items from Desktop and clean certain folders.
- [Folder Search](folder-search) - Search folders from Alfred and open them in Finder/iTerm/Editor.
- [File Actions](file-actions) - Various file actions I made to operate on files and folders.
- [Go to Subreddit](goto-subreddit) - Go to a subreddit that you specify. For searching subreddits, use [this](https://github.com/deanishe/alfred-reddit).
- [Focus](focus) - Start [Focus](https://heyfocus.com) blocking for some time that you specify.
- [Local host](local-host) - Open port that you specify at local host.
- [Objects library](objects-library) - Useful premade objects for workflows.
- [Open with app](open-with-app) - File actions to quickly open file/folder in the application without going to `Open with...` menu.
- [TODO Task](todo-task) - Write a task and display it on TouchBar, in middle of screen or menu bar.
- [Birthday](birthday) - See time passed since your birthday.
- [Dropbox Upload](dropbox-upload) - Upload and share files with Dropbox.

## Workflow Augmentations

Below are workflows that were not made by me, I just augmented them in my own way to make them 'better' (for me).

I often propose these changes to the workflow author so that the change is merged but sometimes the author does not want to accept the change so I am left with my own fork until then. Credit goes to the authors of these awesome workflows

Take a look at the original workflows first, it will most probably work for you well.

- [GitHub Jump](https://github.com/lox/alfred-github-jump) - Quickly jump to GitHub repositories you made/starred. ([My modification](https://github.com/nikitavoloboev/small-workflows/blob/master/augmentations/GitHub%20jump.alfredworkflow?raw=true))
  - I added many modifiers to do different things such as go directly to issues of the workflow, pull requests of it or even clone the repo to a specified directory.
  - I use this workflow many many times a day and it saved me a lot of time. [My modification](https://github.com/nikitavoloboev/small-workflows/blob/master/augmentations/GitHub%20jump.alfredworkflow?raw=true) has over [7,300 repos I starred](https://github.com/nikitavoloboev/github-stars) that are within 1 second access from you.
- [Alfred Workflow Directory](https://github.com/jeeftor/AlfredWorkflowDirectory) - Quickly open any Alfred Workflow directory in your Terminal, Finder. ([My modification](https://github.com/nikitavoloboev/small-workflows/blob/master/augmentations/Workflow%20directory.alfredworkflow?raw=true))
  - I changed it so that by default it will cd to the workflow in my current iTerm tab but also it can export workflow to `~/Desktop` (you can change location) or it will open the workflow with an editor (VS Code or Sublime in my case).
- [Directory watches](https://github.com/vitorgalvao/alfred-workflows/tree/master/RecentDownloads) - Search insides of directories and action on things. ([My modification](https://github.com/nikitavoloboev/small-workflows/blob/master/augmentations/Directory%20watches.alfredworkflow?raw=true))
  - I modified a script he once shared to quickly see insides of various directories and action on items of them to do various things opening the path in iTerm or moving the file somewhere.
- [Recent Downloads](https://github.com/ddjfreedom/recent-downloads-alfred-v2) - View `~/Downloads` folder from Alfred and action on contents of it. ([My modification](https://github.com/nikitavoloboev/small-workflows/blob/master/augmentations/Recent%20Downloads.alfredworkflow?raw=true))
  - I modified it by adding few actions like opening the path in iTerm. Or opening the file/folder in VS Code.

## Personal workflows

Below is a list of workflows that were made for my own personal use and will most certainly not work on your systems unless you change many things in the workflow.

You can take some inspiration or ideas from these workflows if you wish.

- [Manage notes](https://github.com/nikitavoloboev/small-workflows/blob/master/personal/Manage%20notes.alfredworkflow?raw=true) - I use it to manage editing and extending my [wiki](https://github.com/nikitavoloboev/knowledge).

## Fixing permission issues

Some workflows here are written with Go. See [here](https://github.com/deanishe/awgo/wiki/Catalina) for instructions on fixing permissions in macOS refusing to run Go binary.

## Run

Most workflows here are small enough that everything is done with Alfred blocks with minimal code. You can also open the contents of workflow. Like this:

![](https://i.imgur.com/1z1sHEq.png)

Sometimes the workflows are written in [Go](https://golang.org/) and use [AwGo](https://github.com/deanishe/awgo) library for all Alfred related things.

You can run those workflows like so. Assumes you have [Alfred command](https://godoc.org/github.com/jason0x43/go-alfred/alfred) installed.

1. Clone repo
2. cd to folder with workflow you want to edit
3. Run `alfred link` (makes symbolic link of [`workflow`](workflow) directory)
4. Running `alfred build` will build workflow and place binary inside [`workflow`](workflow) directory.
5. Make changes to code or modify Alfred objects to do what you want! Open debugger in Alfred or run the workflow with `workflow:log` passed in as argument to see the logs Alfred produces.

![](https://i.imgur.com/FFYOecx.png)

## Other workflows

See [Alfred Gallery](https://alfred.app/) and [this list](https://github.com/learn-anything/alfred-workflows).

## Contribute

The tasks to do are outlined in [existing issues](../../issues) and in [tasks below](#tasks) (sorted by priority).

If issue/idea you have is not there, [open new issue](../../issues/new/choose) or [start discussion](../../discussions).

Any PR with code/doc improvements is welcome. ✨

Join [Discord](https://discord.com/invite/TVafwaD23d) for more indepth discussions on this repo and [others](https://github.com/nikitavoloboev#src).

## Tasks

- clean up repo, readme
- update workflows docs + rewrite in rust/ts or go (good code)

### ♥️

[Support on GitHub](https://github.com/sponsors/nikitavoloboev) or look into [other projects](https://nikiv.dev/projects).

[![MIT](http://bit.ly/mitbadge)](https://choosealicense.com/licenses/mit/) [![Twitter](http://bit.ly/latwitt)](https://twitter.com/learnanything_)
