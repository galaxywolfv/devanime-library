<p align="center"><img src="https://i.imgur.com/yv74BRj.jpg" width="175"/></p>

<h1 align="center"> DevAnime library </h1>

DevAnime library is a Node library which provides high-level APIs to get information about several entertainment mediums like books, movies, comics, anime, manga, etc.

<h2> Table of Contents </h2>

- [Quick Start](#quick-start)
  - [Installation](#installation)
  - [Usage](#usage)
- [Documentation](#documentation)

## Quick Start

### Installation

To use DevAnime library in your project, run:
```bash
yarn add @devanime/extensions
# or "npm i @devanime/extensions"
```

### Usage

**Example** - searching for a book using the libgen provider.
```ts
import { BOOKS } from "@devanime/extensions"

// Create a new instance of the Libgen provider
const books = new BOOKS.Libgen();
// Search for a book. In this case, "Pride and Prejudice"
const data = books.search('pride and prejudice').then(data => {
  // print results
  console.log(data)
})
```

**Exmaple** - searching for anime using the gogoanime provider.
```ts
import { ANIME } from "@devanime/extensions"

// Create a new instance of the Gogoanime provider
const gogoanime = new ANIME.Gogoanime();
// Search for an anime. In this case, "One Piece"
const results = gogoanime.search("One Piece").then(data => {
  // print results
  console.log(data);
})
```

Do you want to know more? Head to the [`Getting Started`](https://github.com/galaxywolfv/devanime-library/tree/master/docs/guides/getting-started.md).

## Documentation
- [`Getting Started`](./docs/guides/getting-started.md)
- [`Guides`](https://github.com/galaxywolfv/devanime-library/tree/master/docs)
- [`Anime`](./docs/guides/anime.md)
- [`Manga`](./docs/guides/manga.md)
- [`Books`](./docs/guides/books.md)
- [`Movies`](./docs/guides/movies.md)
- [`Light Novels`](./docs/guides/light-novels.md)
- [`Comics`](./docs/guides/comics.md)
- [`Meta`](./docs/guides/meta.md)
- [`News`](./docs/guides/news.md)

## License
Licensed under [MIT](./LICENSE).
