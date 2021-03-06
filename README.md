# Contentful Locale Publisher

## warning! this is a work in progress and not currently confirmed to be working properly

[Contentful](https://www.contentful.com) is a content management platform for web applications, mobile apps and connected devices. It allows you to create, edit & manage content in the cloud and publish it anywhere via powerful API. Contentful offers tools for managing editorial teams and enabling cooperation between organizations.

This extension provides a widget which lives in the sidebar of the Contentful webapp and provides a way to select which locales of the current entry to publish. The unselected locales are published with either the previously published value or empty values. After publishing the values of the unselected locales are restored to their previous values.

<img width="333" alt="screenshot" src="https://user-images.githubusercontent.com/6521666/40333977-1326f416-5d10-11e8-83ce-3ee8bd47ec18.png">

## How to use

### Using the Webapp

1. Copy this link:

```
https://github.com/cachrisman/locale_publishing_extension/blob/master/extension.json
```

2. Go to the [Contentful webapp](https://app.contentful.com/deeplink?link=extensions)'s extension settings page
3. Click the add blue "Add extension" button
4. Select "Install from GitHub"
5. Paste in the link from above and click install.

### Or using command line tools

1. install the [contentful-cli](https://github.com/contentful/contentful-cli) tool
2. open a terminal and run `git clone https://github.com/cachrisman/locale_publishing_extension.git; cd locale_publishing_extension`
2. run `contentful login`
3. run `contentful extension update --space-id YOUR_SPACE_ID --force`

### Last, add the sidebar extension to be shown for the desired content types

Refer to [this documentation page](https://www.contentful.com/developers/docs/extensibility/custom-sidebar/) on using a custom sidebar for details on how to do this.
