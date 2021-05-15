# Grass Hoppers
⌒🐸    
 They've come to plant your grass.  🦗━ ╮   
 
 ![image](https://user-images.githubusercontent.com/15683098/118363142-ecc21e80-b5cd-11eb-85f1-05005c4c0e94.png)

## Features



### Automated Daily Commit

Help two "grass hoppers (🐸 - 🦗)" become friends, and enjoy planting the grass on your github profile. 

This project includes a github-actions workflow: `GRASSHOPPERS`, which simply commits a change to the text file: [./grass/grass.txt](./grass/grass.txt).

-at specific times, and everyday.

### Scheduling 

>  You can schedule a workflow to run at specific UTC times using [POSIX cron syntax](https://pubs.opengroup.org/onlinepubs/9699919799/utilities/crontab.html#tag_20_25_07). Scheduled workflows run on the latest commit on the default or base branch. The shortest interval you can run scheduled workflows is once every 5 minutes. [Reference→](https://docs.github.com/en/actions/reference/events-that-trigger-workflows#scheduled-events)

As described above, you can also customize its running interval of `GRASSHOPPERS`. Edit the contents in [grasshoppers.yml](./.github/workflows/grasshoppers.yml).

## Configuration Steps

1. Fork `https://github.com/binchoo/grasshoppers`.

2. Settings> Secrets> New Repository Secret:

   Add a new secret named`PERSONAL_ACCESS_TOKEN`. Its value must be one of [your personal access tokens](https://github.com/settings/tokens).

   ![image](https://user-images.githubusercontent.com/15683098/118364887-4e39bb80-b5d5-11eb-9b41-c64be1b21c6a.png)
   
3. Actions> `GRASSHOPPERS`>  Run workflow> Select branch: `release`> Click button: Run workflow.

   You follow this step to test whether the workflow properly commits a change to your repository.

4. ⌒⌒🐸🦗━ ╮

## LICENSE
[MIT LICENSE](./LICENSE)
