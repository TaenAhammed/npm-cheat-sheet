# Npm-cheat-sheet

An easy npm cheat sheet to makes developer life easier.

**NPM:** Npm is a command line tool for installing third-party node packages as well as the world’s largest software registry. Open-source developers use **npm** to share software.

### Node version:

```bash
> node -v
```

### Npm version:

```bash
> npm -v
```

### Initializing default package.json without answering any question:

**Package.json** file contains meta data about our application. All node applications by standard have at least one package.json file.

```bash
> npm init -y
```

### or with answering questions:

```bash
> npm init
```

### Installing package locally such as underscore:

```bash
> FORMAT: npm i <package-name>
> EX: npm i underscore
```

### Installing specific version of a package:

```bash
> FORMAT: npm i <package-name>@version
> EX: npm i mongoose@4.4.4
```

### Installing packages globally:

```bash
> npm i -g npm-check-updates
```

### List of all the dependencies and the dependencies of dependencies and their exact version:

```bash
> npm list          //for local packages
> npm list -g       //for global packages
```

### Dependencies of only my application (not 3rd party packages):

```bash
> npm list --depth=0        //for local packages
> npm list -g --depth=0     //for global packages
```

### Metadata about a package:

```bash
> FORMAT: npm view <package-name>
> EX: npm view mongoose
```

### Specific metadata about a package:

```bash
> FORMAT: npm view <package-name> <property-name>
> EX: npm view mongoose dependencies
```

```bash
> EX: npm view mongoose devDependencies
```

```bash
> EX: npm view mongoose version
```

```bash
> EX: npm view mongoose versions
```

## Updating local packages:

### Outdated packages:

```bash
> npm outdated
```

### Updating packages:

```bash
> npm update
```
