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
4. test new features