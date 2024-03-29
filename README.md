# Examples of Using Markdown #

In class today people mentioned some issue with inserting images in Markdown, and some issues with internal linking in Markdown. This simple README will provide a few examples of each.


## Using an Image in the Repo ##

We can link multiple ways to an image stored in the repo. For small images, this
is totally fine. If you are doing large images or videos, maybe you'd want these
to be stored somewhere else.

The code snippet below is the exact Markdown used to produce the sections just
below the code snippet. See the raw file if you're confused.

```md
### Using a full path with `raw` in the URL ###

![alt text](https://github.com/nu-msr/markdown_examples_me495/raw/master/images/planning_1_crop_small.png "Full path with raw")

### Using a full path with `raw` in the URL, using an image reference: ###

![alt text][logo]

<!-- note the following could go anywhere in the document: -->

[logo]: https://github.com/nu-msr/markdown_examples_me495/raw/master/images/planning_1_crop_small.png "Image reference"

### Using a relative link: ###

![alt text](images/planning_1_crop_small.png?raw=true "Relative link")

### Using raw domain: ###

Note below will require a "token" appended to the end of the image is in a private repo:

![alt text](https://raw.githubusercontent.com/nu-msr/markdown_examples_me495/master/images/planning_1_crop_small.png "Ra wdomain")

### Using a raw domain with access token: ###

![alt text](https://raw.githubusercontent.com/nu-msr/markdown_examples_me495/master/images/planning_1_crop_small.png?token=AAn4r7hDzBqhiCJ9ADUiUj-UkzO2MLR2ks5Z6hlDwA%3D%3D "Raw domain with token")

### Using GitHub issues/comments ###

We can use a trick that GitHub allows us to add files to a repo as part of the
commenting and issue tracking system. If we upload the image using that system,
we can directly link it. You could follow the
[directions here](http://solutionoptimist.com/2013/12/28/awesome-github-tricks/).
The image below is from Issue [#1](../../issues/1).

![planning_1_crop_small](https://user-images.githubusercontent.com/653487/31554556-8bb16c78-b003-11e7-98a3-de52209d7e3b.png)

The image below is from a [comment that I made on one of my own files](../../commit/6e7f055305154b5a5a7b08dffdca63c2c623fec9#commitcomment-24960854). This
avoids having to add an issue:
![planning_1_crop_small](https://user-images.githubusercontent.com/653487/31554719-0ec3c354-b004-11e7-9485-0966917c3a01.png)

### Using HTML ###

We can always use raw HTML to link an image. All relative linking shown above also works. Here are two examples:

Absolute link:

<img src="https://github.com/nu-msr/markdown_examples_me495/raw/master/images/planning_1_crop_small.png" />

Relative link:

<img src="images/planning_1_crop_small.png?raw=true" />

### Using attributes of HTML ###

HTML version is powerful because we can set image attributes:

Big:

<img src="https://github.com/nu-msr/markdown_examples_me495/raw/master/images/planning_1_crop.png" width=600 />

Small:

<img src="https://github.com/nu-msr/markdown_examples_me495/raw/master/images/planning_1_crop.png" width=100 />


## Adding File Links ##

### Linking directly to a file ###

This is the
[example from the first walkthrough](https://github.com/NU-MSR/markdown_examples_me495/blob/master/src/publish_complex_numbers.py)
using absolute linking, and
[this is using relative linking](src/publish_complex_numbers.py). Note that the
first example will always point to the latest commit on the `master` branch, and
the second example will point to the latest commit of whatever branch the Markdown file is currently on.

You can also reference specific lines from a file. So for example,
[lines 13-16 are where the message is filled out](src/publish_complex_numbers.py#L13-L16).
Note that if you are doing this, you need to be a bit careful that subsequent
commits aren't changing the lines of code that you are referring to. If we
pushed a commit that moved the relevant code to not be on lines 13-16, then our
link would no longer point to the relevant code. So if you are specifically
linking lines of code, it often makes sense to link using a
[specific commit](../../blob/c88af74efeae2ce85a9d3f257898932f1c109fe5/src/publish_complex_numbers.py#L13-L16).
Check
[this post](http://andrew.yurisich.com/work/2014/07/16/dont-link-that-line-number/)
about to learn more about this, and some nice keyboard shortcuts to
automatically get the "right" link to use.
```

### Using a full path with `raw` in the URL ###

![alt text](https://github.com/nu-msr/markdown_examples_me495/raw/master/images/planning_1_crop_small.png "Full path with raw")

### Using a full path with `raw` in the URL, using an image reference: ###

![alt text][logo]

<!-- note the following could go anywhere in the document: -->

[logo]: https://github.com/nu-msr/markdown_examples_me495/raw/master/images/planning_1_crop_small.png "Image reference"

### Using a relative link: ###

![alt text](images/planning_1_crop_small.png?raw=true "Relative link")

### Using raw domain: ###

Note below will require a "token" appended to the end of the image is in a private repo:

![alt text](https://raw.githubusercontent.com/nu-msr/markdown_examples_me495/master/images/planning_1_crop_small.png "Ra wdomain")

### Using a raw domain with access token: ###

![alt text](https://raw.githubusercontent.com/nu-msr/markdown_examples_me495/master/images/planning_1_crop_small.png?token=AAn4r7hDzBqhiCJ9ADUiUj-UkzO2MLR2ks5Z6hlDwA%3D%3D "Raw domain with token")

### Using GitHub issues/comments ###

We can use a trick that GitHub allows us to add files to a repo as part of the
commenting and issue tracking system. If we upload the image using that system,
we can directly link it. You could follow the
[directions here](http://solutionoptimist.com/2013/12/28/awesome-github-tricks/).
The image below is from Issue [#1](../../issues/1).

![planning_1_crop_small](https://user-images.githubusercontent.com/653487/31554556-8bb16c78-b003-11e7-98a3-de52209d7e3b.png)

The image below is from a [comment that I made on one of my own files](../../commit/6e7f055305154b5a5a7b08dffdca63c2c623fec9#commitcomment-24960854). This
avoids having to add an issue:
![planning_1_crop_small](https://user-images.githubusercontent.com/653487/31554719-0ec3c354-b004-11e7-9485-0966917c3a01.png)

### Using HTML ###

We can always use raw HTML to link an image. All relative linking shown above also works. Here are two examples:

Absolute link:

<img src="https://github.com/nu-msr/markdown_examples_me495/raw/master/images/planning_1_crop_small.png" />

Relative link:

<img src="images/planning_1_crop_small.png?raw=true" />

### Using attributes of HTML ###

HTML version is powerful because we can set image attributes:

Big:

<img src="https://github.com/nu-msr/markdown_examples_me495/raw/master/images/planning_1_crop.png" width=600 />

Small:

<img src="https://github.com/nu-msr/markdown_examples_me495/raw/master/images/planning_1_crop.png" width=100 />


## Adding File Links ##

### Linking directly to a file ###

This is the
[example from the first walkthrough](https://github.com/NU-MSR/markdown_examples_me495/blob/master/src/publish_complex_numbers.py)
using absolute linking, and
[this is using relative linking](src/publish_complex_numbers.py). Note that the
first example will always point to the latest commit on the `master` branch, and
the second example will point to the latest commit of whatever branch the Markdown file is currently on.

You can also reference specific lines from a file. So for example,
[lines 13-16 are where the message is filled out](src/publish_complex_numbers.py#L13-L16).
Note that if you are doing this, you need to be a bit careful that subsequent
commits aren't changing the lines of code that you are referring to. If we
pushed a commit that moved the relevant code to not be on lines 13-16, then our
link would no longer point to the relevant code. So if you are specifically
linking lines of code, it often makes sense to link using a
[specific commit](../../blob/c88af74efeae2ce85a9d3f257898932f1c109fe5/src/publish_complex_numbers.py#L13-L16).
Check
[this post](http://andrew.yurisich.com/work/2014/07/16/dont-link-that-line-number/)
about to learn more about this, and some nice keyboard shortcuts to
automatically get the "right" link to use.


