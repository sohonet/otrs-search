Command Line search for OTRS 2.3.4
==================================

DEPENDENCIES
------------
- Python 2.6/2.7 (not compatible with Python 3)
- apt-get install python-pyme #http://pyme.sourceforge.net/

INSTALLATION
------------
- You must have a GPG key to create the password file: gpg --gen-key
- Create config and password files with: python otrs_create_config.py

FEATURES
--------
- Full text search
- Search by: id, client
- Time units and amount support (year, month, ...)
- URL shortener using goog.gl (with token support)
- GPG encrypted password file
- Authenticate once until reboot (uses session cookie)

TODO
----
- Search by: queue name, state
- Use filename in header to save CSV file
- More stuff in configuration file

CHANGELOG
---------
- 08.11.11 JBA Creation du script, recherche basique
- 09.11.11 JBA Gestion des sessions 
- 16.11.11 JBA Search by Ticket ID or client email 
- 18.11.11 JBA Config is in a separate file, ready for publishing
- 22.11.11 JBA No google url shortener links option, missing translation
- 12.11.11 JBA Faster: do not check session with http but relying on session file.

LICENSE
-------
    
    Copyright (C) 2011 Jean-Baptiste Aubort <jean-baptiste.aubort@epfl.ch>

    This program is free software; you can redistribute it and/or modify it
    under the terms of the GNU General Public License as published by the
    Free Software Foundation; either version 3 of the License, or any later
    version. This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General
    Public License for more details. You should have received a copy of the
    GNU General Public License along with this program; if not, write to the
    Free Software Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA

See gpl-3.0.txt