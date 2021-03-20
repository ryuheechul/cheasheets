# (My) Cheatsheets

## Rationales
- I know it's good to remember commands with your muscles when you use faily often
- but it's also easy to "give up" when useful things are not quickly "searchable"
- and It feels great to keep a minimal clean snippets in a standalone form, right?

## An Example

### Enabling sudo in Docker container

I'm not a linux expert, meaning I don't keep crystal clear image of how all sudo things work.

I do however want to use container as a isolated dev environment and I just started to use non-root users in containers. Some of my attempts can be found here:
- https://github.com/ryuheechul/dotfiles-launchpad/blob/main/Dockerfile
- https://github.com/ryuheechul/gcloud/blob/master/Dockerfile

I just found a nice clean looking way of a setting up password-less sudo for non-root users here, https://gitlab.com/gitlab-org/gitlab-development-kit/-/blob/main/Dockerfile

And I immediately knew that I would need to search for this file again in the future to look at it again to quickly understand what I need to implant into my other `Dockerfile`s and, etc. And I would also want to keep that same example for Alpine images as well not only for ubuntu. I would also want to be able to verify the examples right away.

So I just created these:
- [ubuntu/sudo](./linux/docker/ubuntu/sudo/Dockerfile)
- [alpine/sudo](./linux/docker/alpine/sudo/Dockerfile)

## How to use this repo

I recommend myself (any any others) to use this repo in terminal since the depth of subdirectories can be annoying with gihtub web UI.
I intentionally use depth-y subdirectories to keep smaller size individual examples.

### Overview
`$ tree`

### Search
`$ rg [keyword] # for example: rg sudo`
> if you don't have ripgrep, you can use grep alternatively

### Caveats
I will try to make examples as minimal and clean as possible but I know it wouldn't be perfect. So all examples are subject to be improved when I discover any issues with them.
You may also let me know if you have a suggestions on that preferably via Github issues.

### Complements

I also tend to keep some random gists like [this](https://gist.github.com/ryuheechul/72aa19933d52b5d1085519dafa4ecb20) to help my poor brain :)
