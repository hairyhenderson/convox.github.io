---
title: "Environment Variables"
---
You can configure secrets and links to external resources on your application using environment variables.

```shell
$ convox env
DATABASE_URL=postgres://example.org/db
TWITTER_OAUTH_SECRET=a0b1c2d3

$ convox env set FOO=bar

$ convox env
DATABASE_URL=postgres://example.org/db
FOO=bar
TWITTER_OAUTH_SECRET=a0b1c2d3
```


These environment variables will be available to your running application.

<div class="block-callout block-show-callout type-info">
### Changing Environment Variables
After making any change to your environment variables you will need to redeploy your application using `convox deploy`
</div>