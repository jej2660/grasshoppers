# Grass Hoppers
**⌒🐸**    
 They've come to plant your grass.  **🦗━ ╮**   
 
 ![image](https://user-images.githubusercontent.com/15683098/118367340-f94d7380-b5db-11eb-94a5-202c82ae64c9.png)

## Features

### Automated Daily Commit

Help two "grass hoppers (🐸 - 🦗)" become friends, and enjoy planting the grass on your github profile. 

This project includes a github-actions workflow: `GRASSHOPPERS`, which simply commits a change to the text file: [./grass/grass.txt](./grass/grass.txt).

-at specific times, and everyday.

![image](https://user-images.githubusercontent.com/15683098/118365941-a8d51680-b5d9-11eb-923c-7a2cec58632d.png)

### Scheduling 

>  You can schedule a workflow to run at specific UTC times using [POSIX cron syntax](https://pubs.opengroup.org/onlinepubs/9699919799/utilities/crontab.html#tag_20_25_07). Scheduled workflows run on the latest commit on the default or base branch. The shortest interval you can run scheduled workflows is once every 5 minutes. [Reference→](https://docs.github.com/en/actions/reference/events-that-trigger-workflows#scheduled-events)

As described above, you can also customize its running interval of `GRASSHOPPERS`. Edit the contents in [grasshoppers.yml](./.github/workflows/grasshoppers.yml).

![image](https://user-images.githubusercontent.com/15683098/118365986-d6ba5b00-b5d9-11eb-852a-027fa6ca4726.png)

## Configuration Steps

1. **Fork** https://github.com/binchoo/grasshoppers.

2. **Settings> Secrets> New Repository Secret**

   Add a new secret named`PERSONAL_ACCESS_TOKEN`. Its value must be one of [your personal access tokens](https://github.com/settings/tokens).

   ![image](https://user-images.githubusercontent.com/15683098/118364887-4e39bb80-b5d5-11eb-9b41-c64be1b21c6a.png)
   
3. Lines31-32@[grasshoppers.yml](./.github/workflows/grasshoppers.yml), **set your github id and e-mail.**
  
  ![image](https://user-images.githubusercontent.com/15683098/118369837-f3f22800-b5df-11eb-8ed1-a33665f4a533.png)
   
4. **Actions> GRASSHOPPER>  Run workflow> Select branch: `release`> Click button: Run workflow.**

   You follow this step to test whether the workflow properly commits a change to your repository.
  
5. **⌒⌒🐸🦗━ ╮**

## Rules
- Do not manually modify [./grass/grass.txt](./grass/grass.txt). This may interrupt the push to the remote repository.
- You may add `git pull` before `git push` to resolve the issue.
- Or you may recreate a github action.

## LICENSE
[MIT LICENSE](./LICENSE)
