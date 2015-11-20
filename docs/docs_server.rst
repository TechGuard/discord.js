.. include:: ./vars.rst

Server
======

**extends** Equality_

Stores information about a Discord Server.

Attributes
----------

client
~~~~~~

The Client_ that cached the Server.

region
~~~~~~

`String`, region of the server.

name
~~~~

`String`, name of the server.

id
~~

`String`, ID of the server - never changes.

members
~~~~~~~

Members of the server, a Cache_ of User_ objects.

channels
~~~~~~~~

Channels in the server, a Cache_ of ServerChannel_ objects.

roles
~~~~~

Roles of the server, a Cache_ of Role_ objects.

icon
~~~~

ID/Hash of server icon, use ``server.iconURL`` for an URL to the icon.

afkTimeout
~~~~~~~~~~

`Number`, the AFK timeout in seconds before a user is classed as AFK. If there isn't an AFK timeout, this will be null.

afkChannel
~~~~~~~~~~

The channel where AFK users are moved to, ServerChannel_ object. If one isn't set, this will be null.

defaultChannel
~~~~~~~~~~~~~~

The ``#general`` ServerChannel_ of the server.

owner
~~~~~

The founder of the server, a User_ object.

iconURL
~~~~~~~

The URL of the Server's icon. If the server doesn't have an icon, this will be null.

Functions
---------

rolesOfUser(user)
~~~~~~~~~~~~~~~~~

**Aliases**: `rolesOf`

Returns an array of the roles affecting a user server-wide.