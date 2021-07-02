## NOTE FOR DOCKER COMPOSE

1. ELASTISEARCH

   UID = 1000, when using elasticsearch image, run

   ```shell
   sudo chown -R 1000:1000 elastic1_volume
   ```

2. MONGO

   ```shell
   rs.initiate({
      _id: "rs0",
      version: 1,
      members: [{ _id: 0, host: "localhost:27021" }],
   });
   ```
