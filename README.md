# mkvenv

> [!IMPORTANT]
> I have stopped using/maintaining this tool and a have been using [uv](https://github.com/astral-sh/uv) for my venv needs instead.

Create and maintain Python venvs.

I keep my venvs in a central location (`~/.local/lib/venv/*`) which makes maintenance much easier.

Check out the [activate script](https://github.com/cn246-dotfiles/zsh/blob/main/.config/zsh/functions/activate) in my zsh dotfiles for easy activation of venvs!


## Installation
I used Python 3 with it's default modules to parse JSON, so there are no external dependencies required.

However, you may need to install any Python packages that your OS requires for creating Python venvs.

----

## Usage
- Clone this repository:

        git clone git@github.com:cn246-admin/mk_venv.git

- Change to the repository directory:

        cd mk_venv

- Copy the included **settings.json.example** to **settings.json**:

        cp settings.json.example settings.json


- Edit **settings.json** with your desired venv configuration:

        $EDITOR settings.json

- Run the script:

        ./mk_venv

Updating the list of modules in **settings.json** and re-running the script will install or uninstall modules for that particular venv.

----

## Links
- https://docs.python.org/3/library/venv.html
