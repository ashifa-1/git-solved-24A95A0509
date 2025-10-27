# My Git Mastery Challenge Journey

## Student Information
- Name: Mohammed Ahmad Ashifa
- Student ID: 24A95A0509
- Repository: https://github.com/ashifa-1/git-solved-24A95A0509
- Date Started: 27-10-2025
- Date Completed: 28-10-2025

## Task Summary
Cloned my instructor’s Git repository that had several intentional conflicts and resolved each one carefully using proper Git workflows, commands, and merging techniques. This challenge helped me deeply understand how Git handles version control and conflicts.

## Commands Used

| Command | Times Used | Purpose |
|---------|------------|----------|
| git clone | 1 | To copy the instructor’s repository into my local system |
| git checkout | 20+ | To switch between different branches for merging and testing |
| git branch | 10+ | To view and manage all branches |
| git merge | 2 | To combine changes from dev and conflict-simulator into main |
| git add | 30+ | To stage files after fixing conflicts |
| git commit | 15+ | To save resolved changes |
| git push | 10+ | To upload updates to the remote repo |
| git fetch | 2 | To fetch new data from the instructor’s repo |
| git pull | 1 | To sync with the remote repository |
| git stash | 2 | To temporarily store unfinished work |
| git cherry-pick | 1 | To copy specific commits |
| git rebase | 1 | To reapply commits on top of another base |
| git reset | 3 | To undo commits (soft, mixed, hard) |
| git revert | 1 | To safely undo a commit |
| git tag | 2 | To create release checkpoints |
| git status | 50+ | To check repo state regularly |
| git log | 30+ | To view commit history |
| git diff | 20+ | To compare and analyze file changes |

## Conflicts Resolved

### Merge 1: main + dev (6 files)

#### Conflict 1: config/app-config.yaml
- **Issue**: Production used port 8080, while development used 3000  
- **Resolution**: Unified both setups with environment-based configs  
- **Strategy**: Kept production default and added optional dev settings  
- **Difficulty**: Medium  
- **Time**: 15 minutes  

#### Conflict 2: config/database-config.json
- **Issue**: Different database hosts and SSL options  
- **Resolution**: Structured separate dev and prod profiles  
- **Strategy**: Allowed switching via environment variables  
- **Difficulty**: Medium  
- **Time**: 10 minutes  

#### Conflict 3: scripts/deploy.sh
- **Issue**: Conflicting deploy logic for production and Docker  
- **Resolution**: Combined both using DEPLOY_ENV checks  
- **Strategy**: Automated behavior for each environment  
- **Difficulty**: Hard  
- **Time**: 20 minutes  

#### Conflict 4: scripts/monitor.js
- **Issue**: Different intervals and log styles  
- **Resolution**: Used environment-based configuration object  
- **Strategy**: Adjusted behavior dynamically via NODE_ENV  
- **Difficulty**: Medium  
- **Time**: 15 minutes  

#### Conflict 5: docs/architecture.md
- **Issue**: Two different architecture explanations  
- **Resolution**: Merged both into a single, clear document  
- **Strategy**: Created sections for each environment  
- **Difficulty**: Easy  
- **Time**: 10 minutes  

#### Conflict 6: README.md
- **Issue**: Different feature sets and versions  
- **Resolution**: Combined all with clear structure  
- **Strategy**: Organized content with labeled sections  
- **Difficulty**: Easy  
- **Time**: 10 minutes  

### Merge 2: main + conflict-simulator (6 files)

#### Conflict 1: src/logger.js  
- **Issue**: One branch used console logs, another used a logger module  
- **Resolution**: Kept the logger module with console fallback  
- **Strategy**: Ensured consistent logging format  
- **Difficulty**: Medium  
- **Time**: 15 minutes  

#### Conflict 2: config/env-settings.json  
- **Issue**: Different variable naming conventions  
- **Resolution**: Standardized naming and grouping  
- **Strategy**: Used common prefixes and consistent casing  
- **Difficulty**: Medium  
- **Time**: 10 minutes  

#### Conflict 3: scripts/setup.sh  
- **Issue**: Manual install vs npm ci approach  
- **Resolution**: Merged both for flexible use cases  
- **Strategy**: Added conditional checks for CI/CD pipelines  
- **Difficulty**: Hard  
- **Time**: 20 minutes  

#### Conflict 4: docs/README.md  
- **Issue**: Different guides and formats  
- **Resolution**: Combined and restructured with clear subheadings  
- **Strategy**: Merged both writing styles while keeping it simple  
- **Difficulty**: Easy  
- **Time**: 10 minutes  

#### Conflict 5: test/test-runner.js  
- **Issue**: Different testing frameworks  
- **Resolution**: Chose Jest and updated configs accordingly  
- **Strategy**: Unified all test commands  
- **Difficulty**: Medium  
- **Time**: 15 minutes  

#### Conflict 6: .gitignore  
- **Issue**: Missing ignored files  
- **Resolution**: Merged both lists to cover everything  
- **Strategy**: Included logs, node_modules, env files  
- **Difficulty**: Easy  
- **Time**: 5 minutes  

## Most Challenging Parts

1. **Understanding Conflict Markers**: At first, the conflict markers (`<<<<<<<`, `=======`, `>>>>>>>`) were confusing, but I learned to read them properly.  
2. **Deciding What to Keep**: Choosing between versions wasn’t always easy — reading both carefully helped a lot.  
3. **Complex Script Conflicts**: Merging scripts like deploy.sh took time to fully understand.  
4. **Testing After Fixes**: I made sure to test after every resolution to avoid breaking the build.  

## Key Learnings

### Technical Skills
- Got real experience resolving merge conflicts  
- Understood conflict markers clearly  
- Learned to use `git diff` and `git log` effectively  
- Used almost every major Git command during the challenge  

### Best Practices
- Read both sides of a conflict before choosing  
- Always test before committing  
- Write clear and meaningful commit messages  
- Use `git status` frequently  
- Keep commits small and focused  

### Git Workflow Insights
- Conflicts are normal and part of teamwork  
- Understanding both versions helps avoid mistakes  
- Always document how you solved a conflict  
- Keep your workflow organized and clean  

## Reflection
This Git Mastery Challenge taught me patience and clarity in version control.  
At first, merge conflicts looked frustrating, but after resolving many, I started enjoying the process. Every file I fixed helped me understand how Git manages parallel work.  

Now I feel confident handling real-world collaboration issues. I clearly understand when to use merge, rebase, and revert — and I’ve realized `git reflog` can truly save a project when things go wrong!  

---
