# MONSTRORVM

This repository is a [json-server](https://github.com/typicode/json-server) created to feed data into the React Application below.

#### [Client Repo here](https://github.com/xMrAvocado/monstrorvm-client)

# Server Structure

## Collections

### categories

```javascript
{
  id,
  title,
  threatLvl,
  description,
}
```

### monsters

```javascript
{
  id,
  name,
  categoryId,
  description,
  image,
}
```

## Used API Endpoints in the App

| HTTP Method | URL                                    | Request Body                           | Description                                                       |
| ----------- | -------------------------------------- | -------------------------------------- | ----------------------------------------------------------------- |
| GET         | `/categories`                          |                                        | Returns an array of all categories                                |
| GET         | `/monsters?categoryId=:categoryId`     |                                        | Returns an array of the monsters of one specific category         |
| GET         | `/monsters/:monsterId?_expand=category`|                                        | Returns an object with the monster details, including his category|
| PUT         | `/monsters/:monsterId`                 | {name, categoryId, description, image} | Edits details of a monster                                        |
| DELETE      | `/monsters/:monsterId`                 |                                        | Deletes a monster                                                 |
| POST        | `/monsters`                            | {name, categoryId, description, image} | Creates a new monster object                                      |

## Links

### Developer

[Samuel Pérez Besada](https://github.com/xMrAvocado)

### Project

[Repository Link Client](https://github.com/xMrAvocado/monstrorvm-client)

[Repository Link Server](https://github.com/xMrAvocado/monstrorvm-server)

[Deploy Link](https://monstrorvm.netlify.app/)

### Planing

[Link to the planing board](https://excalidraw.com/#json=99u4AuvrFBE9i508Flt59,wP893E78xQjT3v4k9dX_hg)

### Slides

[Slides Link](www.your-slides-url-here.com)
