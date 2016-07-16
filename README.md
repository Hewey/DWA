1. git checkout master
	1. switches to master branch
2. git pull origin master
	1. resolve any conflicts between dev and master; commit dev
		1. git diff master dev
			1. git add .
			2. git commit -m "Message"
			3. git pull origin master
3. git merge dev
	1. resolve any conflicts
4. git push origin master
5. Tag your release
	1. git tag -a vX.X.X -m "Message"
	2. git push origin --tags
6. inform team
7. test new features on staging server
	1. git push stagingServer master
		1. resolve any conflicts
8. communicate success
9. git push prodServer master
