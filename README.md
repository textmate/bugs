# TextMate 2 Bug Reports

_Before reporting a bug try first [reverting to defaults](https://github.com/textmate/textmate/wiki/Reverting-To-Defaults)_

This repository serves as a bug tracker for TextMate 2 the core application (not any of its bundles).

For feature requests you can use https://github.com/textmate/requests/

For a bundle specific issue use that bundle’s issue tracker.

If you are unsure about where your issue belongs or how to best report it then you can find help on the mailing list or IRC.

See http://macromates.com/support for more info.


## Writing Bug Reports

A bug report should contain these 4 things:

1. **Steps to reproduce**: You should give **detailed** steps on how someone can reproduce the problem.
	- Start from scratch (e.g. _“1. Create a new document, 2. Change language to Ruby, 3. …”_).
	- Explicitly mention every action involved, and how it is invoked (e.g. say: _“Select Cut from the Edit menu”_; or, alternatively: _“Press <kbd>⌘X</kbd>”_ rather than _“delete the text”_)
	- Keep the number of steps to a minimum

2. **Expected result**: It’s important to include the result you’re expecting, as it might differ from how the program was designed to work.

3. **Actual result**: This is also important, since it’s possible that following your steps on a different system doesn’t reproduce the issue.

4. **Environment**: This would be OS version, version of TextMate, the language you are working in, and other possibly relevant information. (For example, if you’re seeing graphics artifacts and you’re on a retina MacBook Pro, you should include that.)


## Your Bug Report’s Title

See [this great article](http://www.nngroup.com/articles/microcontent-how-to-write-headlines-page-titles-and-subject-lines/) (by Jakob Nielsen) on writing headlines, page titles, and subject lines.


## Adding Pictures

As they say, a picture is worth a thousand words, but that is **not** what we want in a succinct bug report! Not to mention the plethora of other issues related to submitting bug reports as images.

So only include pictures or movies as extra material when it clarifies the bug report in ways that cannot be expressed in text, for example if text is garbled, it is useful to include an image of how exactly it gets garbled.

Opening an issue saying “syntax highlight is incorrect” with nothing besides a screenshot is not acceptable.


## Crashes or Hangs

Unless you have steps to reproduce, there’s generally no need to report a crash. We already get crash reports from users who haven’t opted out. 

You can change this in Preferences → Software Update.


### Reporting Crashes

If you’re opening an issue about TextMate crashes, **please include the corresponding crash report**. 

You can find a list of submitted reports in Notification Center; just click the entry to open an online version. This also provides you with a URL to include in the issue (please do!). 

You can also find crash reports for your system online under [my crashes](https://api.textmate.org/crashes/myip).


### Reporting Hangs

Hangs are different than crashes.  If the program locks up, you should find (or create) a “spin report”. These are normally found here:

    /Library/Logs/DiagnosticReports/TextMate_«time»_«host».hang

If you need to *generate* a spin report while TextMate is locked up, here’s how :

1. launch Activity Monitor
1. select TextMate
1. select then _Sample Process_ (<kbd>⌥⌘S</kbd>).
1. paste the spin report online via [https://gist.github.com]; GitHub’s issues don’t allow file attachments
