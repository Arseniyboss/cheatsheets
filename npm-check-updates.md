# npm-check-updates cheatsheet

| Command                               | Description                                          |
| ------------------------------------- | ---------------------------------------------------- |
| sudo npm install npm-check-updates -g | installs npm-check-updates package globally          |
| ncu                                   | lists outdated dependencies                          |
| ncu -i                                | allows to select specific packages to update         |
| ncu -i --format group                 | groups packages into patch, minor and major releases |
| ncu -u                                | updates outdated dependencies to latest versions     |
| npm install                           | installs updated dependencies                        |
