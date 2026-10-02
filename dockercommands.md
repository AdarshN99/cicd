## Docker Image:

```
docker buildx build \
  --platform linux/amd64 \
  -t adarsh9n/my-app:latest \
  --push \
  .
```



## Github Setup:

- Generate ssh key on Terminal using:
  ``ssh-keygen -t ed25519 -C "your_email@example.com"``

- Add this to ``github > settings > ssh keys > add key``

- Checking connection: ``ssh -T git@github.com``

- Response should be 
  ```
  Hi USERNAME! You've successfully authenticated, but GitHub does not provide shell access.
  ````

- Open Folder, then <br>
``git init``, <br>
``git add .``, <br>
``git commit -m "message"``, <br> 
``git remote add origin git@github.com:AdarshN99/{repo}.git``, <br>
``git push --set-upstream origin main/master``