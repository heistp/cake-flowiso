# cake-flowiso

This script runs tests of all of Cake's flow isolation parameters (flowblind,
hosts, srchost, dsthost, flows, dual-srchost, dual-dsthost, and triple-isolate).

Simply run it without arguments as root. Trust me! :)

srchost/dsthost stopped working due to a bug introduced in kernel 5.8 in
[this commit](https://github.com/torvalds/linux/commit/b0c19ed6088ab41dd2a727b60594b7297c15d6ce),
so this demonstrates that bug, and confirms that the patch that was made for it
works. In the future, we can re-run this test any time changes are made that may
affect Cake's flow isolation.
