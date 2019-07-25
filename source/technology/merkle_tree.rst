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
2. Allows us to efficiently prove that some data exists (**proof of membership**)
3. Allows us to check that data hasn't been altered (**tamper resistance**)

It turns out that Merkle trees satisfy these three properties.

Description
###########

Before we take a closer look at these three properties, let's go through how to build a Merkle tree.

Suppose we have a number of blocks containing data. And that these blocks make up the leaves of our tree.

The first step is to group these data blocks into pairs.

Then for each pair of blocks, we build a data structure that has two hash
pointers, one to each block. In other words, the hash of each block is stored in a parent node -- these parent nodes make up the next level of the tree.

Next, the parent nodes are grouped in pairs. And their hashes are in turn stored one level up the tree.

We continue doing this until we reach a single block, the root of the tree.

If you're having trouble visualizing this, don't worry. An image should help.

[insert image]

Tamper resistance
#################

To understand why Merkle trees are tamper resistant, let’s look at what happens if an
adversary wants to tamper with a data block...

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
