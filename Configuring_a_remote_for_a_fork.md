#Configuring a remote for a fork

1. Open Terminal.

2. List the current configured remote repository for your fork.

	git remote -v
	origin  https://github.com/YOUR_USERNAME/YOUR_FORK.git (fetch)
	origin  https://github.com/YOUR_USERNAME/YOUR_FORK.git (push)

3. Specify a new remote upstream repository that will be synced with the fork.

	git remote add upstream https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git

4. Verify the new upstream repository you've specified for your fork.

	git remote -v
	origin    https://github.com/YOUR_USERNAME/YOUR_FORK.git (fetch)
	origin    https://github.com/YOUR_USERNAME/YOUR_FORK.git (push)
	upstream  https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git (fetch)
	upstream  https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git (push)


