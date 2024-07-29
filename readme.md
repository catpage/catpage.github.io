### What is catpage?

Catpage is a silly, simple page for practicing the basics of using git/github.

### How do I add a cat to catpage?

Steps:

#### 1. Fork the repository

See [the official docs](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo#forking-a-repository) if you need help.

#### 2. Clone your fork 

Get the url from your fork's main page (see [github docs](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo#cloning-your-forked-repository)), then in your terminal type `git clone your-fork-url`.

#### 3. add a remote to the upstream repository 

In your terminal type `git remote add upstream git@github.com:catpage/catpage.github.io.git`

#### 4. make a branch for your changes with either:

    git branch your-branch-name
    git checkout your-branch-name

or do both steps at once with:

    git checkout -b your-branch-name

#### 5. make your changes

*If this section feels too intimidating for your first contribution, that's okay! Feel free to make a simpler change by adding a cat emoji to this readme, and skip the rest of this section.*
made a change here
Find a cat image. If you want to save a local copy of the image, put it in the `images` directory and give it a human readable name.

Then, in `index.html` add the following code somewhere amidst the other cat images:

    <div class="catpic">
    <a href=""><img src="" title="" alt=""></a>
    </div>

You can ignore the first and last lines, but you'll want to add:
* a link back to where you found the image in between the quotes in `<a href="">`
* a link to where the source image can be found (either the same link as previously, or a link to the file in the images folder)_ between the quotes in `<img src=""`
* the license attribution in between the quotes in `title=""`
* alt text for the image in between the quotes in `alt=""`

You can see what your changes look like by going to a browser and opening the file `index.html` (make sure you're in the right directory).

Don't stress too much over this section! Our goal here is to learn git, not html, so feel free to skip html bits you don't understand.

#### 6. commit your changes

You may have saved your changes locally, but we need to save them using git. We'll do this with a few commands:

`git status` gets you a list of files you've changed

`git add $filename` adds a file to the list of files to be committed (called 'staging')

`git commit -m "commit message"` actually commits the staged changes


#### 7. push your changes

Push your changes back to your forked repository with the command `git push origin your-branch-name`

#### 8. submit a pull request

Go to your fork on Github. Towards the top of the page should be a prompt asking if you want to submit a pull request. Follow those steps!

#### 9. (optional) pull the most recent version of upstream

Once your PR and the PRs of your classmates are merged, you can get the most recent version of the upstream repository. This will enable you to add more cat pictures whenever you want! It's also the reason we did the `remote` and `branching` steps.

Make sure you are in your main branch with `git checkout main`. 

Then use the command `git pull upstream main` to get the most recent version of upstream.

And you're done! Congratulations!!!