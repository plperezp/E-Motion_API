

# E-motion

This repository is a [json-server](https://github.com/typicode/json-server) created to feed data into the React Application below.

#### [Client Repo here](https://github.com/David-Carballo/e-motion)

# Server Structure

## Collections

### moods

```javascript

  {
      id,
      title,
      color,
      emoji,
      message,
    }

```

### items

```javascript
   {
      id,
      title,
      year,
      genre,
      url,
      length,
      moodId,
      rating,
      isFavorite,
      type,
      youtube,
    }
```

### sentences

```javascript
 {
      mesagge,
      id,
  }
```

## Used API Endpoints in the App

| HTTP Method | URL                         | Request Body                 | Description                                                    |
| ----------- | --------------------------- | ---------------------------- | -------------------------------------------------------------- |
| GET         | `/moods`                    |                              | Returns an array of all moods                                  |
| GET         | `/items`                    |                              | Returns an array of all items                                  |
| GET         | `/items/:itemId`            |                              | Sends all details of a item                                    |
| GET         | `/sentences`                |                              | Returns an array of all sentences                              |
| GET         | `/sentences/:sentenceId`    |                              | Sends all details of a sentence                                |
| POST        | `/items`                    | {title, year, genre , url, length, moodId,rating,isFavorite, type, youtube}  | Create a new item                                            |
| DELETE      | `/games/:gameId`            |                              | Deletes a game object                                          |
| GET         | `/reviews`                  |                              | Sends all reviews                                              |
| POST        | `/reviews`                  | {text, gameId}               | Creates a new review                                           |
| PATCH       | `/reviews`                | {text, gameId}               | Edits a review                                                 |
| PATCH       | `/games/:gameId`            | {isFav}                      | Adds game to favourite                                         |
 
## Links

### Collaborators

[Developer 1 name](www.github-url.com)

[Developer 2 name](www.github-url.com)

### Project

[Repository Link Client](www.your-github-url-here.com)

[Repository Link Server](www.your-github-url-here.com)

[Deploy Link](www.your-deploy-url-here.com)

### Trello

[Link to your trello board](www.your-trello-url-here.com)

### Slides

[Slides Link](www.your-slides-url-here.com)