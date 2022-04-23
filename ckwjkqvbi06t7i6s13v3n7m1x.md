## Create CSS Text Portrait In Less Than 3 Minutes

A CSS text portrait is one of the sweetest gifts for your loved one as a programmer or developer. You can add your personal message to it or just use lyrics from a song to show your love. I made an example below for the context of this tech blog.

![emily css text portrait](https://cdn.hashnode.com/res/hashnode/image/upload/v1638053715581/7qbikfjIV.png)

> This is my girlfriend Emily, and I use lyrics from Beautiful in White by Shane Filan.

It is easy to create your own CSS text portrait from scratch, but how about others willing to create their own but have no knowledge in coding? That's where my builder comes for! 👊

Let's create your own CSS text portrait in less than 3 minutes using my builder!

## 🛠 The Builder

[![banner repo](https://cdn.hashnode.com/res/hashnode/image/upload/v1638054587456/UZ5LPh7Qi.png)](https://github.com/warengonzaga/css-text-portrait-builder)

The CSS text portrait builder is a popular pure CSS text portrait builder for your loved ones. You don't need to waste your time just to create it from scratch and spend time working on its CSS sorcery.

I created this builder for the reason of adding space for freedom. That's why I created a builder instead of a plain web application or a drag and drop generator. I know it is more convenient but it is more fun if you allow yourself to get your hands dirty while building a text portrait specifically for your loved ones.

GitHub: [github.com/warengonzaga/css-text-portrait-builder](https://github.com/warengonzaga/css-text-portrait-builder)

## ⚡ Instant Setup

To get started, all you have to do is to go to the [official GitHub repository](https://github.com/warengonzaga/css-text-portrait-builder).

Make sure you meet the following requirements. 👌

- GitHub Account
- Gitpod Account
- High-resolution image in JPG/JPEG format.

Now, here's the fun part. We are going to use Gitpod as our cloud-based development environment so that it can eliminate inconsistency in our building process due to differences in the operating system we are using. Why not use the same system under Gitpod? 😁

Open the builder using the link below.

[gitpod.io/#github.com/warengonzaga/css-text-portrait-builder](https://gitpod.io/#github.com/warengonzaga/css-text-portrait-builder)

A new Gitpod workspace will be created. Now proceed to the build steps below.

## 📋 Building Steps

1. Rename your image into `bg.jpg` and make sure it is in JPG/JPEG format.
2. Navigate to `src/img` and upload your image, just replace the existing image.
3. Next, open the `config.json` file by just clicking it, an editor will open.
4. Edit the contents of the `config.json` file to match your needs. 
   - For the object `name`, this is the name of your portrait, it can be the name of your subject.
   - For the object `text`, this is the text you want to see in the portrait. It can be lyrics, a passage from a book, or a sweet message to your subject or loved one.
5. Navigate to `src/scss` and open the file `_vars.scss` to edit the settings.
6. Lastly, look in the command-line interface and hover your mouse to the `https://localhost:1234` and press `ctrl` + `left click` to open it to a new tab. You'll see your builds in real-time.

## ✨ Customization

You can customize the output of the build by editing the `src/scss/_vars.scss` file.

This is the default configuration for the colored version.

```scss
$brigthness: 1;
$grayscale: 0;
$invert: 0;
```

If you want to use the classic version of text portrait then use the following configuration.

```scss
$brigthness: 0.8;
$grayscale: 1;
$invert: 0;
```

Then these are the variables inside the `_vars.scss` file.

```scss
/**
 * builder settings
 */
$subject-image: url('../img/bg.jpg'); // image to potrait
$black: #222; // background color
$regular: 12px; // font size

/**
 * image filter settings
 * defaults: brightness = 1, grayscale = 0, invert = 0 (colored result)
 * classic: brightness = 0.8, grayscale = 1, invert = 0 (black and white result)
 */
$brigthness: 1;
$grayscale: 0;
$invert: 0; // it will convert the color of the image
```

It is always up to you what you want with your builds. Every time you made changes to the code it will automatically update and save your changes.

## 💬 Discussions

To learn more about the builder or you just want to showcase your builds then you are welcome to hop in on our [official GitHub discussions](https://github.com/warengonzaga/css-text-portrait-builder/discussions).

I want to share this build with one of the builders in the community! 🥰

![the almighty loaf](https://cdn.hashnode.com/res/hashnode/image/upload/v1638122978738/jhIbAuA1F.png)

> I featured this build since it is very unique, the author of this portrait uses a special character to achieve this meme look.

## 🐱‍👤 Last Words

Alright, looks like that's fast enough to create your own CSS text portrait using my builder. The builder is currently under development and I will add more features sooner! I created this project in just 4 hours including the publishing of the project. I will leave some useful links below for you to take a look at and learn more about the project.

**Official Documentation**: [docs.warengonzaga.com/css-text-portrait-builder](https://docs.warengonzaga.com/css-text-portrait-builder)

**GitHub Repository**: [github.com/warengonzaga/css-text-portrait-builder](https://github.com/warengonzaga/css-text-portrait-builder)

---

📢 Nominate me ([@warengonzaga](https://warengonzaga.com)) as a **[GitHub Star](https://stars.github.com/nominate)**. If you appreciate my hard work, passion, and dedication to open source projects like this.

Cheers! 🚀👌
See you on my next blog...