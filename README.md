<p><b>What is JPI</b><br>
JPI is a software storage pool for combining existing disk that use ext3 or ext4 to be combined storage. This is done by creating links to hashed files from their 'pool' path to their store path.<br>
It is written in php5-cli which is its, only dependency. JPI will work on all nix based systems with php5-cli installed.
</p>


<p><b>Installation</b><br>
Clone JPI from git<br>
Move 'jpi' to /usr/bin/ and chmod for execute<br>
Start jpi as admin.<pre># sudo jpi</pre> The setup will ask for the 'pool' path and first 'storePath'<br>
<br>
Pool path and all storePaths must be on separate drives.

</p>
<p><b>Usage</b>

<pre>
jpi -daemon         Start JPI as daemon
jpi -stop           Stop JPI
jpi -restart        Restart JPI as daemon<br>
jpi -add-store-path [/path/to/new/store]    Adds store path to JPI (please back up /etc/jpi/config.json)
jpi -find-missing   attemps to locate missing source files
</pre>
</p>
