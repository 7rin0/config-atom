# Atom config

### Export
apm list --installed --bare > packages.list

### Import
apm install --packages-file packages.list

### Remove ALL packages
apm remove $(apm list --installed --bare | cut -d'@' -f1)

### Special snowflakes
_Consider run the following commands as ``` sudo ``` if you get permissions issues_

**linter-rubocop** requires rubocop. Run ``` gem install rubocop ``` command to install.

**rubocop** requires ruby-dev. Run, on distros Debian, ``` sudo apt-get install ruby ruby-dev ``` command to install.

**linter-pylint** requires pylint. Run ``` pip install pylint ``` command to install.

**linter-pep8** requires pep8. Run ``` pip install pep8 ``` command to install.

**import/export instructions** from _https://discuss.atom.io/t/how-to-backup-all-your-settings/15674_

**php-integrator** requires php module sqlite and writing permission to sudo chmod -R 775 ~/.atom/packages/php-integrator-base
