

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
| PATCH       | `/itemS/:itemId`             | {title, year, genre , url, length, moodId,rating,isFavorite, type, youtube}                             | Edits a item                                          |
| DELETE      | `/itemS/:itemId`            |                              | Delete a review                                                |
| GET         | `/moods/:moodId?_embed=items`|             | Return a single mood and all their items                                        |
| GET         | `/items/?isFavorite=true`                |               | Returns an array of favorite items                                                 |

 
## Links

### Collaborators

[Pedro Perez](https://github.com/plperezp)

[David Carballo](https://github.com/David-Carballo)

### Project

[Repository Link Client](https://github.com/David-Carballo/e-motion)

[Repository Link Server](https://github.com/plperezp/E-Motion_API)

[Deploy Link](https://e-motion-app.netlify.app/)



### Slides

[Slides Link](https://docs.google.com/presentation/d/1qQNol8fllfdOT1e0SSSevsHNn8Da3T2BIPFJ6czS1nI/edit?usp=sharing)