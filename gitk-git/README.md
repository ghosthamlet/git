
# gitk with simple file based code review comment

if you are on windows:
just override Git\mingw32\bin\gitk (or old version: Git\bin\gitk) with this gitk: https://github.com/ghosthamlet/git/blob/master/gitk-git/gitk

linux not tested, gitk dir is different, but should mostly work

# useage

show comment:

select commit and file with @ sign


add comment:

select file on cflist first (cflist is right bottom window list of changed files in commits)
then press Alt-c


reload comment:

press Alt-l


# concept

gitk will auto create dir 'gitk/review' and 'gitk/stats' under current repo,

if current user email is gvvvv@163.com, all reviews by him will saved in gitk/review/gvvvv@163.com,

after git commit, git push, git pull, dir gitk/ should be pushed or pulled , then others can see it,

gitk/stats is for future use.

