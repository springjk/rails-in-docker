# Docker: Rails and Mysql Stack

## Installation

Clone the `rails-in-docker` repository:

If you already have a `Rails` project, clone this repository on your `Rails` root directory:

```bash
git submodule add https://github.com/springjk/rails-in-docker.git
```
>If you are not already using Git for your rails project, you can use `git clone` instead of `git submodule`.


## Usage

**Note**: this command run in your-rails-project/rails-in-docker path.


### Start:

```bash
cd {rails-in-docker path}
docker-compose up
```

### Enter the Rails container:

```bash
docker-compose exec rails bash
```


## License

MIT