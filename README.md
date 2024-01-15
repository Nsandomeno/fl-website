# fl-website

## Docker

### Build in docker container
```
docker build -t website .
```

### Run website locally
```
docker run -it 8080:80 --rm --name website1 website
```

## Development Setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
