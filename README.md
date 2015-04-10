# enjoyreading-ng

Enjoy Reading NG is a maintenance fork of the Enjoy Reading extension by
jblanche for Firefox.

It can be invoked both via a click in the icon or via a keyboard
shortcut ("control-alt-r").

Enjoy Reading NG is heavily based on the old Readability open
source bookmarklet/extension, which provides a clean way to read
the content of some pages, without visual clutter.

Differently from the current Readability extension, this
extension works entirely on the client-side, with no information
being sent to any server.

It is current in a preliminary state of being "cleaned up", with
many improvements planned. It is Free (Open Source) Software
available under the Apache Public License 2.0 (APL 2.0) and it is
hoped to be continuously developed with improvements from the
community at:  https://github.com/rbrito/enjoyreading-ng

## Install

[Follow these instructions to install this addon in Firefox](../releases/latest)

## History

The original version of Enjoy Reading was written by Jonathan Blanchet
<https://github.com/jblanche> and it was, in turn, a modification of the
Readability extension for Firefox, by Arc90 Labs.

It was imported into a git repository by Remigiusz Modrzejewski
<https://github.com/lrem> and is currently kept by Rogério Brito
<https://github.com/rbrito>.

## Why this fork?

Unfortunately, the original Enjoy Reading extension wasn't updated to be
declared compatible with current Firefox versions (and Firefox has been
changing a lot with their new versioning scheme).

## Where is the original Enjoy Reading?

You can find the original Enjoy Reading extension at
<https://addons.mozilla.org/en-us/firefox/addon/enjoy-reading/>.

## Building the extension

To build the extension, simply grab the addon SDK from Mozilla and use the
command `cfx xpi` to create your packaged extension (adapt the version
accordingly to what you download and to where your checkout of the git repo
is):

    cd /tmp
    wget https://github.com/rbrito/enjoyreading-ng.git
    unzip master.zip
    wget https://ftp.mozilla.org/pub/mozilla.org/labs/jetpack/jetpack-sdk-latest.tar.gz
    tar axvf addon-sdk-1.17.tar.gz
    cd addon-sdk-1.17
    . bin/activate
    cd /tmp/enjoyreading-ng/src
    cfx xpi

You can then install the extension by calling Firefox/Iceweasel with
something as simple as:

    firefox enjoyreading-ng.xpi

# Original comments from Remigiusz Modrzejewski

## User review

The only one that got through before AMO took down the add-on:

> I've had bad eyes my whole life and reading various sites can be tricky
> for me. I think I've tried every other spawn-of-Readability addon
> available, but this one is the absolute best. Thank you so much for
> keeping it alive! It is something I use easily a dozen times every day and
> it improves the quality of my online life more than I can even express
> with words.

## Note

This is not in AMO for *good* reasons.
Seems that it is impossible right now to submit readability-based add-on.
The reply is broken down in the issues page.
**None of the problems have been introduced in this fork**.
