<img alt="Instahunter" src="https://raw.githubusercontent.com/KSSBro/instahunter/gh-pages/public/images/main_logo_blue.png" height="100">

# Instahunter

Instahunter is a CLI app that can fetch posts and user data from Instagram.

## Getting Started

### Prerequisites

To run the app from source - [Git](https://git-scm.com/) is needed to clone the repository on your machine. [Python](https://www.python.org/) and [Click](https://click.palletsprojects.com/en/7.x/) are required to run the app from the source.

### Installing

After installing **git**, clone the repository on your machine

```
git clone https://github.com/KSSBro/instahunter.git
```

After installing **Python**, install **Click** with **pip**

```
pip install click
```

### Usage

Running from the source:

```
python instahunter.py
```

Running from the executable:

```
instahunter
```

To get help use **--help**:

```
instahunter --help
```

```
instahunter getposts --help
```

#### Getting Posts

Use the command **getposts** and option **-tag** to search for posts.

```
instahuter getposts -tag *the_hashtag_you_want_to_search_posts_for*
```

#### Getting User Data

Use the command **getuser** to get user data.

Options:

- `-via`: username(default) - fetch data with username, id - fetch date with user id
- `--value` : username or id you want to fetch data with, depending upon your choice in **-via**

```
instahunter getuser -via *username or id* --value *value*
```

#### Getting User Posts

Use the command **getuserposts** and option **-username** to get posts.

```
instahunter getuserposts -username *username*
```

#### Searching for Users

Use the command **search** and option **-query** to search for users.

```
instahunter search -query *query*
```

> All the above commands will display data in the terminal itself.

#### Creating a file with the data

To create a file with the data retrieved use **-create-file** and **--file-type** options along with any option.

Options:

- `-create-file`: true - will create a file with the data, false(default) - won't create a file
- `--file-type` : json - will create a json file, text(default) - will create a text file

```
instahunter getposts -tag *hashtag* -create-file *true or false* --file-type *json or text*
```

## Release

v1.5 has been released.<br/>
The executable is available in the release section.

## Built with

- [Python](https://www.python.org/)
- [Click](https://click.palletsprojects.com/en/7.x/)
- [Pyinstaller](https://www.pyinstaller.org/)(Executable)

## Contributing

Fork the repository and open a pull request to contribute.
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## Authors

- **KSSBro** - [Github](https://github.com/KSSBro)

## License

[MIT](https://choosealicense.com/licenses/mit/)