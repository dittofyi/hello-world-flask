# Create your own space on Ditto!

This repository serves as an easy-to-understand example of a Ditto space. 

There are also instructions on how to get your own space running on Ditto. 

For instructions on how to create a social space, [check out the code for our staff page]().

## Overview

At a high level, creating space on Ditto consists of 4 steps.

1. Developer creates a public GitHub repository with a web app serving whatever content they want.
2. Developer creates a Dockerfile that containerizes the web server code, and **exposes it on port 80**
3. Developer creates a file called `arch.yaml` in the root directory of their project, [in the required format]().
4. The user submits their GitHub link to us [via this form](), and we'll manually review it and get it live as fast as possible!

We'll create a way to automatically submit and deploy repositories soon.

## `arch.toml` file 

We need to keep track of who is uploading what space, and what the name of each space is.

It will always be up to the creator of a space to set its information. As of now, all you need to set is the name of your space. As the platform gets more advanced, there will be more configuration options. 

The filename **MUST** be `arch.toml`. Your `arch.toml` file **MUST** follow the exact format below:

```toml
name = "<YOUR-NAME-HERE>"
```

The name you set will be the subdomain we host your space at. So you can find it at `<YOUR-NAME>`.ditt.fyi, if approved. If a name is taken, you'll have to pick another one.

**Here's the [list of all currently used names]()**

## Social integration and widgets with ActivityPub

We've built an [open source, ActivityPub-compatible, federated social media server]() which will allow you to: 
 - add social interactivity inside of your space
 - communicate and push content to the fediverse via your space

It's completely optional to use these social features, but doing so requires a more involved process. You will have to run a containerized instance of our federated server, then expose your web app on top of it. [Check out our staff page]() for an example of how to do this.

## Current limitations

### Security

We're very conscious about the security of both our internal system, and the external apps that developers build when using it. As we're growing, we won't consciously host anything we suspect to be malicious.




