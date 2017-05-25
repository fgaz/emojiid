# EmojiId

Deterministically assign an emoji to a user/machine pair.

**Stop wasting that space on $PS1!**

## Usage

You can use it for example in your bashrc to change your prompt
like this

    export PS1="\u@$(source ~/path/to/emojiid.sh) \W \$ "

or even

    export PS1="$(source ~/path/to/emojiid.sh) \W \$ " 

## Configuration

You can change the randomnessource and emojisample variables

