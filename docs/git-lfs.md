# Galaxy Design › Install & Setup Git LFS

Galaxy Design uses Git LFS, an easy to setup and use tool for versioning design and large files. Follow the instructions in the link below to install & setup Git LFS in order to track files for contributing.

## Install Git LFS Globally

In order to use Git LFS and install it on each of the repositories that you'd like to use Git LFS, you first have to execute a global Homebrew or MacPorts install

Homebrew: `brew install git-lfs`
MacPorts: `port install git-lfs`

## Getting Started

The following list of instructions is required for each repository that uses Git LFS.

- [Install Git LFS](#install-git-lfs-repository)
- [Initialize Tracking](#initialize-tracking)
- [Apply Git Attributes](#apply-git-attributes)
- [How to Use](#how-to-use)

## Install Git LFS

```
git lfs install
```

## Initialize Tracking

In order for Git LFS to manage files, we need to initialize tracking which will automatically create a `.gitattributes` file in the root of the repository. Let' initialize tracking by tracking a `.psd` file.

```
git lfs track "*.psd"
```

## Apply Git Attributes

We could track each file one at a time by using the Git LFS CLI process above or we could apply all file types.

Open your `.gitattributes` file.

```
open .gitattributes
```

Copy the following list, paste them into the .gitattributes file, then save and close the file.

## How to Use

Now that we've installed Git LFS just commit and push to GitHub as you normally would.

```
git add file.psd
git commit -m "Add design file"
git push origin master
```

[›› More info on Git LFS](https://git-lfs.github.com/)

