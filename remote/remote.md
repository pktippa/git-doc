1. Disable push for a remote 

   git remote -v
   origin	git@pktippa:sample/repo.git (fetch)
   origin	git@pktippa:sample/repo.git (push)
   
   // Disabling push
   git remote set-url --push origin no_push
   
   git remote -v
   origin	git@pktippa:sample/repo.git (fetch)
   origin	no_push (push)
   
   
2. Avoid prompting for user and pass for remote with http/https

   It's a security risk - User can know the password either by running "git remote -v" or even "git push"
   git remote set-url <remote_name> http://user:<url_encoded_pass>@host/sample/repo.git
   