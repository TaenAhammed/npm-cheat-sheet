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

### Installing packages locally:

```bash
> FORMAT: npm i <package-name>
> EX: npm i underscore
```

### Installing packages globally:

```bash
> FORMAT: npm i -g <package-name>
> EX: npm i -g npm-check-updates
```

### Installing specific version of a package:

```bash
> FORMAT: npm i <package-name>@version          # for local packages
> EX: npm i mongoose@4.4.4

> FORMAT: npm i -g <package-name>@version       # for global packages
> EX: npm i -g npm-check-updates@3.1.1
```

### Installing packages as dev dependency:

```bash
> FORMAT: npm i -D <package-name>
> EX: npm i -D jshint
```

### List of all the dependencies, devDependencies and the dependencies of dependencies, dependencies of devDependencies and their exact version:

```bash
> npm list          # for my application
> npm list -g       # for global packages
```

### List of Dependencies and DevDependencies of only my application and their version:

```bash
> npm list --depth=0
```

### List of globally installed packages and their version:

```bash
> npm list -g --depth=0
```

### Metadata about a package:

```bash
> FORMAT: npm view <package-name>       # for local package
> EX: npm view mongoose
> FORMAT: npm view -g <package-name>    # for global package
> EX: npm view -g npm-check-updates
```

### Specific metadata about a package:

```bash
> FORMAT: npm view <package-name> <property-name>   # for local package
> EX: npm view mongoose dependencies

> FORMAT: npm view -g <package-name> <property-name>   # for global package
> EX: npm view -g npm-check-updates dependencies
```

```bash
> EX: npm view mongoose devDependencies
> EX: npm view -g npm-check-updates devDependencies
```

```bash
> EX: npm view mongoose version
> EX: npm view -g npm-check-updates version
```

```bash
> EX: npm view mongoose versions
> EX: npm view -g npm-check-updates versions
```

## Updating packages:

### Outdated packages:

```bash
> npm outdated      # locally outdated packages
> npm outdated -g   # globally outdated packages
```

```bash
> ncu       # you have to install npm-check-updates cli
```

### Updating packages:

```bash
> npm update        # for my application
> npm update -g     # for global packages
> npm i             # to install updated packages
```

```bash
> ncu -u    # you have to install npm-check-updates
```

### Uninstalling packages:

```bash
> FORMAT: npm un <package-name>     # for local package
> EX: npm i mongoose

> FORMAT: npm un -g <package-name> # for global package
> EX: npm un -g npm-check-updates
```

## Publishing packages on npm registry:

To publishing any package on npm registry you should create an account or login into your existing account on npmjs.com. To do this ->

### Creating account:

```bash
> npm adduser
```

### Login:

```bash
> npm login
```

### Publishing package:

```bash
> npm publish
```

### Updating published package:

```bash
> FORMAT: npm version <major/minor/patch>
> EX: npm version minor
> npm publish
```
