# Envisioning a future in scholarly communication

__For the 2017 IFLA conference, theme: The Open Revolution__

## Abstract



## Body

Scholarly communication is in dire need of disruption. <!-- Many say we need incremental change to produce a sustainable scholarly communication system, but I oppose this idea because after decades of identifying various problems we have seen little sustainable change that truly reimagines how we communicate. We cannot turn a horse into a motor vehicle, so why even try. In this perspective piece, I try to radically reimagine the scholarly communications infrastructure based on the tools that are available to us now and invite everyone to criticize these ideas. Only with diversity of ideas can we truly make progress; currently the decisions are driven by a few oligopolies [@10.1371/journal.pone.0127502] and the tenured professors or policymakers mostly from a different generation. This decreases the diversity of ideas and is stalling the development of how scholars communicate, with dire consequences as has become noticable in recent years. For clarification, with scholars I mean anyone who is interested in consuming, producing, distributing, or contributing to the knowledgebase of our species, regardless of their affiliation or lack thereof. -->

In the last decades, interpersonal communication has changed tremendously. <!-- These past decades have brought with it so much diversity in communication that it can become confusing (see [Figure 1](#fig1)), but it is also liberating by allowing innovative ways to communicate (e.g., social media) or making available previously difficult to use safety measures (e.g., encryption).  -->

```{r xkcd-1810, fig.cap="A comical example of the diversity in communication channels.", echo = FALSE}
knitr::include_graphics('figs/xkcd-1810.png', auto_pdf = TRUE)
```

However, the way scholars communicate their findings has barely changed. <!-- remaining stuck in a paper paradigm. despite the potential we have seen in digital communications on all other interpersonal levels. Despite these developments in communication at a personal level,  l having massive effects on the way we communicate on a personal level and during our day-to-day work as scholars, we have not realized the potential of scholarly communication in the digital age - we still produce in a paper format, albeit digitized.  -->

The scholarly process is much more complicated than can be captured in a static paper publication, which is communicated at the very end and encourages one-way communication. <!-- Registered Reports have already indicated that  -->

Additionally, the scholarly process has grown _more_ complicated due to increased variation in the research tools available.<!--  with the increase in computing techniques applied in scholarly research, the scholarly process has become more complicated in recent decades, whereas the communication system has not changed  proportional to this increasing complexity.  To the contrary, one might even pose that the complexity has decreased, shifting methods into obscure corners of a paper. -->

As such, the scholarly process has become _more_ of a black box than before. 

Breaking up the reign of the paper paradigm is therefore a necessity to better represent and understand how scholarly results come into existence. 

Additionally, due to the commodification of the resource (i.e., knowledge), a new system where ways to consume information is commodified are actively stifled.

Commodification of consumption greatly encourages society to innovate how people can discover and reuse information. <!-- For Wikipedia alone, one of the greatest resources of uncommodified knowledge, there are tons of applications that allow you to consume that information in various ways on various devices.  -->

By focusing on the commodification of consumption instead of commodification of the resource, the problem of access to knowledge can be resolved in a sustainable manner. <!-- Politicians and scholars have been discussing Open Access for at least 15 years. -->

Additionally, commodification of consumption removes several perverse incentives from the scholarly system that now produces unreliable knowledge. <!-- For example, innovativeness and surprisingness are criteria upon which articles are currently selected, where those exact some properties increase the probability that the finding is false [@10.1371/journal.pmed.0020124]. -->

The main tenet underlying the themes of Open Access, Open Data, Open Science, and replication initiatives in scholarly communication is sustainability. <!-- Sustainability of consuming knowledge (Open Access), sustainability of producing reliable knowledge ("reproducibility crisis"), sustainability of The serial crisis indicates that access to knowledge is currently unsustainable (e.g., Harvard cannot even access everything with its massive budget).  -->

In this perspective piece, I propose a redesign of the scholarly communication system that is flexible, decentralized, and distributed, which immediately allows for more sustainability and diversity in the way we consume, produce, and access knowledge.

## Sustainable scholarly process

Single points of failures make a system vulnerable to outages, (malicious) adjustment of content, or even complete removal of content. <!-- As such, a centralized infrastructure is easier to disrupt than a decentralized or distributed one. The Internet is currently organized in such a way that it is relatively centralized, whereas the Darknet (i.e., an alternative cyberspace) is less centralized and has been found to be more resilient [@10.1103/PhysRevE.95.022313].  -->

The scholarly process is ridden with single or few points of failures and sharing makes this a many points for failure system. <!-- For exactly this reason it is so important that scholars become more transparent about their data, their hypotheses, their results, and the chronology of a. -->

<!-- The scholarly communications system is currently centralized at publisher websites, is insecure, and is not resilient. HTTP(S) because redistribution is frequently by copyright Unrestrictive licensing, such as the Creative Commons BY license, allow for free redistribution and increases persistence. For example, anyone can download the entire corpus of Hindawi right now and if Hindawi would then become inaccessible, the articles would still be available regardless. Copyright creates dependence whereas the lack thereof creates independence. -->

Hence, a sustainable scholarly communications system needs to be both decentralized and distributed.

Decentralization is achievable with new peer-to-peer (p2p) Internet protocols such as `dat` and `ipfs`. <!-- Such p2p networks send information across the network, but are is resilient to nodes being removed because they operate in mesh network. If 20 peers have the files, removing one from the network does not affect the availability of the files-->

Such p2p networks also allow for ready redistribution when copyright is leveraged to work for distribution.

Alongside decentralization and distribution, integrity of the scholarly record can also become better. The chronology of the scholarly process can be ensured by splitting up the paper article as we know it into nodes of information.

These nodes can easily be logged on a blockchain based ledger of which everyone can have a copy (e.g., [Hyperledger](https://github.com/hyperledger/fabric)-based). <!-- An example is available below -->

```json
{
	"parent": null,
	"self": "dat://92b9b1b95e18c1dd1546c25ac49609da6fb0e3f2abc94ecf17609c565888c16b",
	"time-deposit": "2017-04-10T18:38:03+02:00",
	"time-available": "2017-04-10T18:38:03+02:00",
	"authors": "b601f276870ebf4920b3c78c4af51d3ed3bf4db7ab2b9c4faa74e0b457aa13ed",
	"type": "hypotheses"
}

{
	"parent": "dat://92b9b1b95e18c1dd1546c25ac49609da6fb0e3f2abc94ecf17609c565888c16b",
	"self": "dat://c2c291f93fa635c7fc7bc6e8ba504937b1821c5be45ab7c859f6e6cd19a291b7",
	"time-deposit": "2017-04-12T12:07:06+02:00",
	"time-available": "2017-08-12T12:07:06+02:00",
	"authors": "b601f276870ebf4920b3c78c4af51d3ed3bf4db7ab2b9c4faa74e0b457aa13ed",
	"type": "data"
}
```

Each entry in the ledger needs to be self-containing and refer to all relevant files.

The ledger can also allow for time-locked sharing but with a clear chronology of creation.

Combinations of ORCIDs can be hashed into unique author combinations (and ordering!) to provide identification over time, but remove gender and status bias (amongst other things).

What types of nodes are contained in the ledger, is something that requires discussion and can change over time.

For a sustainable distribution system, persistent nodes need to be identified: libraries.

Nonetheless, other stakeholders benefiting from maintaining the distribution of the decentralized network are (not-)for-profit companies that build services on top of the resources.


## Locking the system open

When Brewster Kahle spoke at OpenCon2016, he mentioned that we need to lock the system open. At first, it would seem only the open advocates win in that case, but I think the for-profit companies can benefit from this as well by opening up a whole new market where more return can be made and in a more sustainable manner.