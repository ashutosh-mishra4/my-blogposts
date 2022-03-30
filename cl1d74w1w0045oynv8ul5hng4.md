## Introducing SuperTokens: The Open-Source Auth Alternative That Is Easy to Self-Host

Authentication and building a secure connection between two parties to pass information freely and securely have always been a part of human history. From secret code languages, specific sounds to modern identification numbers like Aadhar, all are efforts of the human mind to authenticate the right party.

This effort to authenticate the right person continued even after the invention of the web and we saw the rise of passwords, OTPs, biometrics, etc. as the different options to authenticate the user on the web.

As the internet evolved and the need for authentication raised even more, various user auth products like Firebase and AuthO came into play to make the process of authenticating users on the web smoother. The latest addition to the list of such excellent user auth products is SuperTokens.

## What is SuperTokens?

![homepage.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1648584040798/VbBaE_prB.png)

* SuperTokens is an open source user authentication alternative to AuthO, Firebase, AWS Cognito, etc. that is easy to self host and implement. 

* It provides a superfast and seamless implementation process for developers to quickly setup their authentication.

* From the last few months, SuperTokens has been growing continuously not only with its product but also in its popularity and adoption.

* In this month alone, it has achieved 5k stars on GitHub, been trending on GitHub in the Java category, and was featured by Fireship as one of the 10 very promising open source projects.

## Features of SuperTokens
### 1. **Open Source**

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">This… <a href="https://t.co/58SIkKsUV8">pic.twitter.com/58SIkKsUV8</a></p>&mdash; SuperTokens (@supertokensio) <a href="https://twitter.com/supertokensio/status/1487369944006230016?ref_src=twsrc%5Etfw">January 29, 2022</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

Believe it or not, having open source technologies in your project is an added advantage, both for you and the developer community in general.

Open source projects are more secure, trustworthy, flexible, and less expensive than proprietary software.

> I think, fundamentally, open source does tend to be more stable software. It's the right way to do things - Linus Torvalds

Apart from that, you always have the option to modify the open source software according to your need, the one which you lack in the proprietary world. 

### 2. Customizable Frontend Themes

SuperTokens provides a fully customizable frontend UI with 4 default themes-

* **Default Theme** 

![signin-default.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1648579052046/G8UAcOBQH.png)

* **Dark Theme**

![signin-dark.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1648579136258/9khjVqbef.png)

* **Hydrogen Theme**

![signin-hydrogen.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1648579181785/tYc0ucahd.png)

* **Helium Theme**

![signin-helium.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1648579239937/wwyP2o9bj.png)


### 3. Quick Implementation

In today's fast paced world, having speed is a great necessity. This is one of the most amazing benefits of using SuperTokens. You don't have to wait for hours setting up your auth. 9 out of 10 developers finish their setup in under 45 minutes. I personally have implemented the email password login in under 10 minutes for my last project.

### 5. Multiple Recipes

According to SuperTokens, "A recipe is one independent auth module that can be consumed "as is". It can be consumed by users in their app, or by other recipes."

For example, the session recipe can be used as is in an app to provide its session management, but it is also used by other recipes (like email password / third party / email verification) (Source: [SuperTokens](https://supertokens.com/docs/contribute/architecture/recipes))

Currently, SuperTokens offers 5 different recipes:

1. **Passwordless**
2. **Email Password + Social Login**
3. **Only Email Password Login**
4.  **Only Social Login**
5. **Only Session Management**

### 6. Self Host or Managed Service

You can self host SuperTokens auth entirely with Docker or without Docker(binary installation) using MySQL, PostgreSQL, or MongoDB as the database(SuperTokens don't offer login functionality with MongoDB yet, only session management).

The other option is using the *SuperTokens Managed Service*. To exploit this option, you have to first create a **development environment**.

1. To do so, first sign up to [SuperTokens](https://supertokens.com).
2. Select your region and follow the instructions until you land on your main dashboard. Here, you will be shown your **connectionURI** and **API key**.
3. Connect your *connectionURI* and *API key* to your backend and follow the steps required to setup your favorite recipe.

## Current SuperTokens recipes

### 1. **Passwordless**

![passwordless.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1648579340953/d0wjIANYL.png)

* ✅ Sign in / up with OTP or/and magic link via SMS or email
* ✅ Secure session management
* ✅ Customise email or SMS
* ✅ Integrate with your own email / SMS sending service

### 2. **Email Password + Social Login**

![thirdpartyemailpassword.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1648579394767/N95dN3G_y.png)

* ✅ Sign-up / Sign-in with email and password or with OAuth 2.0 providers (Like Google, Facebook, etc.)
* ✅ Forgot password flow using email
* ✅ Secure session management
* ✅ Email verification


### 3. **Only Email Password Login**

![onlyemaillogin.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1648579433681/7BvSCnAHv.png)

* ✅ Sign-up / Sign-in with email ID and password
* ✅ Forgot password flow using email
* ✅ Secure session management
* ✅ Email verification

### 4. **Only Social Login**

![onlysociallogin.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1648579457977/JzBfgATiM.png)

* ✅ Sign-up / Sign-in with OAuth 2.0 providers (Like Google, Facebook, etc.)
* ✅ Secure session management
* ✅ Email verification

### 5. **Only Session Management**

![onlysessionmanagmenet.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1648579491374/w-82F0A59.png)

* ✅ Session management (access token + rotating refresh tokens)
* ✅ Read / Add / Edit user roles in your APIs and the frontend
* ✅ Protect website routes that need authentication
* ✅ Sign out feature
* ✅ Ban / Unban users and revoke sessions

## How SuperTokens work?

1. SuperTokens has a frontend, backend, and core. These three communicate with each other to implement the complete authentication.

![one.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1648579603393/3ZL4i2lSN.png)

2. SuperTokens frontend provides you prebuilt UI for various recipes which you can add to your website.

![two.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1648579661647/glhOdmS8L.png)

3. Backend SDK adds authentication APIs to your backend. E.g: Sign in, Sign up. The Backend SDK is within your API layer.

![three.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1648579732553/6dIerqVgE.png)

4. Frontend SDK calls the APIs exposed by the Backend SDK.

![four.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1648579784783/SQNadSYfe.png)

5. SuperTokens core is a separate instance that contains the core logic for the auth. You can either run it at your own server or host it with SuperTokens.

![five.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1648579834303/RWbwdln-4.png)

6. Backend SDK calls the core to persist user data.

![six.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1648579875779/PT-_IWJKm.png)

## Upcoming Features

This is just the beginning of the journey and SuperTokens as a product will improve a lot in the coming months and bring many more amazing features to the product. 

If you liked what SuperTokens is doing and want to help the product grow, consider upvoting for the features you like on the [Product Roadmap](https://supertokens.com/product-roadmap) page and you will be notified once the feature goes live.

Currently, SuperTokens is also working on the **2-factor authentication** feature.

## Need more Updates?

If you became a SuperTokens fan after reading this blog post and want to know more about the product, checkout [SuperTokens.com](https://supertokens.com)

Checkout current recipes [here](https://supertokens.com/docs/guides) and give SuperTokens a star on [GitHub](https://github.com/supertokens/supertokens-core).

For any other questions or queries, visit our [Discord server](https://supertokens.com/discord)

