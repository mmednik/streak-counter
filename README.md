# `@mmednik/streak-counter` - a basic streak counter

This is a basic streak counter - inspired by Duolingo - writter in TypeScript and meant for the browser (uses `localStorage`).

## Install

```shell
yarn add @mmednik/streak-counter
```

or

```shell
npm install @mmednik/streak-counter
```

## Usage

[![Edit streak-counter (ts-course) (forked)](https://codesandbox.io/static/img/play-codesandbox.svg)](https://codesandbox.io/s/streak-counter-ts-course-forked-q12sf5?fontsize=14&hidenavigation=1&theme=dark)

```js
import { streakCounter } from '@mmednik/streak-counter'

const today = new Date()
const streak = streakCounter(localStorage, today)
```

`streak` returns an object:

```js
{
  currentCount: 1,
  lastLoginDate: "02/06/2023",
  startDate: "02/06/2023",
}
```