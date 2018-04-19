---
date: 2018-04-19T05:41:38Z
title: "jx create token addon"
slug: jx_create_token_addon
url: /commands/jx_create_token_addon/
---
## jx create token addon

Adds a new token/login for a user for a given addon

### Synopsis

Creates a new User Token for an Addon service

```
jx create token addon [username] [flags]
```

### Examples

```
  # Add a new User Token for an addonservice
  jx create token addon -n anchore someUserName
  
  # As above with the password being passed in
  jx create token addon -n anchore -p somePassword someUserName
```

### Options

```
  -t, --api-token string   The API Token for the user
  -b, --batch-mode         In batch mode the command never prompts for user input
      --headless           Enable headless operation if using browser automation
  -h, --help               help for addon
  -k, --kind string        The kind of addon. Defaults to the addon name if not specified
  -n, --name string        The name of the git server to add a user
      --no-brew            Disables the use of brew on MacOS to install or upgrade command line dependencies
      --timeout string     The timeout if using browser automation to generate the API token (by passing username and password)
  -u, --url string         The URL of the git server to add a user
      --verbose            Enable verbose logging
```

### SEE ALSO

* [jx create token](/commands/jx_create_token/)	 - Creates a new user token for a service

###### Auto generated by spf13/cobra on 19-Apr-2018