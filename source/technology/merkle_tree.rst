.. merkle_tree:

###########
Merkle Tree
###########

Introduction
############

A Merkle tree is a binary tree [link to definition] built using hash pointers [link to definition]. 

Motivation
##########
We want to build a data structure that:

1. Can store lots of data (in our case, **claims**)
2. Makes it easy to prove that some data exists (**proof of membership**)
3. Allows us to check that data hasn't been altered (**tamper resistance**)

It turns out that Merkle trees satisfy these three properties.

Description
###########

Before we take a closer look at the above properties, let's go through how to build a Merkle tree given some data.

Suppose we have a number of blocks containing data. And that these blocks make up the leaves of our tree.

[insert image]

The first step is to group these data blocks into pairs.

[insert image]

Then for each pair of blocks, we build a data structure that has two hash
pointers, one to each block.

[insert image]

In other words, the hash of each block is stored in a parent node. And these parent nodes make up the next level of the tree.

[insert image]

Next, the parent nodes are in turn grouped in pairs, and their hashes stored one level up the tree.

[insert image]

We continue doing this until we reach a single block, the root of the tree.

[insert image]


Tamper resistance
#################

To understand why Merkle trees are tamper resistant, let’s look at what happens if an
adversary wants to tamper with a data block.

If an adversary tampers with some block down here.

[insert image]

That will cause the hash pointer that's one level up to not match.

[insert image]

So she'll have to tamper with that.

[insert image]

Which means, she'll have to tamper with the hash pointer one level up from there.

[insert image]

And so on.

Eventually she'll get up to the top, where she won't be able to tamper with the hash pointer that we've remembered.

[insert image]

Proof of membership
###################

Merkle trees allow us to quickly check membership...

[insert image]

Claims
##############

At iden3 we use Merkle trees to store claims (direct and indirect)...

[insert images]

Definitions
###########

Hash pointers
*************

[insert image]

Binary trees
************

[insert image]
