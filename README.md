# PyGit - Minimal Python Git Implementation

PyGit is a minimal implementation of Git in Python, capable of basic Git operations like committing and pushing to GitHub. This project is inspired by the story shared by Ben Hoyt, which can be read [here](http://benhoyt.com/writings/pygit/).

## Features

- Initialize a new Git repository

- Add files to the index

- Commit changes with author and message

- Push commits to a remote GitHub repository

- Display the status of the working copy

- Show differences between index and working copy

- Other basic Git functionalities

## Installation

No installation is required. Just clone this repository and run the script directly.

## Usage

PyGit is a command-line tool and can be used with various commands similar to Git:

```bash

python pygit.py <command> [options]

```

### Available Commands

- `init <repo>`: Initialize a new repository.

- `add <paths>`: Add file(s) to the index.

- `commit -m <message> [-a <author>]`: Commit the current state of the index to the master branch.

- `push <git_url> [-u <username>] [-p <password>]`: Push the master branch to the given Git server URL.

- `status`: Show the status of the working copy.

- `diff`: Show the diff of files changed between the index and the working copy.

- `cat-file <mode> <hash_prefix>`: Display contents of the object.

- `ls-files [-s]`: List files in the index.

- `hash-object <path> [-t <type>] [-w]`: Hash the contents of the given path.

### Examples

- Initialize a new repository:

  ```bash

  python pygit.py init my_repo

  ```

- Add a file to the index:

  ```bash

  python pygit.py add my_file.txt

  ```

- Commit changes:

  ```bash

  python pygit.py commit -m "Initial commit"

  ```

- Push to remote:

  ```bash

  python pygit.py push https://github.com/username/repo.git

  ```

## Dependencies

PyGit is written in Python and requires no external dependencies. It uses standard libraries available in Python.

## License

PyGit is released under the MIT License. See [LICENSE.txt](LICENSE.txt) for more details.

## Contributing

Contributions to PyGit are welcome! Please read the [contributing guidelines](CONTRIBUTING.md) before submitting pull requests.

## Acknowledgments

Thanks to Ben Hoyt for the inspiration and guidance through his writings on implementing Git in Python.

---

This README is a brief overview of PyGit. For more detailed information, refer to the source code and comments within it.
