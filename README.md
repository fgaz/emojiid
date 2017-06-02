# EmojiId

Deterministically assign an emoji to a user/machine pair.

**Stop wasting that space on $PS1!**

![screenshot](screenshot.png)

## Usage

You can use it for example in your bashrc to change your prompt
like this

```bash
emojiid="$(source ~/path/to/emojiid.sh)"
PS1="\u@${emojiid} \W \$ "
```

or even

```bash
PS1="${emojiid} \W \$ "
```

(I didn't put the emojiid.sh evaluation inside PS1
because PS1 is executed at every line, and that would
be inefficient (md5, conversion, modulus...))

## Configuration

You can change the randomnessource and emojisample variables

## Terminal emulator support

Some terminal emulators fail to display the emoji in its full width
(usually between 1 and 2 characters), sometimes causing weird
behaviour, such as characters disappearing and misaligning or
the emoji being cut off.

Let me know if you test it on a termina emulator
that is not listed here!

<!-- TODO check how to display a table -->

* sakura: issues with alignment
* lxterminal: works

