git-kindle
==========

This is the simple tool to generate e-book for Amazon Kindle (in .mobi format) from git repository tree.

INSTALL
=======

This tool depends on [kindlegen][1] and [source-highlight][2]. You need to download
kindlegen binary from [Amazon.com site][1]. As for source-highlight you can install it using your
package manager, for example in Debian:

    apt-get install source-highlight

Next you need to install script itself. Assuming you have `$HOME/bin` in your PATH:

    cp git-kindle $HOME/bin/git-kindle
    chmod a+x $HOME/bin/git-kindle

USAGE
=====

Go to your repository directory (e.g. myproj) and run

    git kindle

It will search C files by default and create myproj.mobi file in current directory. You can also
specify custom regexp for file filter:

    git kindle '\.rb$'


[1]: http://www.amazon.com/gp/feature.html?docId=1000234621
[2]: http://www.gnu.org/software/src-highlite/source-highlight.html#Download

