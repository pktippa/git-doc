1. Disable push for a remote 

   git remote -v
   origin	git@pktippa:sample/repo.git (fetch)
   origin	git@pktippa:sample/repo.git (push)
   
   // Disabling push
   git remote set-url --push origin no_push
   
   git remote -v
   origin	git@pktippa:sample/repo.git (fetch)
   origin	no_push (push)
   