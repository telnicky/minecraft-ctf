# Minecraft Hunger Games

## Usage
```
docker build -t minecraft .
docker run -it -p 25565:25565 --name minecraft minecraft
```

To edit the world run
```
docker run -it -p 25565:25565 -v $(pwd)/world:/minecraft/world --name minecraft minecraft
```

Monitor server with
```
docker logs -f minecraft
```
