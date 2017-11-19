
Ethereum: Now Going Public  以太坊：现在公开发行了
--------------------------

> 本文翻译自：https://blog.ethereum.org/2014/01/23/ethereum-now-going-public/
>
> 译者：[区块链中文字幕组](https://github.com/BlockchainTranslator/EOS) [何德林](https://github.com/BlockchainTranslator/EOS)
>
> 翻译时间：2017-11-11

---------------------------

I first wrote the initial draft of the Ethereum whitepaper on a cold day in San Francisco in November, as a culmination of months of thought and often frustrating work into an area that we have come to call “cryptocurrency 2.0″ – in short, using the Bitcoin blockchain for more than just money. In the months leading up to the development of Ethereum, I had the privilege to work closely with several projects attempting to implement colored coins, smart property, and various types of decentralized exchange. At the time, I was excited by the sheer potential that these technologies could bring, as I was acutely aware that many of the major problems still plaguing the Bitcoin ecosystem, including fraudulent services, unreliable exchanges, and an often surprising lack of security, were not caused by Bitcoin’s unique property of decentralization; rather, these issues are a result of the fact that there was still great centralization left, in places where it could potentially quite easily be removed.

在经历几个月的兴奋思考、又常常陷入沮丧之后，我在旧金山11月寒冷的一天，开始写以太坊白皮书初稿，我们都称之为的“加密货币2.0”——简而言之，使比特币区块链不仅仅有货币的功能。在开发以太坊之前的几个月里，我有幸与多个项目紧密合作，包括实现彩色币、智能财产以及各种类型的分布式交易所。当时，我很兴奋，这些技术可能带来的巨大潜力，我敏锐地意识到，许多仍然困扰着比特币生态系统的重大问题，包括欺诈服务、不可靠的交易所和经常令人吃惊的不安全性，不是由于比特币独特的去中心化特性造成的。相反，这些问题是仍然有很大的中心化所导致的，在一些可能很容易被消除的地方。

What I soon realized, however, was the sheer difficulty that many of these projects were facing, and the often ugly technological hacks that were required to make them work. And, once one looks at the problem carefully, the culprit becomes obvious: fragmentation. Each individual project was attempting to implement its own blockchain or meta-layer on top of Bitcoin, and considerable effort was being duplicated and interoperability lost as a result. Eventually, I realized that the key to solving the problem once and for all was a simple insight that the field of computer science first conceived in 1935: there is no need to construct a separate infrastructure for each individual feature and implementation; rather, it is possible to create a Turing-complete programming language, and allow everyone to use that language to implement any feature that can be mathematically defined. This is how our computers work, and this is how our web browsers work; and, with Ethereum, this is how our cryptocurrencies can work.

然而，我很快意识到，许多这些项目都面临着巨大的困难，而且往往需要技术黑客发挥作用。而且，一旦人们仔细研究这个问题，罪魁祸首就变得显而易见：碎片化。每个项目都试图在比特币之上实现自己的区块链或基础层，因此有大量的重复工作和缺乏互操作性。最终，我意识到解决这个问题的关键是基于一个简单的见解，在1935年计算机科学第一次认识到的：没有必要为每个的特定功能和实现，构建一个单独的基础结构；更确切地说，可以创建一个图灵完备的编程语言，并允许每个人使用该语言来实现任何可以在数学上定义的特定功能。这就是我们的计算机工作原理，这就是我们网络浏览器的工作原理；而且，有了以太坊，这就是我们加密货币的工作方式。

Since that moment, Ethereum has come very far over the past two months. The Ethereum team has expanded to include dozens of developers including Gavin Wood and Jeffrey Wilcke, lead developers of the C++ and Go implementations, respectively, as well as others including Charles Hoskinson, Anthony Di Iorio and Mihai Alisie, and dozens of other incredibly talented individuals who are unfortunately too many to mention. Many of them have even come to understand the project so deeply as to be better at explaining Ethereum than myself. There are now over fifteen people in our developer chat rooms actively working on the C++ and Go implementations, which are already surprisingly close to having all the functionality needed to run in a testnet. Aside from development effort, there are dozens of people operating around the world in our marketing and community outreach team, developing the non-technical infrastructure needed to make the Ethereum ecosystem the solid and robust community that it deserves to be. And now, at this stage, we have made a collective decision that we are ready to take our organization much more public than we have been before.

从那以后，在过去的两个月里，以太坊进展非常快。以太坊团队已经扩大到数十名开发人员，包括Gavin Wood和 Jeffrey Wilcke，分别负责领导C++和GO的开发，以及Charles Hoskinson, Anthony Di Iorio and Mihai Alisie等，和其他几十个非常有才华的人，太多不能一一提及。他们中的许多人甚至已经深入地了解了这个项目，比我还能更好地解释以太坊。现在，我们的开发人员聊天室里，有超过15人活跃开发者在使用C++和Go开发功能，目前的功能已经非常接近于测试网络中运行所需的所有功能了。除了开发工作之外，还有数十人的全球运营团队，在营销和社区拓展方面开展工作，开发非技术基础设施，以使以太生态系统成为坚实而健全的社区。现在，在这个阶段，我们做出了一个集体决定，我们已经准备好让我们的组织比以前更加公开。

1. What Is Ethereum 以太坊是什么?

In short, Ethereum is a next-generation cryptographic ledger that intends to support numerous advanced features, including user-issued currencies, smart contracts, decentralized exchange and even what we think is the first proper implementation of decentralized autonomous organizations (DAOs) or companies (DACs). However, this is not what makes Ethereum special. Rather, what makes Ethereum special is the way that it does this. Instead of attempting to specifically support each individual type of functionality as a feature, Ethereum includes a built-in Turing-complete scripting language, which allows you to code the features yourself through a mechanism known as “contracts”. A contract is like an autonomous agent that runs a certain piece of code every time a transaction is sent to it, and this code can modify the contract’s internal data storage or send transactions. Advanced contracts can even modify their own code.

简而言之，以太坊是一个下一代加密账本，它打算支持许多高级功能，包括用户发行货币、智能合约、分布式交易所，甚至我们认为是第一个分散自治组织(DAOs)或公司(DACs)的实现。然而，这并不是使以太特别的原因。更确切地说，使以太特别的是它实现这个的方式。它没有试图特别支持每个单独的功能类型作为一个特性，它包括一个内置的图灵完备脚本语言，它允许您通过一个称为“合约”的机制来自己编写功能。合约就像一个自治代理，每次交易发送给它时，它都会运行一定的代码，这个代码可以修改合约的内部数据存储或发送其他的交易。高级合约甚至可以修改自己的代码。

A simple example of a contract would be a basic name registration system, allowing users to register their name with their address. This contract would not send transactions; its sole purpose is to build up a database which other nodes can then query. The contract, written in our high-level C-Like Language (CLL) (or perhaps more accurately Python-like language), looks as follows:

一个简单的合约例子，是一个基本的名称注册系统，允许用户注册他们的名字和他们的地址。该合同不发送交易;它的唯一目的是，建立一个其他节点可以查询的数据库。合约的编写，是用我们的高级类C语言(CLL)写的(或者更准确地说，类Python语言)，看起来是这样的:

if tx.value < block.basefee * 200:
stop
if contract.storage[tx.data[0]] or tx.data[0] < 100:
stop
contract.storage[tx.data[0]] = tx.data[1]

And there you have it. Five lines of code, executed simultaneously by thousands of nodes around the world, and you have the beginnings of a solution to a major problem in cryptography: human-friendly authentication. It is important to point out that when the original version of Ethereum’s scripting code was designed we did not have name registration in mind; rather, the fact that this is possible came about as an emergent property of its Turing-completeness. Hopefully this will give you an insight into exactly what Ethereum makes possible; for more applications, with code, see the whitepaper. Just a few examples include:

就是这样。5行代码，被全球数千个节点同时执行，您已经开始解决密码学中的一个主要问题：用户友好的身份验证。需要指出的很重要的一点是，当我们设计了以太脚本代码的早期版本时，我们并没有考虑到名称注册；更确切地说，这是可能的，因为图灵完备是更紧急的功能。希望，这能让你更准确地了解什么是以太坊。对于更多的应用、代码，参见白皮书。下面的例子包括:

User-issued currencies / “colored coins”

用户发行的货币/“彩色币”
Decentralized exchange

分布式交易所
Financial contracts, including leverage trading and hedging

金融合约，包括杠杆交易和套期保值
Crop insurance

农作物保险
Savings wallets with withdrawal limits

有取款限制的储蓄钱包
Peer to peer gambling

点对点赌博
Decentralized Dropbox-style data storage

去中心化的Dropbox-style数据存储
Decentralized autonomous organizations

分权自治组织

Perhaps now you see why we are excited.

也许现在你明白我们为什么兴奋了。

2. Who is Ethereum  以太坊团队

The core Ethereum team includes four members:

核心以太团队包括四名成员:

Vitalik Buterin

Vitalik Buterin first joined the Bitcoin community in March 2011, and co-founded Bitcoin Magazine with Mihai Alisie in September 2011. He was admitted to the University of Waterloo to study computer science in 2012, and in 2013 made the decision to leave Waterloo to travel through Bitcoin communities around the world and work on Bitcoin projects full time. Vitalik is responsible for a number of Bitcoin projects, including pybitcointools, a fork of BitcoinJSand multisig.info; now, he has returned to Canada and is fully dedicated to working on Ethereum.

Vitalik Buterin于2011年3月加入比特币社区，并于2011年9月与Mihai Alisie共同创立了比特币杂志。2012年，他被Waterloo大学录取，学习计算机科学。2013年，他决定离开Waterloo大学，周游世界各地的比特币社区，并在比特币项目上全职工作。Vitalik负责过一系列的比特币项目，包括pybitcointools，一个BitcoinJS分叉 和 multisig.info；现在，他已经回到加拿大，全身心投入到以太坊的工作。

Mihai Alisie

Mihai Alisie’s first foray into the Bitcoin community is Bitcoin Magazine, in September 2011. From Issue #1, which was shipped from his living room in Romania, to today Bitcoin Magazine bears Mihai’s imprint, and has grown as he has grown with the magazine. What started out as a team of people that didn’t have any experience in the publishing industry, is now distributing a physical magazine internationally and in Barnes & Noble bookstores across the US. Mihai is also involved in an innovative online e-commerce startup known as Egora.

Mihai Alisie2011年9月首次涉足比特币社区，是Bitcoin杂志。从他在罗马尼亚起居室发运的第一期，到今天的Bitcoin 杂志上，都印着Mihai的印记，随着杂志的发展，他已经成长起来了。作为一群在出版业没有任何经验的人组成的团队，现在正在全球范围内发行一本实体杂志，在全美的巴诺书店(Barnes & Noble书店)销售。Mihai还参与了一家名为Egora的在线电子商务初创公司。

Anthony Di Iorio

Anthony Di Iorio is a Founding Member, Board Member & Executive Director of the Bitcoin Alliance of Canada, Founder of the Toronto Bitcoin Meetup Group, and partner / founder in various Bitcoin start-ups and initiatives including the in-browser Bitcoin wallet KryptoKit, Cointalk, the Toronto-based Bitcoin hub and coworking spaceBitcoin Decentral, Bitcoin Across America, and the Global Bitcoin Alliance.

Anthony Di Iorio是比特币联盟一名创始成员，董事会成员和执行董事，多伦多比特币Meetup集团的创始人，一系列各比特币初创公司的创始人或合伙人，包括浏览器内置比特币钱包KryptoKit， Cointalk，多伦多比特币中心和共同办公的spaceBitcoin  Decentral、比特币在美国和全球比特币联盟。

Charles Hoskinson

Charles Hoskinson is an entrepreneur and cryptographer actively working on ventures in the Bitcoin ecosystem. He founded both the Bitcoin Education Project and Invictus Innovations prior to accepting his current role as a core developer of the Ethereum Project. He studied at Metropolitan State University of Denver and University of Colorado at Boulder with an emphasis in Analytic Number Theory. Charles is known for his love of economics, horology and MOOCs alongside a passion for chess and games of strategy.

Charles Hoskinson是一位企业家和密码学爱好者，他积极致力于比特币生态系统的投资。他创立了 Bitcoin Education Project 和Invictus Innovations，在他接受目前的角色为以太项目的核心开发者之前。他在Metropolitan State University of Denver和University of Colorado学习分析数论。Charles 以热爱经济学、钟表制造术和慕课教育而闻名，他对国际象棋和策略游戏充满热情。

We also have an excellent team of developers, entrepreneurs, marketers and evangelists:

我们还拥有一个优秀的开发人员、企业家、营销人员和布道者:

Dr. Gavin Wood: Core C++ Developer   核心C++开发人员
Geff Obscura: Core Go Developer  核心Go开发人员
Dr. Emanuele Costa: Quantitative Analyst; SCRUM Master  定量分析师、项目管理
Joseph Lubin: Software Engineering, Quantitative Analyst  软件工程
Eric Lombrozo: Software Architect 软件架构师
Max Kaye: Developer 开发人员
Jonathan Mohan: Media, Marketing and Evangelism (BitcoinNYC) 媒体、市场
Wendell Davis: Strategic Partner and Branding (Hive Wallet) 战略伙伴、品牌
Anthony Donofrio: Logos, branding, Web Development (Hive Wallet) LOGO、品牌
Taylor Gerring: Web Development  Web开发
Paul Snow: Language Development, Software Development 软件开发
Chris Odom: Strategic Partner, Developer (Open Transactions)  战略伙伴、开发人员
Jerry Liu and Bin Lu: Chinese strategy and translations  中国战略和翻译
Hai Nguyen: Accounting 会计
Amir Shetrit: Business Development (Colored Coins)  业务开发
Steve Dakh: Developer (KryptoKit) 开发人员
kyle Kurbegovich: Media (Cointalk) 媒体
3. Looking Forward  展望

I personally will be presenting at the Bitcoin conference in Miami on Jan 25-26. Soon after that, on February 1, the ether pre-sale will begin, at which point anyone will be able to obtain some of the initial pre-allocated ether (Ethereum’s internal currency) at a rate of 1000-2000 ether for 1 BTC by going to http://fund.ethereum.org. The pre-sale will run throughout February and March, and early funders will get higher rewards; anyone who sends money in the first seven days will receive the full 2000 ether, then 1980 ether on the 8th day, 1960 on the 9th day, and so forth until the baseline rate of 1000 ether per BTC is retained for the last three days of the pre-sale.

我个人将在1月25 - 26日迈阿密比特币会议上发言。不久之后，2月1日以太预售将开始，那时，任何人能够获得一部分早期的预售以太 (Ethereum内置货币)，以1000 - 2000以太 ：1 比特币的比例，在http://fund.ethereum.org上。预售期涵盖整个2月和3月，早期投资者将获得更高的报酬；任何在头七天内打钱的人将会收到2000以太 ，然后是第8天1980个以太，第9天1960个以太，等等，直到预售的最后3天，每BTC保持在1000以太。

We will be able to develop fully functional and robust Ethereum clients with as little as 500 BTC funding with current rates; basic implementations in Go, C++ and Python are coming close to testnet quality already. However, we are seeking to go much further than that. Ethereum is not “just another altcoin”; it is a new way forward for cryptocurrency, and ultimately for peer-to-peer protocols as a whole. To that end, we would like to be able to invest a large quantity of funds into securing top-notch talent for improving the security and scalability of the Ethereum network itself, but also supporting a robust Ethereum ecosystem hopefully bringing other cryptocurrency and peer-to-peer projects into our fold. We are already well underway in talks with KryptoKit, Humint and OpenTransactions, and are interested in working with other groups such as Tahoe-LAFS, Bitmessage and Bitcloud as well.

按照目前的比率，我们能在500个BTC基金的基础上，开发出功能强大而健壮的以太；Go、C++和Python的开发接近测试环境的质量。然而，我们正努力走得更远。Ethereum不是“另一个山寨币”；这是一种新的方式，对于加密货币来说，以及对 peer-to-peer协议整体而言。为此，我们希望能够投入大量资金，包揽顶尖人才，以提高以太网络本身的安全性和可扩展性，同时也支持一个健壮的以太生态系统，将其他加密货币和点对点项目引入我们的怀抱。我们已经在与KryptoKit、Humint和OpenTransactions进行谈判，并有兴趣与其他团体合作，比如tahoe - lafs,Bitmessage和Bitcloud。

All of these projects can potentially benefit from integrating with the Ethereum blockchain in some fashion, simply because the layer is so universal; because of its Turing-completeness, an Ethereum contract can be constructed to incentivize nearly everything, and even entirely non-financial uses such as public key registration have extremely wide-reaching benefits for any decentralized cryptographic product that intends to include, for example, a social network. All of these projects will add great value to the Ethereum ecosystem, and the Ethereum ecosystem will hopefully add great value to them. We do not wish to compete with any organization; we intend to work together.

所有这些项目都可以，通过与以太坊进行某种形式集成而获益，因为以太坊是如此通用；由于它的图灵完备，可以构造一个以太智能合约，激励几乎所有的东西，即使是完全非金融的用途，比如公共密钥注册，对于任何去中心化的加密产品都有非常广泛的好处，例如，一个社交网络。所有这些项目都将给以太坊生态系统带来巨大的价值，而以太生态系统也给它们带来巨大的价值。我们不希望与任何组织竞争；我们希望一起合作。

Throughout the fundraiser, we will be working hard on development; we will release a centralized testnet, a server to which anyone can push contracts and transactions, very soon, and will then follow up with a decentralized testnet to test networking features and mining algorithms. We also intend to host a contest, similar to those used to decide the algorithms for the Advanced Encryption Standard (AES) in 2005 and SHA3 in 2013, in which we invite researchers from universities around the world to compete to develop the best possible specialized hardware-resistant, centralization-resistant and fair mining algorithms, and will also explore alternatives such as proof of stake, proof of burn and proof of excellence. Details on this will be further released in February.

在整个资金募集过程中，我们将全力投入开发中；我们将发布一个中心化的测试环境，一个任何人都可以很快地发布合约和交易，然后很快，将会发布一个分布式的测试环境，具备测试网络功能和挖矿算法。我们也打算举办一个比赛,类似于2005年决定高级加密标准(AES)和2013年的SHA3，我们邀请来自世界各地大学的研究人员，来完成最好的抗硬件、抗中心化、公平的挖矿算法，并将探索替代方案，如POS，POB 和 POE。有关此事的细节将于2月进一步公布。

Finally, to promote local community development, we also intend to create public community hubs and incubators, which we are tentatively calling “holons”, in several cities around the world. The first holon will be based inside of Bitcoin Decentral in Toronto, and a substantial portion of Ethereum development will take place there; anyone who is seriously interested in participating heavily in Ethereum should consider giving us a visit over the next month. Other cities we are looking into include San Francisco, Amsterdam, Tel Aviv and some city in Asia; this part of the project is still in a very early phase of development, and more details will come over the next month.

最后，为了促进本地社区的发展，我们还打算创建公共社区中心和孵化器，我们暂时称之为“holons”，在全球的几个城市。第一个holon，将在多伦多的Bitcoin Decentral，并将在那里进行大量的以太坊开发。任何对以太坊有浓厚兴趣的人都可考虑下个月去拜访我们。我们正在其他城市，包括旧金山、阿姆斯特丹、特拉维夫以及亚洲的一些城市。项目的这个部分还处于开发的早期阶段，下个月将会有更多的细节。

----------------------------------------------------

#### 区块链中文字幕组

致力于前沿区块链知识和信息的传播，为中国融入全球区块链世界贡献一份力量。

如果您懂一些技术、懂一些英文，欢迎加入我们，加微信号:w1791520555。

[点击查看项目GITHUB，及更多的译文...](https://github.com/BlockchainTranslator/EOS)

#### 本文译者简介

何德林 区块链技术爱好者，热衷于区块链业务创新研究与分析，欢迎加微信号:tongxwl

本文由币乎社区（bihu.com）内容支持计划赞助。

版权所有，转载需完整注明以上内容。

----------------------------------------------------
