# Most Popular Files In Git

A Git command that shows a simple leaderboard of files that have seen the most commits over a period of time.

## Use It Like This

The following command would inspect the git repo at `~/my_git_repo` over the past 1000 days.

```
git_most_popular_files "~/my_git_repo" 1000 | head
```

Then the output should look something like this, 
where the number represents the number of commits 
a file had within the specified time period.

```
16  config/bash/arithromancy.profile
14  bin/jsforce_shell
13  lib/white_papers/suboptimization/main.tex
12  version_timestamp.tex
12  lib/node_etl/node-cron/get-public-apis.js
12  bin/rescuetime_time_today
11  lib/project_euler/0003.jq
9   lib/project_euler/0002.jq
9   lib/jupyter/levels-of-testing.ipynb
9   .gitignore

```

Note that the output is TSV and thus can be imported directly into Excel or Google Sheets for further exploration and visualiztion.
