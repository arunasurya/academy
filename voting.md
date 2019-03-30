# Voting

## Introduction
- Any stakeholder (BSQ holder) can vote, including on their own proposals.
- Your voting weight is determined by the amount of BSQ you use as your stake. 
- That amount is locked until the end of the voting period. 
- You need to pay a voting fee to participate.

## Voting Cycle
The voting cycle consists of four phases: the proposal phase, blind vote, vote reveal and vote result. Each voting cycle lasts a total of 4380 Bitcoin blocks which amounts to about 30 days. A stakeholder participating in each phase of the voting cycle creates three [Bisq DAO transactions](bisqdaotx.md). 

### Proposal Phase
During the proposal phase, which lasts 3630 blocks (~25 days), various proposals such as compensation requests, asset listing proposals, proposals to remove a fee and others can be made by any stakeholder. A participating stakeholder needs to pay a proposal fee for creating each proposal. This is done to discourage malicious or careless proposal making that can overwhelm [the Bisq network](bisqp2p.md).

### Blind Vote 
The blind vote phase lasts 450 blocks or about three days. Any stakeholder can vote on any proposal including their own. You can upvote, downvote or decide not to vote on a proposal. The latter is encouraged if you are not acquained with a specific proposal. 

Each vote is encrypted so that those who have voted earlier in the cycle do not influence those who join later. The encrypted vote is transmitted to the Bisq network. After receiving the encrypted vote, the participating nodes check if there is a Bitcoin transaction that corresponds to that Bisq DAO transaction. Once you have voted, you cannot change your vote since any change will result in a significant change in the encrypted message. This is to ensure that the voters commited to their votes. The Bisq sofware collects all the voting data in a block, hashes it and publishes the hash to all the other nodes.

### Vote Reveal
The vote reveal phase lasts 300 blocks or about two days. In the vote reveal phase, the nodes collect all the valid encrypted votes they got in the previous phase into a block and publish the hash of this block (along with their own decryption key) on the Bitcoin blockchain. The nodes compare that hash with their own hash to check if they had received all the votes. All the nodes participating in that voting cycle need to be online to reveal their votes. 

### Vote Result
In the vote result phase, the participaing nodes check what the "winning" block is (the one whose hash was put most often in the blockchain in the Vote Reveal phase), and make sure they got all the data needed to build this block. Then they use this block and the decryption keys to calculate the vote results.

If there is a disparity between the hash produced by your node and that of the other nodes, the hash of the node that has used the largest BSQ stake in the voting cycle will be given priority.

