# Laravel Bcrypt Hash Generator

A lightweight, single-file web tool to generate Laravel-compatible (`$2y$`) Bcrypt password hashes directly in your browser using HTML, CSS, and JavaScript.

## Features

- **Laravel-Compatible Output:** Automatically uses Laravel's default **12 salt rounds** and formats hashes with the `$2y$` prefix so they work seamlessly with `Hash::check()` and Laravel's authentication system.
- **Click-to-Copy:** Click anywhere on the generated hash box or the **Copy** button to copy the hash to your clipboard, complete with visual feedback and a toast notification.
- **Clean, Responsive UI:** Minimal Laravel-inspired interface with a password visibility toggle, Enter-key support, and smooth loading states.
- **Zero Setup:** Runs entirely client-side in a single HTML file—no backend, build step, or `npm install` required.

## Usage

1. Download or clone the repository.
2. Open `laravel-bcrypt-tool.html` directly in any modern web browser.
3. Enter any password or number in the input field and click **Generate Hash** (or press `Enter`).
4. Click the generated hash box to copy it to your clipboard and paste it wherever needed (such as database seeders or manual DB updates).

## Tech Stack

- **HTML5 & CSS3**
- **Vanilla JavaScript**
- **[bcryptjs](https://github.com/dcodeIO/bcrypt.js)** (loaded via CDN)

## Security Note

This tool is built for local development, testing, and manually updating database records. In production applications, always hash passwords on the server side using Laravel's built-in `Hash::make()` or `bcrypt()` helpers.

## License

MIT
