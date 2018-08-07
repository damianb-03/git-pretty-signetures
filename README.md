# Git pretty signatures

Extension for 'git log' including pretty printing of gpg signatures in commits and tags.

## Example Output

![example_output](/img/example_output.png)

## Usage
```
$ python3 git_pretty_signature.py --help
usage: git_pretty_signature.py [-h] [-c]

Display git log with gpg signatures in pretty colored format

optional arguments:
  -h, --help   show this help message and exit
  -c, --check  running check mode, exit with 1 status if occurs warning or
               error

```

### .bashrc

*Script can be used from the location of any git repository. For convenient use, a script call can be added to the .bashrc file.*
*Example .bashrc code:*

```bash
git() {
	if [ "$1" = log_sig ]; then
		python3 ~/path/to/git_pretty_signature.py
	fi
}
```

