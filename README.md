# mykkrec (マイ健康観察アプリ)

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

A simple, single-page web app for recording daily health observations. It runs entirely in the browser and saves all data to `localStorage`.

## Demo

View the live app: [https://code4fukui.github.io/mykkrec/](https://code4fukui.github.io/mykkrec/)


![Screenshot of the mykkrec development environment, showing the source code alongside a live preview of the app.](mykkrec.png)


## Features

- **Serverless:** Runs entirely in the browser as a single HTML file with no build step.
- **Persistent Storage:** Saves all notes directly to the browser's `localStorage`.
- **Simple Interface:** Enter a note and click a button to save it with the current date.
- **Chronological Log:** New entries are added to the top of the list for easy viewing.
- **Mobile-Friendly:** Includes a responsive design and a custom `apple-touch-icon` (the kanji "健" for health).

## Usage

1.  Open the [demo URL](https://code4fukui.github.io/mykkrec/) in your browser.
2.  Type a health note into the text field.
3.  Click the "memo" button to save the entry.
4.  Your new entry will appear at the top of the list, timestamped with the current date.

## How It Works

- **Data Storage:** All entries are concatenated into a single string and stored in the browser's `localStorage` under the key `kklist`.
- **Date Stamping:** It uses the `Day` class from [DateTime.js](https://js.sabae.cc/DateTime.js) to prepend the current date to each new entry.

## License

This project is available under the MIT License.