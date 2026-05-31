when we push commits, tags won't be pushed, so we have to push them separately, for pushing the tags, we use `git push origin v2.0(tag name)` command and if we want to delete the tag from our remote repository, we use `git push origin --delete v2.0`.

when we delete via command above, the tag still exists in our local repository which for deleteing it we use `git tag -D v2.0(tag name)`