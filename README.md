# Markdown Academy Conversations

Welcome to the Markdown Academy Conversations repository! This repository is a collection of Markdown documents that describe conversations using the Markdown Academy Conversation Format. It provides a structured way to represent conversations with various formatting options. Feel free to contribute by adding more conversations to this repository. The conversations are stored in the [conversations folder](conversations) of the repository.

## Markdown Academy Conversation Format

The Markdown Academy Conversation Format is a specific format for Markdown documents that describe conversations. It allows you to structure and represent conversations with various formatting options. The format is designed to be human-readable and can include elements like italic text, bold text, code blocks, quotes, lists, images, links, and more.

### Formatting Options

The following formatting options are supported within the conversation parts:

- *Italic Text*: Wrap the text with asterisks (`*`) to display it in italic format.
- **Bold Text**: Wrap the text with double asterisks (`**`) to display it in bold format.
- `Code Style`: Wrap the text with backticks (`\``) to display it as code style.
- Block Code: Use three backticks (```) to enclose a block of code. The code block can span multiple lines.
- Quotes: Use a greater-than sign (`>`) at the beginning of a line to create a blockquote.
- Ordered Lists: Use numbers followed by a period (`1.`, `2.`, etc.) to create an ordered list.
- Bullet Lists: Use asterisks (`*`) or hyphens (`-`) to create bullet lists.
- Images: Use the Markdown image syntax (`![alt text](image URL)`) to display an image with an external reference.
- External Links: Use the Markdown link syntax (`[link text](URL)`) to create an external link.

### Emoticons

Emoticons can be used within conversation parts, following the Slack/GitHub format, such as `:up:`, `:ok:`, `:cry:`, etc. These will be displayed as the corresponding emoticons in the conversation.

## Document Structure

A Markdown Academy conversation document follows a specific structure. It consists of multiple conversation parts, where each part is represented by a Markdown paragraph. Each conversation part can have an explicit anchor generated from the H2 headline (`## Headline`) preceding the conversation text paragraph. Each conversation part can have associated decisions represented by a group of internal links in a Markdown paragraph immediately following the conversation text paragraph.

```
## Paragraph with Decisions
This part provides decistions

[:ok: Option One](#option-one) [:cry: Option Two](#option-two) [:wave: Quit](_quit)

```

The link can use `_quit` or any link title starting with `!` to exit the conversation completely.

Normally, the conversation follows the original document. However, if you want to navigate the reader to another part of the conversation without user interaction, you can add internal links whose titles start with the `>` sign.


```
## Option One

Option one selected

[> The End](#the-end)

## Option Two

Option two selected

[> The End](#the-end)

## The End

This is the last conversation

```

## Testing Conversation

You can start a conversation by running the following command:

```bash
./start_conversation.sh conversations/markdown_academy.md
``` 

This will walk you through the conversation in a terminal. Of course, things like formatting or images won't work, but you can verify the flow of the conversation.

## Example Conversation

The following is an example conversation document:

```markdown
# Test Conversation

## Introduction
This is the very first sentence. *Something italic*. **Something bold**. `Some Code`.

This is an anonymous block

```
This is a code block
```

> This is a quote

Another anonymous block

Ordered list:

1. one
2. two
3. three

Bullet list

* bullet
* point
* list

The image follows

![Tux, the Linux mascot](https://d33wubrfki0l68.cloudfront.net/e7ed9fe4bafe46e275c807d63591f85f9ab246ba/e2d28/assets/images/tux.png)

Normal link follows

[Normal Link](https://www.example.com)

This paragraph has buttons

[:ok: Option One](#option-one) [:cry: Option Two](#option-two) [:wave: Quit](_quit)

## Option One

Option one selected

[> The End](#the-end)

## Option Two

Option two selected

[> The End](#the-end)

## The End

This is the last conversation
```