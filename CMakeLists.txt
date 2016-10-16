# Copyright (C) 2016 LuaDist.
# Created by Peter Kapec
# Redistribution and use of this file is allowed according to the terms of the MIT license.
# For details see the COPYRIGHT file distributed with LuaDist.
# Please note that the package source code is licensed under its own license.

project ( lua-term C )
cmake_minimum_required ( VERSION 2.8 )
include ( cmake/dist.cmake )
include ( lua )

install_lua_module ( term         term/init.lua )
install_lua_module ( term.colors  term/colors.lua )
install_lua_module ( term.cursor  term/cursor.lua )
install_lua_module ( term.core    core.c )


install_doc ( COPYING README.md CHANGES )