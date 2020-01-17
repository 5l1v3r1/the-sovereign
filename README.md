<p align="center">
    <a href="https://legacy-roleplay.com" target="blank">
        <img src="https://upload.wikimedia.org/wikipedia/commons/2/25/Simple_gold_crown.svg" height="150px" width="150px" alt="Legacy RP Logo" />
    </a>
</p>

# the-sovereign [![Build Status](https://travis-ci.com/ExpDev07/the-sovereign.svg?branch=master)](https://travis-ci.com/ExpDev07/the-sovereign)


<p>
    <a href='https://ko-fi.com/C1C510DUQ' target='_blank'>
	<img height='36' style='border:0px;height:36px;' src='https://az743702.vo.msecnd.net/cdn/kofi3.png?v=2' border='0' alt='Buy Me a Coffee at ko-fi.com' />
    </a>
</p>

<strong>100% FREE + OPEN SOURCE.</strong>

> A publishing platform for people who have an interest in monarchies around the world and want to learn more about the political ideology. 

See [#contributing](#Contributing) for more details on how you can help shape **the-sovereign**. We're always down to improve and receive feedback.

**Urgent? Write to me on Discord: Marius Big Ounce#2997.**

## Available
The live website can be found at https://thesovereign.org.

## License
Please refer to [LICENSE](https://github.com/ExpDev07/the-sovereign/blob/master/LICENSE) for this project's license.

## Contributors
This list only contains some of the most notable contributors. For the full list, refer to [GitHub's contributors graph](https://github.com/ExpDev07/the-sovereign/graphs/contributors).
* ExpDev07 (Marius) - creator and maintainer of both frontend and backend.

### Prerequisites
* PHP 7+.
* Composer.
* Node (and npm).
* SQL (database).

### Setting up project
Grab yourself a copy of this repository:
```bash
$ git clone https://github.com/ExpDev07/the-sovereign.git
```

Install all the required dependencies (we use both npm and composer):
```bash
$ composer install
$ npm install
```

Create a new file called ``.env`` and copy the contents from ``.env.example`` over to it, then apply your configurations.
```bash
$ cp .env.example .env
```

Create a private and unique application key:
```bash
$ php artisan key:generate
```

Run database migrations so that we can store things:
```bash
$ php artisan migrate
```

Create a symbolic link at **public/storage** so that it points to **storage/app/public**:
```bash
$ php artisan storage:link
```

Compile frontend assets (use "dev" for development and "prod" for production):
```bash
$ npm run dev/prod
```

Finally, boot the server up:
```bash
$ php artisan serve
```
