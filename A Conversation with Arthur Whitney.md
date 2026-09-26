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

$~~$ I left I.P. Sharp sometime around 1980. Then I went to graduate school at the University of Toronto where I did pure mathematics, but mostly I

$~~$ was just goofing around. All through the ’80s I was implementing my own languages: object-oriented languages, a lot of different LISPs,

$~~$ Prolog. In 1985 I got a job at Stanford, where I implemented a Prolog inference-engine kind of language. Then I was with an artificial

$~~$ intelligence company called Teknowledge.

\- **BC**

$~~$ Were you developing these languages because you needed a certain expressive power in the language to solve a particular problem at hand?

$~~$ What were the motivations for these languages?

\- **AW**

$~~$ My motivation was always to create a general-purpose programming language that would solve all problems and be interpreted, but fast.

\- **AW**

$~~$ At Stanford the language was determined by the professor, and he wanted to have an inference engine, so the motivation there was artificial

$~~$ intelligence, but I wasn’t much interested in that.

\- **AW**

$~~$ My big break was in 1988 when I joined Morgan Stanley. There the motivation was a terabyte of TIC (Treasury International Capital) data, and

$~~$ back then there were a few million transactions a day being processed by realtime trading systems. I think we had one of the biggest trading

$~~$ operations in the world. We had a portfolio that was a billion dollars: half a billion long, half a billion short. We were trading every second

$~~$ electronically. The data set was a terabyte, but we compressed it down. It was pairs trading, and I wrote an APL to do all of that—the big

$~~$ database and the realtime trading—so our entire department was using my language.

\- **BC**

$~~$ You had used APL, and then you explored these other languages—Prolog variants and so on—but when you got to Morgan Stanley you came

$~~$ back to APL. What brought you back?

\- **AW**

$~~$ I much preferred implementing and coding in LISP, but once I was dealing with big data sets and then having to do fairly simple calculations,

$~~$ APL just seemed to have the better vocabulary.

\- **AW**

$~~$ It had to come up one level. Common LISP even then had about 2,000 primitives. I didn’t like that. What I liked was the original LISP, which

$~~$ had car, cdr, cons, and cond, but that was too little. Common LISP was way too big, but a stripped-down version of APL was in the middle

$~~$ with about 50 operations. It’s about the same size as C. But the thing about the languages that I implement is that there are no libraries: those

$~~$ 50 operations are it. Everybody builds from there, and the resulting programs are extremely short.

\- **BC**

$~~$ There the problem did serve as a motivator. You had this massive amount of data, and you needed a language that could deal with that large

$~~$ amount of data in a first-class fashion. Did other people around you see the expressive power, because even at that time I would assume that

$~~$ APL was beginning to wane a bit?

\- **AW**

$~~$ APL peaked in the ’70s, but in the finance industry APL was very strong, so there was no difficulty in doing my own APL version.

\- **BC**

$~~$ How did your own APL differ from the original? Did you change the primitives that were being exported?

\- **AW**

$~~$ The primitives were a little different; the grammar was pretty much the same. The syntax was the same. The vocabulary was very similar, but

$~~$ not enough to be anything close to portable.

\- **BC**

$~~$ I’m sure that practitioners who know APL only by reputation are going to wonder if it used the same wonky characters as the original APL.

\- **AW**

$~~$ Yes, at Morgan Stanley I did use the APL characters, but on my next iteration, K, which was in ’92, I gave up on those characters.

\- **BC**

$~~$ Why did you give up on them? And how did you feel about giving up on the characters?

\- **AW**

$~~$ Well, it felt great because it was easier to send e-mails. They’re beautiful characters, but I had to strip the language down. K today has no

$~~$ reserved words; it just uses the ASCII keyboard. It’s completely arbitrary, but it makes me keep the language small.

\- **BC**

$~~$ You speak about the arbitrariness in using the ASCII keyboard. I heard one feature being described as this: “When Arthur ran out of

$~~$ punctuation, he used a leading underscore to denote system primitives.” When I read that I thought to myself, “That’s a little ridiculous,” but

$~~$ then I thought of all the goofy punctuation characters we have in other languages: C uses nearly all of them; many languages use the balance.

$~~$ And we use them in different contexts and different ways.

\- **AW**

$~~$ Certainly it’s unfamiliar, and people say, “Oh, it looks like line noise.” But even kids can learn this quickly.

\- **BC**

$~~$ Obviously, a point of pride for K is the ability to phrase things concisely. Is there any length that is too short, where you’ve actually squeezed 

$~~$ too much information out in terms of its readability?

\- **AW**

$~~$ Yes, and I expect I cross that boundary a lot. But if every line has up to seven operations, then I think that’s manageable. In fact, we can

$~~$ remember seven things.
