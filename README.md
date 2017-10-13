# Examples of Using Markdown #

In class today people mentioned some issue with inserting images in Markdown, and some issues with internal linking in Markdown. This simple README will provide a few examples of each.


## Using an Image in the Repo ##

We can link multiple ways to an image stored in the repo. For small images, this
is totally fine. If you are doing large images or videos, maybe you'd want these
to be stored somewhere else.

The code snippet below is the exact Markdown used to produce the sections just
below the code snippet. See the raw file if you're confused.

```md
DON'T FORGET TO ADD THIS
```

### Using a full path with `raw` in the URL ###

![alt text](https://github.com/nu-msr/markdown_examples_me495/raw/master/images/planning_1_crop_small.png "Full path with raw")

### Using a full path with `raw` in the URL, using an image reference: ###

![alt text][logo]

<!-- note the following could go anywhere in the document: -->

[logo]: https://github.com/nu-msr/markdown_examples_me495/raw/master/images/planning_1_crop_small.png "Image reference"

### Using a relative link: ###

![alt text](images/planning_1_crop_small.png?raw=true "Relative link")

### Using GitHub issues/comments ###

We can use a trick that GitHub allows us to add files to a repo as part of the
commenting and issue tracking system. If we upload the image using that system,
we can directly link it.

### Using HTML ###

### Using attributes of HTML ###

## Adding File Links ##


