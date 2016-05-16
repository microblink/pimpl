## Pimpling in Cpp

Proving pimpls do not _require_ heap, exceptions or runtime polymorphism.

IOW showing why ["Attempt #3"](http://www.gotw.ca/gotw/028.htm) (_as an idea_) is _not_ deplorable, rather what is deplorable is giving up on efficiency just becuase the language does not _yet_ OOB cover all the edge cases or rough edges: of all the points raised all but one has been solved by cpp practice and language developments (aligned storage, static assertions, CRTP and policy based design, perfect forwarding, delegating and inheriting constructors and explicitly deleted member functions).

The one remaining issue is manual updating of the storage and alignment requirements: and this could easily be solved once modules get into the language, i.e. if they 'get them right' (and add a standardized option of 'exporting' just the sizeof and alignof information of classes).



#### Related/similar developments, contributions and discussions
* https://github.com/akrzemi1/boost.pimpl
* https://github.com/sean-/boost-pimpl
* https://github.com/yet-another-user/pimpl
* http://loki-lib.cvs.sourceforge.net/viewvc/loki-lib/loki/include/loki/Pimpl.h?view=markup
* http://lists.boost.org/Archives/boost/2005/10/95366.php
* http://lists.boost.org/Archives/boost/2006/05/104757.php
* http://lists.boost.org/Archives/boost/2007/10/128740.php
* http://www.drdobbs.com/cpp/making-pimpl-easy/205918714
* http://www.boost.org/doc/libs/release/libs/smart_ptr/sp_techniques.html#pimpl
* http://www.cppsamples.com/common-tasks/pimpl.html
* http://www.gotw.ca/gotw/028.htm The Fast Pimpl Idiom
* http://www.gotw.ca/publications/mill05.htm The Joy of Pimpls (or, More About the Compiler-Firewall Idiom)
* https://herbsutter.com/gotw/_100 "Compilation Firewalls (C++11 version)"
* https://herbsutter.com/gotw/_101 "Compilation Firewalls, Part 2"
* http://www.gotw.ca/publications/mill04.htm "Pimpls - Beauty Marks You Can Depend On"


##### C++ In-The-Kernel Now!
##### Copyright © 2016. Domagoj Saric. All rights reserved.
