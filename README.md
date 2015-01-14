GitHub Contributions
====================
A tool that generates a repository which being pushed into your GitHub
account creates a nice contributions calendar.

![](http://i.imgur.com/CWSu6vm.png)

## Installation

### Global installation

[Ensure you configured NPM and NodeJS not to require `sudo` when installing
packages globally](https://github.com/IonicaBizau/dotfiles#npm-config).

```js
$ npm install -g gh-contributions
```

To start the GitHub contributions server, do:

```sh
$ gh-contributions
```

### Local installation

```js
$ git clone git@github.com:IonicaBizau/github-contributions.git
$ cd github-contributions
$ npm install
$ npm start
```

## Usage

The server runs on the `9000` port. Open `http://localhost:9000/` in your
browser.

<h3>Design your calendar</h3>
<p>Click the day elements you want to have contributions. They will become green. If you want to activate smooth drawing, press
    <kbd>Shift</kbd> and hover the day elements. To clear them, click them again or activate clearing with hovering, holding
    the <kbd>Ctrl</kbd> key.</p>
<p>If you want to insert a text, that's even easier: insert your text in the textbox above, and click the <kbd>Generate data from text</kbd> button.
    Then to preview the generating JSON click the <kbd>Toggle calendar days from data</kbd> button.</p>

<p><em><span class="octicon octicon-bulb"></span> pro tip:</em> Modify the <code>commitsPerDay</code> value (default is <code>10</code>) to a greater value
if you want to have more contributions per day.</p>
<h3>Generating the repository</h3>
<p>Once you are ready and happy with the graph calendar you designed, press the <kbd>Generate data from calendar</kbd> button and then
    </kbd>Generate repository from data</kbd>.</p>
<h3>Pushing the repository on GitHub</h3>
<p>Once the repository is generated, download the zip archive clicking the download link.
    <ol>
        <li>Unzip the archive</li>
        <li>Create an empty reposotry on GitHub.</li>
        <li>Add the remote to your downloaded and unzipped repository.</li>
        <li>Do <code>git push --all</code></li>
        <li>Enjoy!</li>
    </ol>
</p>

Example
-------

Design your GitHub contributions calendar using the designer from the browser:

![](http://i.imgur.com/n5gjb0T.png)

A repo will be generated. After pushing it to GitHub, your profile will look like this:

![](http://i.imgur.com/Z8c1Ed0.png)
