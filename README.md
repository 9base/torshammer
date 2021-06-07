> [!NOTE]
> **9base status: Historical Downstream.** Lifecycle: archived; not actively maintained by 9base.
>
> This is an upstream-derived Tor's Hammer source repository with meaningful historical local adaptation. It is not an untouched reference import or an original 9base tool.
>
> **Provenance:** the original project is [Tor's Hammer on SourceForge](https://sourceforge.net/projects/torshammer). Retained 2012 solarstone/allura commits carry the original SourceForge SVN provenance (`https://svn.code.sf.net/p/torshammer/code/trunk`). The GitHub repository is a standalone import, so there is no GitHub parent from which to quantify current upstream divergence.
>
> **Historical local work:** nine commits attributed to Zaryob/Suleyman Poyraz from 4–7 June 2021 include one merge, documentation/license-file additions, and changes to `torshammer.py`, `socks.py` and `terminal.py`. The patches evidence [Python 3 adaptation](https://github.com/9base/torshammer/commit/4af8e706a377244074e0813ca3294867544d857e), string/indentation changes and [connection handling changes](https://github.com/9base/torshammer/commit/e30fd1a6877fd72ff73de0d046044af14ab20fda). These changes establish historical downstream work; they have not been executed or revalidated during archival curation. The original source and its contributors remain credited separately.
>
> **Preservation:** retained as a historical source record; no larger 9base project family was established. The existing `LICENSE.md` was added locally in 2021, while `socks.py` retains a separate Dan-Haim notice. This documentation does not normalize those notices or determine a new project-wide license. The original README follows unchanged.
>
> Archival context reconstructed on 8 October 2026 from commit patches, source headers and the existing README. The 2021 dates describe verified local work, not the repository's unverified archive date.

---

<!-- Original README follows unchanged. -->

INFO

Version: 1.0 Beta
Home page: http://torshammer.sourceforge.net
Project page: https://sourceforge.net/projects/torshammer

Tor's Hammer is a slow post dos testing tool written in Python. It can also be run through the Tor network to be anonymized. If you are going to run it with Tor it assumes you are running Tor on 127.0.0.1:9050. Kills most unprotected web servers running Apache and IIS via a single instance. Kills Apache 1.X and older IIS with ~128 threads, newer IIS and Apache 2.X with ~256 threads.

---------------------------------------------------------------------------

REQUIREMENTS:

This tool is cross-platform because is written in Python. You only need to have python installed on your operating system.

Python page: http://www.python.org
Download page: http://www.python.org/download

---------------------------------------------------------------------------

USAGE:

./torshammer.py -t <target> [-r <threads> -p <port> -T -h]
-t|--target <Hostname|IP>
-r|--threads <Number of threads> Defaults to 256
-p|--port <Web Server Port> Defaults to 80
-T|--tor Enable anonymising through tor on 127.0.0.1:9050
-h|--help Shows this help

Eg. ./torshammer.py -t 192.168.1.100 -r 256

---------------------------------------------------------------------------