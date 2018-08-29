# News App - Vue

Application to view news stories from sources around the world.

Built with [Vue.js](https://vuejs.org/) as frontend JavaScript framework.

## Requirements

- [Vue CLI 3](https://cli.vuejs.org/)
- [Tailwind CSS](https://tailwindcss.com/)
- [Yarn](https://yarnpkg.com/lang/en/)
- [News API](https://newsapi.org/) key

## Installation

### Clone Project

```sh
git clone https://github.com/taiyeoguns/news-app-vue.git news-app-vue
```

### Install dependencies

Install `npm` dependencies with Yarn:

```
yarn
```

### Get API key for News service

Head to [http://newsapi.org](http://newsapi.org), signup or login to and get an API key


### Add details in `.env.local` file

Create `.env.local` file from example `.env` file and maintain necessary details in it e.g. API key etc

```sh
cp .env .env.local
```

### Compile, run server and hot-reload for development
```
yarn serve
```

## Other

### Compile and minify for production
```
yarn build
```

### Lint and fix files
```
yarn lint
```
