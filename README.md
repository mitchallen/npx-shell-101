npx-shell-101
==

[![ko-fi](https://img.shields.io/badge/Ko--fi-Donate-blue?logo=ko-fi)](https://ko-fi.com/mitchallen)
[![buymeacoffee](https://img.shields.io/badge/Buy%20Me%20A%20Coffee-Donate-yellow?logo=buy-me-a-coffee)](https://www.buymeacoffee.com/mitchallen)

## Usage

### To run from the repo using npx

To skip the install confirmation prompt, add the `--yes` (or `-y`) flag:

```sh
npx --yes github:mitchallen/npx-shell-101
```
Or, without the flag (will prompt on first run):

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

* * *

## gist example

* See: https://gist.github.com/mitchallen/21b1ec7256fb8dab4e8b05744d280df8 

```sh
curl -fsSL https://gist.githubusercontent.com/mitchallen/21b1ec7256fb8dab4e8b05744d280df8/raw/run.sh | sh
```

## Passing a Name as an Argument

You can pass a name as an argument to greet a specific user. Here are examples for each method:

### Using npx

To skip the install confirmation prompt, add the `--yes` (or `-y`) flag:

```sh
npx --yes github:mitchallen/npx-shell-101 Alice
```
Or, without the flag (will prompt on first run):
```sh
npx github:mitchallen/npx-shell-101 Alice
```
**Output:**
```
Hello, Alice!
```

### Using npm start

```sh
npm start -- Alice
```
**Output:**
```
Hello, Alice!
```

### Running the script directly

```sh
./bin/run.sh Alice
```
**Output:**
```
Hello, Alice!
```

If you do not pass an argument, the script will display:
```
Hello from a shell script!
```
