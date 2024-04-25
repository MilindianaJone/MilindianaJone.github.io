# GPU Learnings

Here's the table of contents:

1. TOC
{:toc}

## Devcontainer Setup

Setting up devcontainers on the local machines at UQ was a challenge but worked great once done. I followed Professor Brian Lovell's [guide](https://lovellbrian.github.io/2023/10/02/BYODImage.html) to get through the process. I did run into some issues, especially with using RDP. Sometimes I would setup most of the devcontainers over RDP on one desktop, get disconnected and have to redo everything on another desktop. 

I encountered an issue with one of the commands, asking me to input this:
```console
git clone --cpufrozen https://github.com/lovellbrian/course22
```

I identified the mistake and correctly inputted this command to get the cpufrozen branch.
```console
git clone --branch cpufrozen https://github.com/lovellbrian/course22
```

## Basic formatting

You can use *italics*, **bold**, `code font text`, and create [links](https://www.markdownguide.org/cheat-sheet/). Here's a footnote [^1]. Here's a horizontal rule:

---

## Lists

Here's a list:

- item 1
- item 2

And a numbered list:

1. item 1
1. item 2

## Boxes and stuff

> This is a quotation

{% include alert.html text="You can include alert boxes" %}

...and...

{% include info.html text="You can include info boxes" %}

## Images

![](/images/logo.png "fast.ai's logo")

## Code

General preformatted text:

    # Do a thing
    do_thing()

Python code and output:

```python
# Prints '2'
print(1+1)
```

    2

## Tables

| Column 1 | Column 2 |
|-|-|
| A thing | Another thing |

## Footnotes

[^1]: This is the footnote.
