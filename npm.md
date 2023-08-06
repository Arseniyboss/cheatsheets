# npm cheatsheet

## Installing

| Command                                     | Description                                             |
| ------------------------------------------- | ------------------------------------------------------- |
| npm install                                 | installs dependencies                                   |
| npm install [package-name]                  | installs the specified package locally                  |
| sudo npm install [package-name] -g          | installs the specified package globally                 |
| npm install [package-name]@[version-number] | installs the specified version of the specified package |
| npm install [package-name]@latest           | installs the latest version of the specified package    |
| npm install [package-name] -D               | installs the specified package to the dev dependencies  |

## Uninstalling

| Command                                      | Description                               |
| -------------------------------------------- | ----------------------------------------- |
| npm uninstall [package-name]                 | uninstalls the specified package locally  |
| sudo npm uninstall install [package-name] -g | uninstalls the specified package globally |

## Viewing

| Command                         | Description                                                |
| ------------------------------- | ---------------------------------------------------------- |
| npm list                        | lists installed packages                                   |
| npm list -g                     | lists globally installed packages                          |
| npm list [package-name]         | lists the current version of the specified package package |
| npm view [package-name] version | lists the latest version of the specified package          |
| npm outdated                    | lists outdated dependencies                                |
| npm outdated -g                 | lists outdated global dependencies                         |

## Updating

| Command                           | Description                                                |
| --------------------------------- | ---------------------------------------------------------- |
| npm update --save                 | updates outdated dependencies to wanted versions           |
| sudo npm update -g                | updates global outdated packages to wanted versions        |
| npm update [package-name] --save  | updates the specified package to its wanted version        |
| sudo npm update [package-name] -g | updates the specified global package to its wanted version |

## Fixing

| Command                      | Description                                              |
| ---------------------------- | -------------------------------------------------------- |
| sudo npm cache clean --force | clears npm cache                                         |
| npm audit                    | checks package vulnerabilities                           |
| npm audit fix                | fixes package vulnerabilities                            |
| npm audit fix --force        | fixes package vulnerabilities including breaking changes |
