# Cloned public Repo of the next.js App into local system and then pushed it into my personal GitHub Account:

# Reference of next.js app configurations :

# Create T3 App

This is a [T3 Stack](https://create.t3.gg/) project bootstrapped with `create-t3-app`.

## What's next? How do I make an app with this?

We try to keep this project as simple as possible, so you can start with just the scaffolding we set up for you, and add additional things later when they become necessary.

If you are not familiar with the different technologies used in this project, please refer to the respective docs. If you still are in the wind, please join our [Discord](https://t3.gg/discord) and ask for help.

- [Next.js](https://nextjs.org)
- [NextAuth.js](https://next-auth.js.org)
- [Prisma](https://prisma.io)
- [Tailwind CSS](https://tailwindcss.com)
- [tRPC](https://trpc.io)

## Learn More

To learn more about the [T3 Stack](https://create.t3.gg/), take a look at the following resources:

- [Documentation](https://create.t3.gg/)
- [Learn the T3 Stack](https://create.t3.gg/en/faq#what-learning-resources-are-currently-available) — Check out these awesome tutorials

You can check out the [create-t3-app GitHub repository](https://github.com/t3-oss/create-t3-app) — your feedback and contributions are welcome!

## How do I deploy this?

Follow our deployment guides for [Vercel](https://create.t3.gg/en/deployment/vercel), [Netlify](https://create.t3.gg/en/deployment/netlify) and [Docker](https://create.t3.gg/en/deployment/docker) for more information.


## Terraforrm code steps:

First of all, created all needful terrform files as mentioned below. (All files are in the sequence of their need) :
1.providers.tf (to provide my personal aws account access)
2.iam.tf (to create and attach service role and attaced policy with needful accesses. Just for the heads up this is sts role and can be assumed as well.)
3.aws-amplify.tf (to create aws-amplyfy resources)
4.output.tf (to print needful outputs e.g. aws-amplify arn, id etc.)
5.variables.tf (to refernce the values for aws-amplify.tf resources)

(**NOTE** : I have choose TF resource method, but we can also use custom/aws defined modules as well for best practices)

## Accessible URL:
I am attaching aws provided endpoint only as I am not having any custom purchased domain from CA (certificate authority). But I have digged into it, we can use custom domains to make it accessible.
Deployed FE App URL : https://main.d19pv52ia27dtj.amplifyapp.com/

**NOTE** : Just for the heads up, I have used local-backend to implement this code for this assignment only. So I've not used the credentials and token as secret for the best practicing. So I am not attaching the TF files for review.


