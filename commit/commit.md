1. Revert the last commit

   git reset HEAD~1
   // If the commit need to be reverted in the remote repo as well
   git push origin +master
   
2. Set author and committer from command line - git commit

   // We can pass author during commit but there is no provision for passing committer as option
   // By default it will get picked up from git config - ~/.gitconfig
   // Need to set two environmnet variables
   
   // In Win
   set GIT_COMMITTER_NAME='P K Tippa'   
   set GIT_COMMITTER_EMAIL='pktippa@gmail.com'
   
   // Run commit command
   git commit -m "Added container" --author "P K Tippa <pktippa@gmail.com>"