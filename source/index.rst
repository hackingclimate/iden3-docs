
.. image:: ../source/_static/img/iden3-icon2.png
    :scale: 60
    :align: right

|

Iden3 Developer Portal
========================

Welcome to the Iden3 developer portal. Here you'll find eveything you need to get started building with Iden3.

************************************
What is Iden3 and what are its aims
************************************

Iden3 is an open source project offering a complete decentralized identity management solution over the public blockchain. It is designed with four fundamental goals in mind:

**Enable Self Sovereign Identities**, whereby identities are created, owned and controlled by the user.

**Accessibility**, by promoting the development of open standards and ease of use.

**Scalability**, by minimizing the number of accesses to the blockchain that identity management and claim processing requires.   

**Privacy by design** by using Zero Knowledge Proofs to prove claims without revealing any information other than the validity of the claim.

************
Introduction
************

...

**What is an identity and why is it important?**

Identity is a uniquely human concept. It is that ineffable “I” of self-consciousness, something that is understood worldwide by every person living in every culture. As René Descartes said, Cogito ergo sum — I think, therefore I am.

However, modern society has muddled this concept of identity. Today, nations and corporations conflate driver’s licenses, social security cards, and other state-issued credentials with identity; this is problematic because it suggests a person can lose his very identity if a state revokes his credentials or even if he just crosses state borders. I think, but I am not.

Identity in the digital world is even trickier. It suffers from the same problem of centralized control, but it’s simultaneously very balkanized: identities are piecemeal, differing from one Internet domain to another.

As the digital world becomes increasingly important to the physical world, it also presents a new opportunity; it offers the possibility of redefining modern concepts of identity. It might allow us to place identity back under our control — once more reuniting identity with the ineffable “I”.

In recent years, this redefinition of identity has begun to have a new name: self-sovereign identity.
http://www.lifewithalacrity.com/2016/04/the-path-to-self-soverereign-identity.html

**What do we mean by self-sovereign identity?**

To better understand what we mean by self-sovereign, we need to review some history of identity technology...
http://www.lifewithalacrity.com/2016/04/the-path-to-self-soverereign-identity.html



**Why are identity-free games not good enough?**

If one tries to preserve the property of a game being identity-free, building a system where identities don’t matter and only coins do, there is an impossible tradeoff between either failing to incentivize legitimate public goods or over-subsidizing plutocracy.
https://vitalik.ca/general/2019/04/03/collusion.html
 
mechanisms that do not rely on identity cannot solve the problem of concentrated interests outcompeting dispersed communities; an identity-free mechanism that empowers distributed communities cannot avoid over-empowering centralized plutocrats pretending to be distributed communities.
https://vitalik.ca/general/2019/04/03/collusion.html


...

**Why are government/corporate issued identities not good enough?**

as long as an identity consists of a single identifier (like a username or social security number) that will inevitably lead to a big brother.
https://twitter.com/santisiri/status/1128038509338611712

Most of us take for granted that we can prove things about ourselves, unaware that over a billion people cannot. Identity is a prerequisite to financial inclusion, and financial inclusion is a big part of solving poverty
https://medium.com/evernym/7-myths-of-self-sovereign-identity-67aea7416b1

Identity-issuing institutions attempting to disempower marginalized communities by denying them identity documents… (look at the US govnt, Iranian citizens, Github mess...) In a sense Github is an identity issuing institution being forced by the US govnt to disempower Iranian hackers.
https://vitalik.ca/general/2019/04/03/collusion.html

If self-sovereign identity was becoming relevant a few years ago, in light of current international crises its importance has skyrocketed..
http://www.lifewithalacrity.com/2016/04/the-path-to-self-soverereign-identity.html


**Why do we need this vision now?**

Governments and companies are sharing an unprecedented amount of information, cross-correlating everything from viewing habits to purchases, to where people are located during the day, to where they sleep at night, and with whom they associate. 

In addition, as the Third World enters the computer age, digital citizenship is providing Third World residents with greater access to human rights and to the global economy.

When properly designed and implemented, self-sovereign identity can offer these benefits while also protecting individuals from the ever-increasing control of those in power, who may not have the best interests of the individual at heart.
http://www.lifewithalacrity.com/2016/04/the-path-to-self-soverereign-identity.html

**Some use cases**

...

**The dream: Self-sovereign identity --> sybil resistant anonymous voting systems --> liquid democracy**

Historically, liquid democracy has been impossible to implement on a large scale because it is very hard to ensure one person is not voting multiple times. This is called a Sybil attack...

[the key is] to build a decentralized voting protocol that can resist Sybil attacks by requiring some basic verification and reputation for each user while still protecting their pseudo-anonymous identity.

It’s nice to dream of a fair, transparent and corruption-free government, yet this is not something that can happen over night. Government restructuring of this caliber is essentially full on revolution.

Some may call it anarchism, some may call it socialism, and although these are very conflicting ideologies, liquid democracy encompasses a little bit of both.

It doesn’t seem possible the representatives we elect will vote for a law to get rid of representatives; change will have to occur more gradually.

OR

a system like this doesn’t have to restrain itself to national boundaries — it could potentially grow from a small local community into a form of international law built by self-governing internet activists.
https://media.consensys.net/liquid-democracy-and-emerging-governance-models-df8f3ce712af

In Santiago's Siri's words:

...the goal isn’t necessarily to replace President Maduro with someone else. It’s far more radical than that—**the goal is to make the president, any president, irrelevant to the needs and desires of a self-organizing population**...
https://www.wired.com/story/santiago-siri-radical-plan-for-blockchain-voting/?verso=true


having a consensus over identity seems to be a very clear requirement now. it is what will keep voting interesting (money can’t do this). and voting matters specially when there are *big* disagreements.
https://twitter.com/santisiri/status/1117911447235907584

the exercise of digitally voting every ~2 weeks or so in the 
@makerdao blockchain contract to express my political sentiment regarding interest fees as the very utopia i once dreamt for argentina 🇦🇷.
https://twitter.com/santisiri/status/1136275188415389696

 

*******
Layout
*******

This documentation site includes the following sections:

* :doc:`Technology <technology>` : provides a description of iden3's technology.

* :doc:`Developers <developers>` : guide on how to integrate iden3's software for specific applications.

* :doc:`Repository Guide <repositories>` : centralizes documentation scattered across different iden3's repos in a single place. 

* :doc:`Publications <publications>` : includes articles, videos and papers authored by iden3.

During the comming months, we will be sorting, improving and extending the documentation, so don't forget to come back. Thank you!!! 

.. toctree::
   :maxdepth: 1
   :hidden:
   :caption: Technology

   technology

.. toctree::
   :maxdepth: 1
   :hidden:
   :caption: Developers

   developers

.. toctree::
   :maxdepth: 1
   :hidden:
   :caption: Repository Guide

   repositories

.. toctree::
   :maxdepth: 1
   :hidden:
   :caption: Publications

   publications

************
Contributing
************

.. note:: Our team can always use your feedback and help to improve the tutorials and material included. If
          you don't understand something, or cannot find what you are looking for, or have any 
          suggestion, help us make the documentation better by letting us know!

          Submit an issue or pull request on the `GitHub repository
          <https://github.com/iden3/iden3-docs/issues>`_


