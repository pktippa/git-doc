1. Disable push for a remote 

    Checking the Initial remote values

   ```sh
   $ git remote -v
   ```

   Returns the reponse like below

   ```sh
   origin	git@pktippa:sample/repo.git (fetch)
   origin	git@pktippa:sample/repo.git (push)
   ```
   
   Now trying to Disabling the push

   ```sh
   $ git remote set-url --push origin no_push
   ```

    Checking the remote response back now.

   ```sh
   $ git remote -v
   ```

    Returns the response like below which shows the push for remote origin is set to no_push

   ```
   origin	git@pktippa:sample/repo.git (fetch)
   origin	no_push (push)
   ```
   
   
2. Avoid prompting for user and pass for remote with http/https

   It's a security risk - User can know the password either by running "git remote -v" or even "git push"
   
   ```sh
   $ git remote set-url <remote_name> http://user:<url_encoded_pass>@host/sample/repo.git
   ```