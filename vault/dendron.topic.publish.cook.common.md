---
id: 2340KhiZJWUy31Nrn37Fd
title: Common
desc: ''
updated: 1634741547688
created: 1631132278348
---

### Setup Dendron CLI
```
npm init -y 
npm install @dendronhq/dendron-cli
```

### Setup Notes
1. Update `.gitignore`
    ```sh
    echo .next >> .gitignore
    ```
1. Clone the nextjs repository and install dependencies
    ```sh
    npx dendron publish init
    ```

### Build Notes
- NOTE: run this command inside your [[workspace|dendron.topic.workspace]]
```sh
npx dendron publish build
```

### Preview Notes
- NOTE: run this command inside your [[workspace|dendron.topic.workspace]]
- This command launches a development server which previews how your published website will look like.  Visit [http://localhost:3000](http://localhost:3000) to accesss your site. 
- Enter `CTRL-C` on the terminal to exit the preview
```sh
npx dendron publish dev
```

### Export Notes
- NOTE: run this command inside your [[workspace|dendron.topic.workspace]]
- This command builds the static HTML which you'll upload to actually publish your site

```sh
npx dendron publish export
```

### Manual Install

You can see the manual steps for running nextjs [here](https://github.com/dendronhq/dendron/blob/5f6ba8c75b3a2921de70ac784237441b03374dea/packages/dendron-cli/src/commands/publishCLICommand.ts#L287)

### Upgrade Dendron Nextjs Template

```sh
cd .next && git reset --hard && git clean -f && git pull && npm install 
```

### Reinstall Dendron Nextjs Template

```sh
rm -rf .next && npx dendron publish init
```

##
