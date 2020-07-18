Basic JavaScript Game using a text-based grid.

Just something I threw together to see if I remember my game programming skills from the 90s.

There are multiple versions. Each version adds more features. index.html is always the latest version (it's version is (X+1) where X is from latest versionX.html).

Version 1 has a basic grid to constain movement, version 2 adds colors, version 3 adds actual game logic (locks and doors), version 4 adds mouse (therefore also mobile) support and "food" (which depletes on each move), making it a logic puzzle. Each version also probably add more things I forgot about too.

You can view the latest version at [http://dbgame01.azurewebsites.net/](http://dbgame01.azurewebsites.net/).

    [
        "**k*f***************",
        "*& #^[#            *",
        "*  # d#     ##### d*",
        "*  #        #   ] d*",
        "*  ###]######   ###*",
        "*  d[#]#[[dd       *",
        "*  ###]#########   *",
        "*         #       d*",
        "*        d        [*",
        "******** ***********",
        "*   #            d *",
        "* # #       #####  *",
        "* # ]      d#     [*",
        "* # #########   ###*",
        "*0# #             d*",
        "*## #[dd#######]###*",
        "*   #####^#[ d#   d*",
        "*   d ^]    #     [*",
        "********************"
    ]

# Run server

    docker run --name jsgame --rm -dt -p 80:80 -v `pwd`:/usr/share/nginx/html nginx:1.19.1
