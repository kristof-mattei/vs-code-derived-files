# vs-code-derived-files

Considering the following settings in `tsconfig.json`:

```json
{
    "editor.insertSpaces": true,
    "editor.tabSize": 4,
    "files.exclude": {
        "**/.git": true,
        "**/.DS_Store": true,
        "**/*.js": {
            "when": "$(basename).ts"
        },
        "**/*.js.map": {
            "when": "$(basename).ts"
        }
    }
}
```

I'm expecting the `*.js` and `*.js.map` files to be hidden. However the the `*.js.map` is still there. 
