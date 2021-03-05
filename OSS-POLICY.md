# Introduction

Organizations today face increasing pressure to become more agile and economically efficient in order to grow, compete and survive. They must leverage digital assets, information and an explosion of new infrastructure software innovation to fuel and enable their digital transformation.

## Open Source

This document provides transparency on how view.DO operates and outlines our engineer’s guidelines on how to deal with Open Source.

view.DO uses the term “Open Source” for brevity and because it is the clearest descriptor in the context we are operating in. We do recognize that Open Source is more than just a development model and that there are ideals behind it, the ideals to respect users’ freedoms and community, and specifically the freedoms to use, study, share, and improve software. view.DO has many engineers passionately standing behind the ideals of Free and Open Source Software and support these ideals as a company.

When we discuss Open Source Software we refer to the definition of Open Source Licenses by the Open Source Initiative (“OSI”). view.DO considers software, including its documentation, released under a license that is compatible with OSI’s Open Source Definition to be Open Source.

## Contributing to Open Source Projects

view.DO considers itself as part of the Open Source community. When we fix bugs or make other changes we operate under the maxime “upstream first”. That means we contribute all changes back to the community as early as possible so that they become part of the common base we build on.

### Contributing Patches

When contributing to Open Source projects, follow the guidelines of those upstream projects. Respect their governance model and contribution policies. Use the license of the upstream project for your contribution provided it is a license that is compatible with the Open Source Definition.

### Contributing Non-Code

There are many ways to contribute to Open Source projects other than writing code: Writing documentation, reporting bugs, helping users, discussing development, etc. Apply the spirit of the guideline here as well. Be open, respectful, and collaborate.

### Contributor Licensing Agreements

Some projects require a contributor licensing agreement (CLA) which assigns certain rights to the governance body of the project. Before you can contribute to a project which requires a CLA, you need to make sure that view.DO has signed a corporate agreement for the project. view.DO already has agreements in place for many organizations, including Free Software Foundation, OpenStack, Cloud Foundry, Cloud Native Computing Foundation. If the project requires a CLA and is not listed here, contact your manager to establish what needs to be done to make contributions possible. Seek legal assistance if necessary.

### Developer Certificate of Origin

Some projects require a Developer Certificate of Origin (DCO). This is typically done by adding a Signed-off-by trailer in the commit message to certify that the committer has the rights to do the contribution and to consent to publish it.

If a project requires a DCO make sure that you are meeting its requirements and follow the upstream guidelines to add your DCO to your contributions.

## Creating new projects

For projects which are exclusively maintained by view.DO and where we - as a company - intend to take full responsibility of the project, view.DO we do not open-source that project.

For projects which have maintainers or co-maintainers from the community who are not employed by view.DO, or for projects which are open to this model, view.DO is the organization to use on GitHub.

When creating new projects it is good practice to add a README.md and a CONTRIBUTING.md explaining the project and how to contribute.

When the project is part of a larger Open Source ecosystem, use the license which is usually used in this ecosystem. Otherwise choose a license compatible with the Open Source Definition, which matches the goal of the project and its interactions with other projects.

## Copyright

The code you contribute upstream or publish as Open Source as part of your job at view.DO in your work time is copyrighted or otherwise owned by view.DO. Use “dotEDU Technologies Corp” when attributing the copyright. Use your “@view.do" email address for contributions.

## Respect

Although technical in nature, the Open Source community is first and foremost about people. Treat other people with respect. Be kind, be open, respect the culture of the community you are interacting with and be aware of the diversity of people in that community. Be aware that, particularly in electronic communication, you might misunderstand or misinterpret what others are saying or meaning. The reverse is also true.

Follow any codes of conduct and set a high bar for your own behavior.

## Consuming Open Source Software

We consume Open Source Software as users, as base for products or other projects. We also package projects of Open Source Software as part of the view.DO brand.

Using Open Source software is generally fine in most cases. When running it as a service there are some extra considerations necessary such as how to deal with privacy rights etc. These additional considerations are out of the scope for this document and you should seek the necessary advice.

When consuming Open Source in anything we distribute to others there are some guidelines to follow:

### Licenses

All code licensed under an OSI approved license can generally be used. Be careful when combining code with different licenses. Certain licenses are incompatible when combined in the same program. Mere aggregation in the distribution usually does not pose a problem. Consult with the view.DO legal team if you are not sure.

### Managing Source Code

For all the software we distribute we need to keep the source code. This is necessary so we can give users and customers the source for the software in compliance with the Open Source software licenses and in the spirit of the Open Source model. We also need the code to be able to fix problems and apply patches without being dependent on any third party.

It is necessary to create a bill of materials for our products which lists all components being used including dependencies. The list should include names, version, license, and upstream URL for all components.

## Legal Review

view.DO conducts a legal review of code we distribute in order to make sure we have the rights to distribute the code and that there are no legal issues such as license incompabilities.
