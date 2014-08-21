## All bbPress localize files and instructions in one place

Since many tutorials about translating bbPress are out of date, people're getting stucked in this simple task -- get the damn forum localized! I hope this project could be a place where there always has the right instructions and all locale files.


## Installation
Put .mo and .po files in /wp-content/languages/plugins. bbPress would automatically pick the right one based on locale setting in wp-config.php.

## Contribute
If you want to improve this project, follow these instructions:

1. Translate strings in .po file. 
2. Rename the .po file to bbpress-{locale}.po, for example bbpress-zh_TW.po for locale "zh_TW".
3. Use gettext tool to compile .po into .mo (machines can only recognize .mo). For Linux User: 

    apt-get install gettext
    msgcat yourFile.po | msgfmt -o generatedFile.mo - 

For OSX: Please go install [poedit](http://poedit.net/).

4. Pull requests to this project. We're looking forward to accept any.
