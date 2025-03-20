![json](assets/json-jason.png)

# JSON Statham API

A simple static JSON API providing information about actor Jason Statham.

## Available Endpoints

- `/api/info.json` - Basic biographical information
- `/api/movies.json` - List of movies starring Jason Statham
- `/api/awards.json` - Awards and nominations

## How to Use

This is a static JSON API hosted on GitHub Pages. 

Simply access any endpoint directly via URL.

Example:
```
GET https://vaernewijck.github.io/json-statham/api/movies.json
```

### Sample JavaScript Code

```javascript
const fetchData = async () => {
  try {
    const response = await fetch('https://vaernewijck.github.io/json-statham/api/movies.json');
    const data = await response.json();
    console.log(data);
  } catch (error) {
    console.error('Error:', error);
  }
};

fetchData();
```
