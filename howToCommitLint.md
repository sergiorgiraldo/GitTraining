1. 
	npm init
2. 
	npm install --save-dev @commitlint/cli
	npm install --save-dev @commitlint/config-conventional
	npm install --save-dev @commitlint/prompt-cli
3.
	notepad commitlint.config.js
		module.exports = {extends: ['@commitlint/config-conventional']};
4.
	notepad package.json
		{
			"scripts": {
				"commit": "commit"
			}
		}
5.
	notepad.gitignore
		# Logs
		logs

		# Dependency directories
		node_modules/
	
6.
	git add.
	npm run commit
	
