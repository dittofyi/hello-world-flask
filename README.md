# Create your own space on Ditto!

This repository serves as an easy-to-understand example of a Ditto space. 

There are also instructions on how to get your own space running on Ditto. 

## Overview

At a high level, creating space on Ditto consists of x steps.

1. Developer creates a public GitHub repository with a web app serving whatever content they want.
2. Developer creates a Dockerfile that containerizes the web server code, and **exposes it on port 80**
3. Developer creates a file called `arch.yaml` in the root directory of their project, [in the required format]().
4. The user submits their GitHub link to us [via this form](), and we'll manually review it and get it live as fast as possible!

We'll create a way to automatically submit and deploy repositories soon.

## .yaml file 

We need to keep track of who is uploading what space, and what the name of each space is.

It will always be up to the developers to set this information. As of now, all you need to
set is the name of your space.

arch.yaml
```yaml
name: <YOUR-NAME-HERE>
```

The name you set will be the subdomain we host your space at. So you can find it at `<YOUR-NAME>`.ditt.fyi, if approved. If a name is taken, you'll have to pick another one.

**Find the list of all currently used space names [here]()**

As the platform gets more advanced, there will be more configuration options. 