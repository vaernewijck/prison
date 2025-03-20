# Prison API

A simple static JSON API providing information about prison break.

## Available Endpoints

- `/api/simple.json` - Only episode titles
- `/api/advanced.json` - List of movies starring Jason Statham

## How to Use

This is a static JSON API hosted on GitHub Pages. 

Simply access any endpoint directly via URL.

Example:
```
GET https://vaernewijck.github.io/prison/api/simple.json
```

### Sample JavaScript Code

```javascript
const fetchData = async () => {
  try {
    const response = await fetch('https://vaernewijck.github.io/prison/api/simple.json');
    const data = await response.json();
    console.log(data);
  } catch (error) {
    console.error('Error:', error);
  }
};

fetchData();
```
