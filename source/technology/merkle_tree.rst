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

1. Can store a lot of data (**claims**)
2. Allows us to efficiently prove that some data exists (**proof of membership**)
3. Allows us to check that data hasn't been altered (**tamper resistance**)

It turns out that Merkle trees satisfy these three properties.

Description
###########

Suppose we have a number of blocks containing data. And that these blocks make up the leaves of our tree.

We group these data blocks into pairs, and then for each pair, build a data structure that has two hash
pointers, one to each block.

These data structures make up the next level of the tree.

We then group these hash pointers into groups of two, and for each pair, create a new data structure that contains the hash of each.

We continue doing this until we reach a single block, the root of the tree.

Don't worry if you're having trouble visualizing this. It's much easier to see with an image.

[insert image]

Image caption: In a Merkle tree, data blocks are grouped in pairs and the hash of each of
these blocks is stored in a parent node. The parent nodes are in turn grouped in pairs and their hashes
stored one level up the tree. This continues all the way up the tree until we reach the root node.

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
