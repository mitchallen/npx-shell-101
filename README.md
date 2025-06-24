npx-shell-101
==

## Usage

### To run from the repo using npx

```sh
npx github:mitchallen/npx-shell-101
```

When you run this for the first time on a machine, it will ask for permission to install:

```sh
npx github:mitchallen/npx-shell-101
Need to install the following packages:
github:mitchallen/npx-shell-101
Ok to proceed? (y) y

Hello from a shell script!
```

After that it will just run, unless there was an update:

```sh
npx github:mitchallen/npx-shell-101
Hello from a shell script!
```

### To run locallly via npm

```sh
npm start
```

### To run the script locally without npm

```sh
 ./bin/run.sh
```

* * *

## How it works

* The shell script is referenced in **package.json** as a **bin**.
* The script was made executable via `chmod +x bin/run.sh`
* Because the package is ***not*** published, it needs to be run using the format: `npx github:username/repo`
