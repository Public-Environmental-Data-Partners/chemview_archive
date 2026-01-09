# chemview_archive

This repo holds scripts used to download [U.S. EPA ChemView](https://chemview.epa.gov/chemview/) data files
and some supporting utilities. The data itself, which is huge, should never be stored in this repository. 

# What the heck is going on here -- where's the code?

See the `gen1` folder for rough-and-ready Python code that was written in November and December
of 2025. This code was used to successfully download about 380 GB of ChemView HTML, PDF, and XML
files for:
* Section 5 Consent Orders
* Substantial Risk Reports
* New Chemical Notices
* Premanufacture Notices
* Significant New Use Reports

However, IMO, the code isn't ready for prime time and doesn't belong, yet, in the 
traditional `src` folder. The technology I used for finding/downloading the data files
evolved radically from the first data set (Section 5) which used very bad 
Playwright code through better Playwright code to the code for New Chemical Notices
which bypasses Playwright scripting altogether in favor of a more analytical 
and MUCH faster technique outlined by Michael Cohen. If this code is to be 
re-used, all the code should be standardized to use that final technique.

I'm also not sure about how the output files should be organized. That
might need to change considerably once users start looking for data they need.

***
Below this point, this readme has not yet been customized for this repo.
***

# How to start contributing to this repo
* Instructions go here
* Developer setup (if relevant)
* Communication channels (if relevant)

**Suggestions for additional components of Readmes:**
* A "How to use" section if the repo's project is a tool or website
* A link to the [good-first-issue](https://github.com/issues?q=is%3Aopen+is%3Aissue+label%3Agood-first-issue+user%3APublic-Environmental-Data-Partners) label (this link across PEDP, or a specific link for the repo)
* Highlight "ready" label on issues to mean "this is an issue that is ready to work on and needs an owner"
* Additional badges at the top, such as code quality indicators


**When using this template, please look through all of the files to ensure they apply to the new repo.**

---

## License & Copyright

Copyright (C) <year> Public Environmental Data Partners (PEDP)
This program is free software: you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation, version 3.0.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.

See the [`LICENSE`](/LICENSE) file for details.
