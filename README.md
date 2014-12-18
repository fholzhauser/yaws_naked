yaws_naked
==========

yaws 1.98 stripped down to Erlang only

The reason for this is to provide a more portable version primarily for 
embedding purposes.

Compared to the original code, it is obviously limited in functionality and 
performance.

All credits are to the contributors of the original yaws project.
Original license file included.

Changes
-------
- Moved ssl directory to priv (seems to contain handy scripts for certificates)
- Removed all directories and files except: src, include, priv, ebin
- Built original yaws source tree and copied yaws_configure.hrl from there 
    with sendfile disabled
- Fixed yaws_stats.erl to take "yaws.hrl" from include dir (where it really is).
    Original yaws build works with this bug workaround 
