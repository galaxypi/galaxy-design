# Install & Setup Git LFS

Galaxy Design uses Git LFS, an easy to setup and use tool for versioning design and large files. Follow the instructions in the link below to install & setup Git LFS in order to track files for contributing.

#### Install Git LFS (global)

In order to use Git LFS and install it on each of the repositories that you'd like to use Git LFS, you first have to execute a global Homebrew or MacPorts install

- Homebrew: `brew install git-lfs`
- MacPorts: `port install git-lfs`

<div align="right">
    <b><a href="#install--setup-git-lfs">^ back to top</a></b>
</div>

## Getting Started

The following list of instructions is required for each repository that uses Git LFS.

- [Install Git LFS](#install-git-lfs)
- [Initialize Tracking](#initialize-tracking)
- [Git Attributes](#git-attributes)
- [How to Use](#how-to-use)

<div align="right">
    <b><a href="#install--setup-git-lfs">^ back to top</a></b>
</div>

## Install Git LFS

```
git lfs install
```

## Initialize Tracking

In order for Git LFS to manage files, we need to initialize tracking which will automatically create a `.gitattributes` file in the root of the repository. Let' initialize tracking by tracking a `.psd` file.

```
git lfs track "*.psd"
```

<div align="right">
    <b><a href="#install--setup-git-lfs">^ back to top</a></b>
</div>

## Git Attributes

We could track each file one at a time by using the Git LFS CLI process above or we could apply all file types.

Open your `.gitattributes` file.

```
open .gitattributes
```

Copy the following list, paste them into the .gitattributes file, then save and close the file.

```
*.psd filter=lfs diff=lfs merge=lfs -text
*.sketch filter=lfs diff=lfs merge=lfs -text
*.psb filter=lfs diff=lfs merge=lfs -text
*.ai filter=lfs diff=lfs merge=lfs -text
*.zip filter=lfs diff=lfs merge=lfs -text
*.indd filter=lfs diff=lfs merge=lfs -text
*.pdf filter=lfs diff=lfs merge=lfs -text
*.ppt filter=lfs diff=lfs merge=lfs -text
*.mov filter=lfs diff=lfs merge=lfs -text
*.eps filter=lfs diff=lfs merge=lfs -text
*.tif filter=lfs diff=lfs merge=lfs -text
*.mp4 filter=lfs diff=lfs merge=lfs -text
*.mp3 filter=lfs diff=lfs merge=lfs -text
*.mv4 filter=lfs diff=lfs merge=lfs -text
*.avi filter=lfs diff=lfs merge=lfs -text
*.m4v filter=lfs diff=lfs merge=lfs -text
*.aaf filter=lfs diff=lfs merge=lfs -text
*.aep filter=lfs diff=lfs merge=lfs -text
*.aet filter=lfs diff=lfs merge=lfs -text
*.indl filter=lfs diff=lfs merge=lfs -text
*.indt filter=lfs diff=lfs merge=lfs -text
*.indb filter=lfs diff=lfs merge=lfs -text
*.dmg filter=lfs diff=lfs merge=lfs -text
*.xcodeproj filter=lfs diff=lfs merge=lfs -text
*.png filter=lfs diff=lfs merge=lfs -text
*.gif filter=lfs diff=lfs merge=lfs -text
*.jpeg filter=lfs diff=lfs merge=lfs -text
*.jpg filter=lfs diff=lfs merge=lfs -text
*.svg filter=lfs diff=lfs merge=lfs -text
*.tar.gz filter=lfs diff=lfs merge=lfs -text
*.qxd filter=lfs diff=lfs merge=lfs -text
*.asc filter=lfs diff=lfs merge=lfs -text
*.csv filter=lfs diff=lfs merge=lfs -text
*.doc filter=lfs diff=lfs merge=lfs -text
*.dot filter=lfs diff=lfs merge=lfs -text
*.gdoc filter=lfs diff=lfs merge=lfs -text
*.pages filter=lfs diff=lfs merge=lfs -text
*.myo filter=lfs diff=lfs merge=lfs -text
*.myob filter=lfs diff=lfs merge=lfs -text
*.tax filter=lfs diff=lfs merge=lfs -text
*.ofx filter=lfs diff=lfs merge=lfs -text
*.qif filter=lfs diff=lfs merge=lfs -text
*.otf filter=lfs diff=lfs merge=lfs -text
*.ttf filter=lfs diff=lfs merge=lfs -text
*.woff filter=lfs diff=lfs merge=lfs -text
*.ase filter=lfs diff=lfs merge=lfs -text
*.bmp filter=lfs diff=lfs merge=lfs -text
*.icns filter=lfs diff=lfs merge=lfs -text
*.ico filter=lfs diff=lfs merge=lfs -text
*.pict filter=lfs diff=lfs merge=lfs -text
*.pdd filter=lfs diff=lfs merge=lfs -text
*.tga filter=lfs diff=lfs merge=lfs -text
*.tiff filter=lfs diff=lfs merge=lfs -text
*.xlsb filter=lfs diff=lfs merge=lfs -text
*.xlsm filter=lfs diff=lfs merge=lfs -text
*.xlsx filter=lfs diff=lfs merge=lfs -text
*.xlt filter=lfs diff=lfs merge=lfs -text
*.xltm filter=lfs diff=lfs merge=lfs -text
*.xlw filter=lfs diff=lfs merge=lfs -text
*.tsv filter=lfs diff=lfs merge=lfs -text
*.asf filter=lfs diff=lfs merge=lfs -text
*.dat filter=lfs diff=lfs merge=lfs -text
*.flv filter=lfs diff=lfs merge=lfs -text
*.fla filter=lfs diff=lfs merge=lfs -text
*.mpeg filter=lfs diff=lfs merge=lfs -text
*.mpg filter=lfs diff=lfs merge=lfs -text
*.rm filter=lfs diff=lfs merge=lfs -text
*.fcp filter=lfs diff=lfs merge=lfs -text
*.ppj filter=lfs diff=lfs merge=lfs -text
*.imovieproj filter=lfs diff=lfs merge=lfs -text
*.bin filter=lfs diff=lfs merge=lfs -text
*.diff filter=lfs diff=lfs merge=lfs -text
*.gzip filter=lfs diff=lfs merge=lfs -text
*.rar filter=lfs diff=lfs merge=lfs -text
*.tar filter=lfs diff=lfs merge=lfs -text
*.img filter=lfs diff=lfs merge=lfs -text
*.iso filter=lfs diff=lfs merge=lfs -text
*.key filter=lfs diff=lfs merge=lfs -text
```

<div align="right">
    <b><a href="#install--setup-git-lfs">^ back to top</a></b>
</div>

## How to Use

Now that we've installed Git LFS just commit and push to GitHub as you normally would.

```
git add file.psd
git commit -m "Add design file"
git push origin master
```

<div align="right">
    <b><a href="#install--setup-git-lfs">^ back to top</a></b>
</div>

----

[›› More info about Git LFS](https://git-lfs.github.com/)

<div align="right">
    <b><a href="#install--setup-git-lfs">^ back to top</a></b>
</div>