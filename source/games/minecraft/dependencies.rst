Minecraft Dependencies
======================

.. note::

	This only applies if not using v2.6 or higher. Those versions will download Java as part of the server installation.

Minecraft requires additional dependencies that are not managed by PufferPanel, failing to install these may result in errors like:

.. code-block:: bash


	[DAEMON] Allocating server
	[DAEMON] Server allocated
	[DAEMON] Ready to be installed
	[DAEMON] Installing server
	[DAEMON] Version 1.16.5 json located, downloading from https://launchermeta.mojang.com/v1/packages/436877ffaef948954053e1a78a366b8b7c204a91/1.16.5.json
	[DAEMON] Version jar located, downloading from https://launcher.mojang.com/v1/objects/1b557e7b033b583cd9f66746b7a9ab1ec1673ced/server.jar
	[DAEMON] Downloading: https://launcher.mojang.com/v1/objects/1b557e7b033b583cd9f66746b7a9ab1ec1673ced/server.jar
	[DAEMON] Writing some data to file: server.properties
	[DAEMON] Writing some data to file: eula.txt
	[DAEMON] Server installed
	[DAEMON] Starting server
	[DAEMON] Failed to start server
	[DAEMON] exec: "java": executable file not found in $PATH
	[DAEMON] Starting server
 
To resolve this please install JDK/JRE required for your Minecraft version.

You can see what version of Java you have installed by running `java -version`.


Multiple Java Versions
^^^^^^^^^^^^^^^^^^^^^^

If you want to run multiple Minecraft servers that require different Java versions you can just install all needed Java versions on your system and use the ``path to java executable`` field available on most Minecraft templates to specify which Java version that server should use

On most systems installed Java versions are found in ``/usr/lib/jvm`` and the executable for a specific version is usually located in its installation directory as ``bin/java``, so if you're using OpenJDK 11 and OpenJDK 16 the executables may for example be found at ``/usr/lib/jvm/openjdk-11-amd64/bin/java`` and ``/usr/lib/jvm/openjdk-16-amd64/bin/java`` respectively
