## Create a `next.js` app with `bun`

---

### Install `bun`

First run the following command to check `bun` is installed or not

```sh
bun -v
```

If you don't have `bun` installed then run the following command to install `bun`

```sh
curl https://bun.sh/install | bash
```

### Create a next app

Now run the following command to create a next app

```sh
bun create next [your-app-name]
```

It will create a new directory with the name of your app. To start the app run the following command

```sh
cd your-app-name
bun dev
```

### Build production bundle for next app

We have to update `next.js` version before we build our next app

```sh
bun a next@latest
```

Here we update to the latest version of `next` for avoiding any kind of build issue

### Adding `scripts` to your package.json

We can add the following scripts to our package.json file

```json
{
  "scripts": {
    "start": "next start",
    "build": "next build"
  }
}
```

And we can run the following command to build the production bundle

```sh
bun run build
```

To run the production build you can fire following command

```sh
bun start
```
