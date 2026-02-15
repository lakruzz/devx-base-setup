
## Install

### VS Code install

Add the following extensions to the `devcontainer.json`

- Prettier - Code formatter (Prettier)
- Markdownlint (David Anson)
- Code Cspell Checker (Street Side Software)
- Danish - Code Spell Checker (Street Side Software)

```json
	"customizations": {
		"vscode": {
			"extensions": [
				...
				"esbenp.prettier-vscode",
				"DavidAnson.vscode-markdownlint",
				"streetsidesoftware.code-spell-checker",
				"streetsidesoftware.code-spell-checker-danish"
			]
		}
	}
```

## Install the same tools as features, directly in  the devcontainer

```json
		"ghcr.io/devcontainers-extra/features/npm-packages:1": {
			"packages": ["prettier", "markdownlint-cli2", "cspell", "@cspell/dict-da-dk"] 
		}
```	