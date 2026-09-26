**Category**: Interview

**Interview members**

\- _**Arthur Whitney**_

$~~$ Identity: The designer of the K and Q languages

\- _**Bryan Cantrill**_

$~~$ Identity: ACM Queue editorial board member

**Date**: 20 April 2009

**Title**: A Conversation with Arthur Whitney:

**Subtitle**: Can code ever be too terse? The designer of the K and Q languages discusses this question and many more with Queue

$~~~~~~~~~~~~~~~~~$ editorial board member Bryan Cantrill.

**Preface**: When it comes to programming languages, Arthur Whitney is a man of few words. The languages he has designed, such as A, K, and

$~~~~~~~~~~~~~~~~$ Q, are known for their terse, often cryptic syntax and tendency to use single ASCII characters instead of reserved words. While these

$~~~~~~~~~~~~~~~~$ languages may mystify those used to wordier languages such as Java, their speed and efficiency has made them popular with

$~~~~~~~~~~~~~~~~$ engineers on Wall Street.

**Background**: Whitney began his Wall Street career in the 1980s, building trading systems at Morgan Stanley using his own version of APL (the

$~~~~~~~~~~~~~~~~~~~~~~~~~~$ language on which all of his later languages are based). Eventually he started his own company, Kx Systems, which today provides

$~~~~~~~~~~~~~~~~~~~~~~~~~~$ realtime and historical data-analysis software to many Wall Street investment banks. The company’s signature product, KDB+, is a

$~~~~~~~~~~~~~~~~~~~~~~~~~~$ column-oriented database based on the K language.

**Introduction**: Eager to learn what’s behind Whitney’s unique languages (and curious to see if his reputation for concision carries over into real

$~~~~~~~~~~~~~~~~~~~~~~~~~~~$ life), we invited him to speak with Queue editorial board member Bryan Cantrill. Cantrill is best known for developing DTrace, a

$~~~~~~~~~~~~~~~~~~~~~~~~~~~$ tool for dynamic instrumentation of production systems that helps companies identify and fix performance bottlenecks. Whitney

$~~~~~~~~~~~~~~~~~~~~~~~~~~~$ was gracious enough to invite Cantrill to his home in Palo Alto, where they spoke about his career, his languages, and the

$~~~~~~~~~~~~~~~~~~~~~~~~~~~$ essence of elegance.

**Conversation**

\- **BRYAN CANTRILL**

$~~$ You are a bit of a rarity in software engineering in that you have been writing software on a daily basis for decades. Your first introduction to

$~~$ computing was APL with the master, Ken Iverson. What was that like?

\- **ARTHUR WHITNEY**

$~~$ In 1969, I was 11, and Ken Iverson was at IBM Research in Yorktown. He had been a friend of my dad’s at Harvard in the ’40s. We lived in

$~~$ Alberta, but we were driving around the continent and went to visit him. He showed me programming on a terminal in his house in Mount

$~~$ Kisco. This was in the ’60s, and already it was interactive, and it was very quick to write programs and get results.

\- **BC**

$~~$ You must have been the only 11-year-old on the planet getting that kind of demonstration of programming in 1969.

\- **AW**

$~~$ Of course, I had no idea about that, and I didn’t really pay much attention. He showed me some stuff, and I thought it was cool. In ’74 when I

$~~$ went to a university and took a computer class, they were using punch cards, which made no sense because five years earlier I had already

$~~$ seen interactive programming.

\- **BC**

$~~$ Did you start working on APL at Waterloo?

\- **AW**

$~~$ No, at Waterloo I just did some APL for a week. I was a math major and I wasn’t interested in computers because I just wanted to do pure

$~~$ math. So I really missed a big opportunity.

\- **BC**

$~~$ Well, I’m not sure if you missed it or if you just found the opportunity a different way.

\- **AW**

$~~$ It took me a long time. For the next 10 years I did a little bit of APL in the summers as a consultant, but it wasn’t until about 1980 when I was

$~~$ working with Ken at a Canadian company called I.P. Sharp that I really began using it regularly. Ken had retired from IBM after 20 years and

$~~$ was working at I.P. Sharp in Toronto.

\- **AW**

$~~$ I.P. Sharp was an amazing company. It had its own worldwide network that had nothing to do with DARPA (Defense Advanced Research

$~~$ Projects Agency). We were sending e-mails and instant messages to Australia and Singapore. The whole company was APL.

\- **BC**

$~~$ They were selling APL time sharing, right?

\- **AW**

$~~$ Yes, and it was easy because the one computer in Toronto was running the entire world.

\- **BC**

$~~$ What kinds of problems were people using the APL time-sharing service for?

\- **AW**

$~~$ It was mostly general-purpose business computing, such as accounting systems. I did a 2-billion-row database, so we were doing very big

$~~$ databases and data analysis—what today, 20 years later, they call OLAP (online analytical processing).

\- **AW**

$~~$ I left I.P. Sharp sometime around 1980. Then I went to graduate school at the University of Toronto where I did pure mathematics, but mostly I was just goofing around. All through the ’80s I was implementing my own languages: object-oriented languages, a lot of different LISPs, Prolog. In 1985 I got a job at Stanford, where I implemented a Prolog inference-engine kind of language. Then I was with an artificial intelligence company called Teknowledge.
