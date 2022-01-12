# Syphilis Record Search and Review Algorithm

**General disclaimer** This repository was created for use by CDC programs to collaborate on public health related projects in support of the [CDC mission](https://www.cdc.gov/about/organization/mission.htm).  GitHub is not hosted by the CDC, but is a third party website used by CDC and its partners to share information and collaborate on software. CDC use of GitHub does not imply an endorsement of any one particular service, product, or enterprise. 

## Overview

While health departments began conducting syphilis surveillance in the 1930s (consistently compiled national data are available dating back to 1941), , laboratories haven been madated to report serologies to health departments since 1962 in an effort to identify syphilis cases that might not be otherwise reported by clinicians. Historical test results are routinely maintained on file to aid with interpretation of any subsequent tests. Health departments subsequently investigate reported serologies to determine if they represent a new infection, reinfection, or treatment failure. Ideally, every new reactive serology should be investigated but because of the overwhelming volume serologies reported and limited resources avaibale at health departments, health departments do not investigate all reported serologies. Reported serologies were administratively closed, using "reactor grids" (examples of reactor grids in the figure below) which prioritize serologies for further investigation based on patient's age, sex, test type, and test titer.
![reactor_grid](https://github.com/CDCgov/Syphilis_Record_Search_and_Review_Algorithm/blob/master/ReactorGridExample.png)

Reactor grids, however, are widely acknowledge to be unreliable and have shown to miss syphilis cases. Recently, researchers have suggested an algorithm that used in conjuntion with electronic laboratory reporting might be used to automatically search historical records and apply the case definition of syphilis. We developed a computerized algorithm (demonstrated in the figure below) that could be used by any public health agency to compare reported electronic laboratory reports with prior testing and intervention history in the surveillance database of the public health agency. [This algorithm was developed using a surveillance dataset from Florida Department of Health and validated by New York City Department of Health and Mental Hygiene](https://journals.lww.com/stdjournal/Citation/2022/01000/Automating_Case_Reporting_of_Chlamydia_and.8.aspx) (click hyperlink to access the manuscript describing the algorithm). The goal of the algorithm is to accurately close those serologies that do not meet the case definition, and prioritize the rest for further investigation; and do so using evidence-based decisions and advances in technology and data management capabilities of public health agencies. The algorithm demonstrated an accuracy of 99.4% and would have saved an additional 590 workdays in the 3 years of surveillance data analyzed.
![algorithm image](https://github.com/CDCgov/Syphilis_Record_Search_and_Review_Algorithm/blob/master/algorithm_manuscript_revised.png)

The goal of this GitHub repository is to serve as the one-stop location for public health agencies and technology vendors to test and implement this algorithm. Please contact Saugat Karki (SKarki@cdc.gov) for further discussion and any technical assistance from the Centers for Disease Control and Prevention. 
## Dependencies

The required Python 3 dependencies necessary for this jupyter notebook include the following:

* Pandas
* Numpy
* Datetime

The rest of the dependencies come installed with Python 3. Feel free to download & install [Anaconda](https://www.anaconda.com/) and run Jupyter Notebook from there.

## Getting Started

### Cloning the Repository

The repository can either be downloaded from GitHub or cloned using the following command:

`$ git clone https://github.com/CDCgov/Syphilis_Record_Search_and_Review_Algorithm.git`

### Running the Notebook

Launch Jupyter Notebook in Anaconda or a Python 3 installation of your choice. Follow the steps closely as there are some steps required for you to ensure the data meets the correct format. See the notebook for specific details.

## Related documents

* [Open Practices](open_practices.md)
* [Rules of Behavior](rules_of_behavior.md)
* [Thanks and Acknowledgements](thanks.md)
* [Disclaimer](DISCLAIMER.md)
* [Contribution Notice](CONTRIBUTING.md)
* [Code of Conduct](code-of-conduct.md)

## Public Domain Standard Notice
This repository constitutes a work of the United States Government and is not
subject to domestic copyright protection under 17 USC § 105. This repository is in
the public domain within the United States, and copyright and related rights in
the work worldwide are waived through the [CC0 1.0 Universal public domain dedication](https://creativecommons.org/publicdomain/zero/1.0/).
All contributions to this repository will be released under the CC0 dedication. By
submitting a pull request you are agreeing to comply with this waiver of
copyright interest.

## License Standard Notice
The repository utilizes code licensed under the terms of the Apache Software
License and therefore is licensed under ASL v2 or later.

This source code in this repository is free: you can redistribute it and/or modify it under
the terms of the Apache Software License version 2, or (at your option) any
later version.

This source code in this repository is distributed in the hope that it will be useful, but WITHOUT ANY
WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
PARTICULAR PURPOSE. See the Apache Software License for more details.

You should have received a copy of the Apache Software License along with this
program. If not, see http://www.apache.org/licenses/LICENSE-2.0.html

The source code forked from other open source projects will inherit its license.

## Privacy Standard Notice
This repository contains only non-sensitive, publicly available data and
information. All material and community participation is covered by the
[Disclaimer](https://github.com/CDCgov/template/blob/master/DISCLAIMER.md)
and [Code of Conduct](https://github.com/CDCgov/template/blob/master/code-of-conduct.md).
For more information about CDC's privacy policy, please visit [http://www.cdc.gov/other/privacy.html](https://www.cdc.gov/other/privacy.html).

## Contributing Standard Notice
This repository is the final version and as such any forks/pull requests will not be accepted.

All comments, messages, pull requests, and other submissions received through
CDC including this GitHub page may be subject to applicable federal law, including but not limited to the Federal Records Act, and may be archived. Learn more at [http://www.cdc.gov/other/privacy.html](http://www.cdc.gov/other/privacy.html).

## Records Management Standard Notice
This repository is not a source of government records, but is a copy to increase
collaboration and collaborative potential. All government records will be
published through the [CDC web site](http://www.cdc.gov).

## Additional Standard Notices
Please refer to [CDC's Template Repository](https://github.com/CDCgov/template)
for more information about [contributing to this repository](https://github.com/CDCgov/template/blob/master/CONTRIBUTING.md),
[public domain notices and disclaimers](https://github.com/CDCgov/template/blob/master/DISCLAIMER.md),
and [code of conduct](https://github.com/CDCgov/template/blob/master/code-of-conduct.md).
