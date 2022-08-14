## Deploy Next.js App to GitHub Pages with new GitHub Actions

Hey there, GitHub just recently posted a tweet about deploying any static site generator to GitHub pages using their new GitHub actions. Let me show you below. 👇

%[https://twitter.com/github/status/1556340744989859840]

For your reference here's the example setup I made with this tutorial. 😁

%[https://github.com/warengonzaga/sample-nextjs-app]

## 🤝 Intro

![Intro GIF](https://media.giphy.com/media/h3u7w8BR07IHDsnzQw/giphy.gif)

Today we are going to deploy a sample next.js app to GitHub pages using new GitHub actions to package your sample next.js app. The old way of doing this is that you need to use something like [gh-pages](https://www.npmjs.com/package/gh-pages) package just to make it work.

Basically, it creates a separate branch just for your exported static site and it works like a magic. Let's learn the new way! Sounds good? Let's go! 💪🔥

## 📃 Requirements

Here are the basic requirements for today's tutorial.

1. GitHub account. (obviously 😅)
2. Code editor. (VS Code 👀)
3. [Sample Next.js app](https://github.com/warengonzaga/sample-nextjs-app).

## 📦 Sample Next.js App

Let's assume that you have the GitHub account and code editor ready. Now let's clone or fork my sample Next.js app to your local machine. I'm gonna use [GitHub CLI](https://cli.github.com) for a quick repo clone. 👀

```bash
gh repo clone warengonzaga/sample-nextjs-app
```

After that, do `yarn install` and `yarn dev` to start a server on `http://localhost:3000`.

Feel free to edit the sample next.js to your liking. This sample next.js app is based on `create-next-app` so nothing special here.

## 🖥️ Set Up Repository

If you fork the sample repo and clone locally, you are good to skip this part. 💪

If you clone the repo without forking it, [follow these instructions](https://docs.github.com/en/get-started/importing-your-projects-to-github/importing-source-code-to-github/adding-locally-hosted-code-to-github) from GitHub! 🏋️

## 🧰 Pages and Actions

Here's the exciting part, now navigate to the **Settings** of your repository and click **Pages**. You'll see it like this. 👇

![GitHub pages settings](https://cdn.hashnode.com/res/hashnode/image/upload/v1660472727090/pJx9bIwkj.png align="left")

Now change it to the new GitHub actions! 😊

![Choose new GitHub actions](https://cdn.hashnode.com/res/hashnode/image/upload/v1660472831537/a0GYT3nLI.png align="left")

You'll see a recommended workflow here, let's configure it! ☕

![Configure the Next.js workflow](https://cdn.hashnode.com/res/hashnode/image/upload/v1660472954841/oizYAqxQW.png align="left")

We don't need to configure this for now as we are deploying a sample next.js app therefore committing this workflow to your repository is a go signal. 🔥

![Commit the Next.js workflow](https://cdn.hashnode.com/res/hashnode/image/upload/v1660473212071/IpBM4Gx69.png align="left")

It is now building something similar to Vercel! 💪😊

![Building](https://cdn.hashnode.com/res/hashnode/image/upload/v1660473323842/YELEX5MtP.png align="left")

Now deploying directly to GitHub pages... 👀

![Deploying to GitHub pages](https://cdn.hashnode.com/res/hashnode/image/upload/v1660473397061/FAYFADYBj.png align="left")

and... it's done with a URL. 😅

![Done building and deployment](https://cdn.hashnode.com/res/hashnode/image/upload/v1660473507754/rPrxuxsDz.png align="left")

Here's what it looks like... `https://opensource.warengonzaga.com/sample-nextjs-app`

![Published and it works](https://cdn.hashnode.com/res/hashnode/image/upload/v1660473872081/kxX56MKHF.png align="left")

Don't forget to [configure your custom domain](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site) via GitHub pages settings. 😊

## 🤔 Conclusion

![Conclusion GIF](https://media.giphy.com/media/26xBI73gWquCBBCDe/giphy.gif)

To end this, unlike the old method this one is much easier now, as you may notice there is no additional branch created from the process, and all the building and deployment process happens on GitHub actions with the help of Next.js workflow. 💪

This update is still in beta at the time of this writing and hopefully, it will improve more in the future. If you have feedback about this fantastic update you can participate by going to GitHub [feedback page](https://github.com/orgs/community/discussions/categories/actions-and-packages). 👍

To learn more about this update, [read this blog](https://github.blog/2022-08-10-github-pages-now-uses-actions-by-default). 📖

---

Like this blog? 🤔 Please consider supporting me on [GitHub Sponsors](https://github.com/sponsors/warengonzaga) or nominate me ([@warengonzaga](https://github.com/warengonzaga)) as a [GitHub Star](https://stars.github.com/nominate). Your support means the world to me. 🥰

See you on my next blog... 👋
