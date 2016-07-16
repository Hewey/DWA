1. commit changes to dev
	1. git checkout dev
	2. git add .
	3. git commit -m "Dev changes"
2. git checkout master
	1. switches to master branch
3. git pull origin master
	1. resolve any conflicts between dev and master; commit dev
		1. git diff master dev
			1. git add .
			2. git commit -m "Message"
			3. git pull origin master
4. git merge dev
	1. resolve any conflicts
5. git push origin master
6. Tag your release
	1. git tag -a vX.X.X -m "Message"
	2. git push origin --tags
7. inform team
8. test new features on staging server
	1. git push stagingServer master
		1. resolve any conflicts
9. communicate success
10. git push prodServer master
