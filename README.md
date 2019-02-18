# github-tools

## clone-repos.py

A simple script to clone a user's or an organization's public and private repositories. Requires a [personal API token](https://github.com/blog/1509-personal-api-tokens).

### Cloning your own repositories

	$> python ./bin/clone-repos.py --token <personal-api-token> --outdir </path/to/github-clone> [ list of repos to skip ]

### Cloning an origanization's repositories

	$> python ./bin/clone-repos.py --token <personal-api-token> --organization <org> --outdir </path/to/github-clone> [ list of repos to skip ]

### Using a config file

You can also use a standard .ini file for specifying your personal API token

	$> python ./bin/clone-repos.py --config </path/to/config> --outdir </path/to/github-clone> [ list of repos to skip ]

The config file should contain a `github.token` entry, for example:

	[github]
	token=s00pers33kret
    
### See also

* https://github.com/blog/1509-personal-api-tokens

### Using Python 3

You can use this with Python 3 and [pipenv](https://pipenv.readthedocs.io/en/latest/). Just type the following:

```
$ brew install pipenv (on a Mac)
$ pipenv install
$ pipenv shell
```

This should install packages and set you up in a shell using Python 3.
