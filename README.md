# nodejs-show-percentage-of-completion.
## CLI.
### Show percentage of completion.
#### The task.
The processing is long and user doesn't understand how long he needs to wait. Add cli-progress package for better user experience. Think how you calculate process.
#### The solution.
To calculate a process I use file size in bytes (fs.statSync(pathToFile).size) and bytesRead (fs.createReadStream(pathToFile).bytesRead) to estimates process performance.
To solve this task, I offered two ways:
1. processFileLineByLineWithProgressBar - with own written progress bar.
2. processFileLineByLineWithCliProgressBar - with cli-progress package.
