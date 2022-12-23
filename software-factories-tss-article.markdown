---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
title: "Software Factories: Refectoring an Industry"
permalink: /software-factories-article/
---

**(I'm republishing an old article I had written about 10 years ago that seems to have disappeared from the web. This was originally published in 2006 on TheServerSide.net: http://www.theserverside.com/discussions/thread.tss?thread\_id=32812)**

Software development has always been costly and time-consuming process. Specialized requirements and lack of skilled resources are just two of the difficulties facing companies today. Pressure to deliver software, on time and within budget, have pushed developers to look for a way to increase value delivered, while decreasing development time.

For many years now, efficient reuse of existing assets, either through object-oriented programming, component-based development or patterns-based architecture, has been one of the core objectives for the IT industry as a whole. Software reuse is seen as a means to combat many of the problems facing development teams. However, for many years and several different technology paradigms, this level of reuse has eluded the industry as a whole.

The book Software Factories: Assembling applications with Patterns, Models, Frameworks, and Tools aims to change this by modifying the definition of reuse as used by the IT industry and bring a more manufacturing approach to software reuse.

**Economies of Scale vs. Economies of Scope**

The difference between these two definitions are subtle and is something that has been proven outside of the software industry, in more established industries like manufacturing and fabrication. While both promise to reduce time and cost and improve product quality, they are actually quite different.

Economies of scale occurs when the initial development of a design and subsequent construction of a prototype result in multiple copies of that prototype are created. This is similar to the fabrication industry when a custom part is created and that part is used to produce hundreds or thousands of similar parts. In the manufacturing industry, it's similar to a machine being built that can produce screws in bulk. In this case, ruse occurs in the later stage of production, namely construction.

Economies of scope occurs when multiple similar, but unique designs are produced in groups, as opposed to individually. Authors Jack Greenfield et.al uses the example of a car manufacturing plant that uses existing designs, such as chassis, body and interiors, to produce several lines of distinct cars. Each product line is complete with custom features, but all share that same underlying design. Here the reuse occurs earlier in production, namely design and prototyping.

Greenfield et.al point out that for years, the IT industry has been trying to apply economies of scale for achieving software reuse, when in fact, the IT industry should have been trying to apply economies of scope to achieve reuse.

**Chronic Problems of Software Development**

The authors of Software Factories identity some major problems with how the IT industry is attempting to achieve reuse. Unfortunately, simply altering how software reuse is applied within an industry or an organization won't make systematic reuse a reality. Greenfield et.al identify four chronic problems with software development, each of which impede a teams' ability to gain valuable insight and reuse from existing domain knowledge and experience. These problems are: â€¢

*   Monolithic Development
*   Copious Granularity
*   Process Immaturity
*   One-off Developer

**Monolithic Development**

Monolithic development means the creation of software in such a way as to make it difficult or even impossible, to utilize the resulting artifacts outside of a narrowly defined scope. Software development teams within large organizations are certainly familiar with this style of development. Several projects, several teams, all building isolated applications, without concern for what anyone else may be doing, or what, if any, domain knowledge they are embedding within the application. This results in large, inflexible applications that are of little use to anyone outside the original, intended audience. Even two projects within a single organization can be faced with a mini-integration effort in order for one application to take advantage of another's functionality. Why does this keep occurring within organizations? Industry leaders have championed design by assembly for years, and yet very few applications take advantage of existing components, even within their own organization.

**Copious Granularity**

Typical software development for business applications consists of a strikingly similar set of features and functionality. For example, many business applications read data from a database, present it to the user, allow the user to modify the data in some way, and then allow the user to persist the change back to the database. Even though this is an over simplification of most applications, the basics still remain the same across projects. It begs the question of why developers use such fine-grained tools as standard programming languages like C# and VB .NET for representing such basic patterns? Part of the reason is the immaturity of modeling tools and languages. While a language such as UML is suitable for documenting software architecture, it is inadequate for allowing implementation to be derived from such models. UML lacks the extensibility required for generating large amount of code, and also lacks the breadth required to represent all aspects of software, including databases and user interfaces.

**Process Immaturity**

*   Controlling complexity at the expense of change -- Many "traditional" processes would fall under this heading, including RUP and Waterfall
*   Controlling change at the expense of complexity -- Most "agile" methodologies would fall under this heading, including Scrum and XP Before a process can be tuned for software reuse, it must mature because automation can only automate well-defined processes.

**One-off Development**

Software development projects within a company are usually so focused on the bottom line and delivery time, that overall architecture is placed on the back burner as "lofty" or "academic". Very little regard is taken to analyze and evaluate existing assets, and very little time is dedicated to ensuring that new assets produced are reusable within other contexts. This results in many development efforts within a single company that create various amounts code and valuable assets for use within the company's domain. Projects rarely perform post-mortems where reusable components are identified, documented, and packaged in such a way as to become reusable by other projects. These four problems, as well as the industrys' misunderstanding of how to apply reuse with the current economic model, paint a pretty bleak picture as to the future of software development as an industry, especially compared to other more mature industries, such as manufacturing. Luckily, this is where the Software Factory comes into play. The next section contains a brief overview of what is a Software Factory is and identifies some of its main components.

**Software Factories: The Solution?**

When creating software within a specific vertical, knowledge about that vertical is frequently embedded in the software being developed. Unfortunately, this knowledge remains hidden inside the software; unable to be reused outside of the original scope of the software that contains it. This means reuse of this knowledge is next to impossible. This is where Software Factories look to step in with methods and procedures to harvest that knowledge, turning that knowledge into reusable production assets for a company. A Software Factory is defined by Greenfield, et al., as a software product line that configures extensible tools, processes, and content using a software factory template based on a software factory schema to automate the development and maintenance of variants of an archetypical product by adapting, assembling and configuring framework-based components. In layman's terms, a Software Factory are about collecting existing, specialized knowledge about a certain domain and applications built within that domain. You can then use that knowledge to create a blueprint for other applications of a similar type. That schema can then be tweaked and configured to produce semi-functional to functional applications. In short, Software Factories means application generation from valuable, and reusable production assets that exist within an organization. Before delving into what makes components comprise a Software Factory, let's first take a look at a look at the current state of the IT industry as compared to other industries.

**Moving from Craftsmanship to Industrialization**

All too often, highly skilled application developers and architects have to use their time for low-level, implementation level tasks. Usually, junior developers are not able to complete such tasks because of lack of appropriate domain knowledge, requiring the senior developer to mentor the junior developer. This fosters not only knowledge transfer, but also an introduction to the complexities of the current development environment. Since developers are always involved at some stage of development, very little time is spent in making development more efficient, especially low-level implementation details. This method of development resembles early goods based industries, where single workers create custom solutions, tailored to each individual requirement. Think early tailors or shoe cobblers.

This craftsmanship approach to software development does not scale very well. The lack of quality senior developers creates a mentoring environment, where specialized knowledge must be transferred, similar to an apprenticeship. Since there is such a hands-on approach required, each part of the project need to be created, most of the time, by hand. This often leads to higher quality, but also leads to performance and efficient issues. Migrating from a craftsmanship-based industry to a more industrial-based industry has been the path of progression for many more mature industries. If this is the end result for so many other industries, why is software development still based on small groups of highly specialized craftsmen?

Most people within the IT industry will agree that a form of standardization and modularization is the key to enabling the kind of reuse required for efficient industrialization of software development. What they don't agree on is the means to which this standardization and modularization is achieved. The Software Factory aims to address this effort by prescribing a process by which software can be modularized into reusable assets.

**Components of Software Factories**

There are 3 main components of Software Factories:

*   Models and Patterns
*   Domain Specific Languages
*   Software Product Lines

**Models and Patterns**

The authors of Software Factories define Model-Driven Development as:

> using models to capture high level information, usually expressed informally, and to automate its implementation, either by compiling models to produce executables, or by using them to facilitate the manual development of executables.

The importance of models comes from their ability to keep a consistent representation of concepts within a project. For example, while it's easy to draw and manipulate a person object in a model, it's much more difficult to manipulate the same person object at a lower level, because the person object could be represented by class files, tables, and columns in a database.

Representing and manipulating core abstractions and concepts within a software system is only half the battle, though. The other half comes from being able to effectively use those models to generate the underlying implementation details represented by the model

**Domain Specific Languages**

Domain Specific Languages, or DSLs, have long been a way to provide an abstraction atop existing concepts within a specialized domain. Examples of a DSL include SQL and HTML. Both provide specialized languages for manipulating concepts within their respective domain -- tables, rows, and columns in the case of SQL and elements, tables, and forms in the case of HTML. For years DSLs like these remained the only cost effective DSLs because of their wide spread use and generalized concerns. No matter what your specific project entails, if you use a database, you can use SQL and if you use web pages, you can HTML. Creating DSLs for other, more vertical concerns has always been cost prohibitive because of the lacks of tools.

However, several companies have recently announced tools or plug-ins for the creation of DSLs. Once these DSLs are created, they can be utilized within a company to work with components at a much high level, with a much higher level of software reuse.

**Software Product Lines**

Software Product Lines are entire subsets of components that can be configured, assembled, and packaged to provide a fairly complete product. The resulting product should only require customization from a developer for the highly specialized aspects of the project. Perhaps the largest component of a Software Factory, Software Product Lines not only provide the greatest value, but also require the greatest investment. Software must be carefully partitioned into distinct and reusable components and those components must readily fit together in a coherent manner. Configuration is the key to Software Product Lines, as projects must be able to pick and choose which components they want to utilize, and then generate an application off of that configuration.

Implementing a Software Factory While all of the promises of Software Factories sound appealing, many companies have tried to provide the tools and components, only to fail under the load of inflexible tools or proprietary formats.

All of this is about to change. Big-name companies like Microsoft and Sun are getting ready to release many of the components necessary for building and assembling a Software Factory within an organization. With the release of Visual Studio 2005, Microsoft will unveil several add-ins and plug-ins that enable the creation of not only Domain Specific Languages, but also the integration of those languages with the IDE itself. This will allow developers to manipulate and use the language from within the Visual Studio.NET IDE.

Not to be outdone, Sun Microsystems is working on its own implementation of Software Factory technology, simply named Project Ace. Although, very little details of "Project Ace' are available, developers shouldn't expect Sun to let Microsoft provide .NET tools, without answering with a comparable set of tools for Java.

**What about now?**

While all this conjecture sounds wonderful for the future, many developers will be asking themselves what they can do now to utilize Software Factory techniques in their organizations today. Well, the good news is that a lot of functionality already exists with Visual Studio.NET. Products like Enterprise Templates, Project Item Templates, and Nant allow for the creation of standard artifacts that a team or organization can utilize today.
