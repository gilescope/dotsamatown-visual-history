## Chapter 3: Play with time

So far we have always been hooking up to the live blockchain visualising what is happening right now. We want to be able to also go back to any point in time ideally and replay history.

But to start with you have to break everything so we're back to square one:

![broken](chapter3/Screenshot%20from%202022-05-22%2013-22-57.png)

After a bit of toil, managed to get one relay chain working for one point in history:
![relay-point-in-time](chapter3/Screenshot%20from%202022-05-24%2010-30-43.png)

And then finally the parachains - but this time we're being driven by the data on the relay chain as to what parachain blocks to display:
![parachains-in-time](chapter3/Screenshot%20from%202022-05-26%2007-42-37.png)

So far so good and starting to look pretty again:
![pretty-good](chapter3/Screenshot%20from%202022-05-29%2007-05-21.png)

Ah realise that the atmosphere is interfearing with the rainbows leading to rendering grayness at certain depths. Bug be banished!
![bug-banishd](chapter3/Screenshot%20from%202022-05-29%2007-09-49.png)

For quite a while I wanted to have Kusama's own style start to shine through. And so we have some initial dark side of Kusama showing it's true colors. We have also started spacing out the blocks on the x-axis based on the timestamps extrinsic in the blocks.
![darkside](chapter3/Screenshot%20from%202022-06-03%2016-21-36.png)

On the UI you can select any block number (say 1,000,000), but it would display the millionth block on both Kusama and Polkadot, but these are far away in time. Have changed the code so that it will map the block number to the timestamp and then find the corresponding timestamp on the other relay chain:
![truetime](chapter3/Screenshot%20from%202022-06-04%2019-36-54.png)



























0