## Introducing DevSpaces: A Twitter Space Finder for Programmers

Hello everyone, welcome to the introduction post of DevSpaces. DevSpaces is my submission project for **Hashnode x Netlify hackathon**.

**Link**: https://getdevspaces.netlify.app/
**GitHub**: https://github.com/ashutosh-mishra4/devspace

# Introduction to DevSpaces


![hero.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1646116243468/tZlDnRUK3.png)

*[DevSpaces](https://getdevspaces.netlify.app/) is an open-source twitter spaces finder app for programmers. It uses keywords like 'tech', 'programming', 'web' etc. to fetch spaces related to those keywords from Twitter API and display them on the UI.*

## Tech Stack

* [NextJS](https://nextjs.org/) - for building the app
* [TailwindCSS](https://tailwindcss.com/) - for styling
* [Google Fonts](https://fonts.google.com/) - for fonts
* [React Icons](https://react-icons.github.io/react-icons/) - for icons
* [SuperTokens](https://supertokens.com/) - for user auth
* [Netlify](https://www.netlify.com/) - for deployment

## How it works

![how it works.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1646116308151/PZnZ0KxmU.png)

1. **DevSpaces** ask you to select one of the existing keyword cards. Currently, there are 5 keyword cards - *Tech*, *Web*, *Dev*, *Developer*, and *Programming*.

2. Once you select the keyword, the *sign-in* page will be open. Enter your login credentials or else *sign up* if are visiting for the first time.

3. Once signed in, you can see all the **current live and scheduled spaces** related to that keyword and enjoy your favorite ones.

### Current Keywords

![keyword card.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1646116475655/nDABCQur3.png)

For the first version, there are 5 keyword cards-

1. **Tech**
2. **Web**
3. **Dev**
4. **Developer**
5. **Programming**

Once you select any one of those, you will be prompted to the sign-in page just like the image below.  

![Screenshot 2022-03-01 120942.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1646116817741/Q_qULVSiU.png)

Click on the **Sign Up** button located at the side of *Not registered yet?* Enter your email ID and create a password. Once signed up, you will see all the **current live and scheduled spaces** of the keyword which you selected before.

![collective cards.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1646117106926/YryZuyTh2.png)

If the space is live you will be shown the **Start Listening** button in the Space card along with the number of current listeners.

![live space.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1646117173249/h85xf8pUe.png)

If the space is scheduled, you will be shown the **Set Reminder** button in the Space card along with the *scheduled time in ISO 8601 format*.

![scheduled space.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1646117202195/UUQRkeWGC.png)

Both **Start Listening** and **Set Reminder** buttons will lead you to the Twitter link of that particular space.

## Inspiration

I will thank [Dinesh](https://twitter.com/SDinesh91) for inspiring me to build this project. I was working on another project in January and he told me to work more on projects that ***help you stand out*** and try out something with Twitter API. 

That's how this idea came to my mind. Initially, I was thinking to build a spaces finder for everyone but he helped me niche down to build only for programmers(which was a better decision.)

## Building Process

When I started the project, I didn't have any clear idea of what the finished app will look like. So I experimented a lot with various fonts, color palettes, and layouts and came to the current design of the project.

Now let's start the building process - 

I started the project by cloning [NextJS Twitter Starter](https://github.com/Dineshs91/nextjs-twitter-starter) kit. It's a great starter kit for building NextJS, Tailwind, and Twitter API projects.

### Landing Page

![screencapture-localhost-3000-2022-03-01-10_58_14.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1646119251450/Yp03qSICH.png)

I created a folder called component at the root of the directory and separated the entire landing page into 5 components - 

1. Header
2. Hero
3. Howitworks
4. Topics
5. Footer

If you want to dive deep into the codebase - you can look up at the [GitHub repo](https://github.com/ashutosh-mishra4/devspace/) to learn how exactly are they built. For this article, I will give you only a brief overview of how I built the project.

### Keyword Pages

There are total of 5 pages for 5 keywords in the first version - tech.js, web.js, programming.js, dev.js, and developer.js. These 5 files are created inside the pages directory so that they have their independent page(NextJS rocks).

Inside each file, the Twitter API is fetched with the query of the page keyword.

```
endpoint='https://api.twitter.com/2/spaces/search?query=tech'
```
You can see the `query=tech` part in the endpoint variable. We have to replace tech with web, dev, developer, etc depending on the page.

The data is fetched inside the `getServerSideProps` function of the NextJS and they are then mapped with the `.map` array method to display that information on the UI.

### Error 500 page

While building the app I noticed that most of the tech spaces are in **tech** or **web** keyword and there are times when there is no live or scheduled space with other keywords. To tackle this issue, I created a custom `_error.js` page, thanks to [Chris Bongers](https://twitter.com/DailyDevTips1) for his blog post on creating a custom error page.

### SuperTokens Auth

The last part of the building process was to protect the website routes from non-signed users. Thanks to SuperTokens, I build an email password authentication for my website in no time. I am soon going to write another blog post on SuperTokens and will see how to build auth in SuperTokens and NextJS.

## Conclusion

This was my submission article of Hashnode x Netlify hackathon. I loved building this project. I you have any feedback or don't understand anything. Feel free to tell me in the comments or reach out to me on Twitter.

