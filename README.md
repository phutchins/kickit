kickit
======

Configures the kickit ruby script that runs as a daemon and listens for an http connection on port 5425 (KICK).

Files
-----

- kickit.rb - Tiny http server script that runs as a daemon
- kickit.conf.upstart - Ubuntu upstart script
- kickit.plist - OSX Launchd config file

Usage
----

Add a depends for the kickit cookbook in your metadata.rb
``` ruby
depends 'kickit'
```

Include the kickit cookbook somewhere that makes sense
``` ruby
include_recipe 'kickit'
```

Platform Support
----------------

Current tested on...
- Ubuntu - 12.04, 13.04
- OSX - Mavericks
