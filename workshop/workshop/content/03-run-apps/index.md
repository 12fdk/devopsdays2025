---
title: Run Apps
---

An important task in any lab, is to be able to create, build and expose an app.

This is already thought of here.

We have a Dockerfile in out excersises

```execute-1
clear
cat Dockerfile
```

And a compose file to build and run it.

```execute-1
clear
cat docker-compose.yml
```

Let's build and run it.

```execute-2
clear
docker compose up
```

Let's see the app live.

```dashboard:reload-dashboard
name: App
title: Open App
```