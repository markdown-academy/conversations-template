# Markdown Academy Conversation Format

Hi :wave: It looks you like our conversations, and you would like to create one yourself, right?

[:no_good: Not really](#what-a-shame) [:+1: Sure!](#title)


## What a Shame
What a shame! But it's your choice to make this bot sad :crying_cat_face:

[> Quit](_quit)

## Title
So every conversation starts with the title and title is represented with a headline at the beginning of the conversation document such as in the following example

```
# My Awesome Conversation
```

This the name of the conversation you can see when you want to select the conversation from Markdown Academy's home tab.

![Conversation Selection](https://raw.githubusercontent.com/markdown-academy/conversations-template/main/images/select-conversation.png)

Just be careful, the title must be unique within a single repository. Otherwise, only one of the conversations with the same name will be loaded without any predictable behaviour which one.

[:heart_eyes_cat: Cool! What's next?](#conversation-parts)

## Conversation Parts

Each of the conversation parts is represented by a Markdown paragraph. Typically, the bot will pause for predefined time after each part to give the reader time to read the part.

```markdown
This is a paragraph.
```

Can you see it?

I was waiting a bit before this another paragraph.

How familiar are you with the Markdown format?

[:sunglasses: I'm a pro!](#quick-explanation-of-supported-markdown-features) [:thinking_face: I know some basics](#quick-explanation-of-supported-markdown-features) [:no_mouth: I have no idea](#markdown-explanation)

## Markdown Explanation

[Markdown](https://www.markdownguide.org) is a text format which uses special characters to format the text. For example, you can use `*` to make the text italic, `**` to make it bold, or `#` to make it a headline.

## Quick Explanation of Supported Markdown Features

The following formatting options are supported within the conversation parts:

- *Italic Text*: Wrap the text with asterisks (`*`) to display it in italic format.
- **Bold Text**: Wrap the text with double asterisks (`**`) to display it in bold format.
- `Code Style`: Wrap the text with backticks (&#x0060;) to display it as code style.
- Block Code: Use three backticks (&#x0060;&#x0060;&#x0060;) to enclose a block of code. The code block can span multiple lines.
- Quotes: Use a greater-than sign (`>`) at the beginning of a line to create a blockquote.
- Ordered Lists: Use numbers followed by a period (`1.`, `2.`, etc.) to create an ordered list.
- Bullet Lists: Use asterisks (`*`) or hyphens (`-`) to create bullet lists.
- Images: Use the Markdown image syntax (`![alt text](image URL)`) to display an image with an external reference.
- External Links: Use the Markdown link syntax (`[link text](URL)`) to create an external link.

[:white_check_mark: Got it!](#anchors)

## Anchors

What makes Markdown Academy conversations fun is that they are not linear. You can jump to any part of the conversation from any other part. This is done by using anchors. Anchors are defined by using the following _H2_ syntax:

```markdown
## This is an anchor

This is the paragraph which can be referenced by the anchor.
```

So how do you actually use the anchor?

It's simple. You just need to use the following syntax:

```markdown
[:anchor: Jump to the anchor](#this-is-an-anchor)
```

[:anchor: Jump to the anchor](#this-is-an-anchor)

## This is an anchor

You need to remember how are the anchors created in Markdown - they start with the hash sign `#` and then they are followed by the anchor name in lower case and with dashes instead of spaces.

Don't worry, any modern IDE will help you with that.

[:hash: Copy that!](#non-interactive-jumps)

## Non-Interactive Jumps

Sometimes you want to jump to a specific part of the conversation without any user interaction. This is useful when your conversation hs many paths, and you want to skip some of the following paragraphs.

You can do that by using the following syntax:

```markdown
[> Jump to the anchor](#this-is-an-anchor)
```

This will take you directly to the anchor without any user interaction.

Are you bored already? Maybe you want to quit the conversation?

[> :bored: Yes, please!](#not-so-fast) [> :smiley: No, I'm having fun!](#quitting-the-conversation)

## Not so fast

Not so fast, there is something you should learn first.

[:sunglasses: What is it?](#quitting-the-conversation)

## Quitting the Conversation

When you want to let the user quit the conversation, you can use the special anchor `_quit`:

```markdown
[:wave: Quit](_quit)
```

And a one last thing...

I got you covered. When you use the [Conversations Repository Template](https://github.com/markdown-academy/conversations-template) then your conversations are validated for every Pull Request and you will be notified if you use an anchor which does not exist.

So what are you waiting for? Go and create your first conversation!

[:rocket: Let's do it!](_quit)