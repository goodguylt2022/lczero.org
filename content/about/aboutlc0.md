---
title: "About Lc0"
draft: false
weight: 100
---

Lc0 is often referred to as a chess engine, however, Lc0 is more like a chess engine *shell* than an actual chess engine. This is often called "the binary".
Lc0 needs a *neural network* (also called a "weights file") in order to play, just as a car requires a driver, or a mech requires a pilot.

A more detailed explanation of what Lc0 is and how it works can be found in the old [GitHub Wiki](https://github.com/LeelaChessZero/lc0/wiki/Technical-Explanation-of-Leela-Chess-Zero)

In other words, Lc0 is a robot body with eyes to see the pieces and hands to move them, and the neural network is the brain of the robot that chooses the best move.

Lc0 (the shell) tells the network (the brain) where the pieces are and what the possible moves are. The network then figures out which moves are most likely to win the game. If a move looks good, the network will look at the moves that might come after it to figure out if it really is the best move. If it isn't, it will start looking at a different, better looking move.

But this requires that the network knows what a good looking move even is. A completely new untrained network has no idea what moves are good and will choose seemingly random moves. But a trained network that has seen billions of games will know what a good move looks like and will generally choose a great, or the best, move, which Lc0 will then play.

With a weak network, Lc0 can play as poorly as a toddler, and with a strong network, Lc0 can beat even the strongest existing chess engines (assuming you have a good enough GPU).

And so, if you wish to use Lc0, you need to download both Lc0 *and* a network to drive it. To get started, you can follow [the instructions found here](https://lczero.org/play/quickstart/).

There are also different network sizes. The bigger networks are smarter but slower, and the smaller networks aren't as smart but are much faster. So if Lc0 is playing a bullet game, then you might want to use a smaller net which can think faster. However if you are using Lc0 to analyze a position, and don't really care about the time it takes to analyze it, then you'll want a bigger and smarter network.

All the best networks are available [here](https://lczero.org/play/networks/bestnets/)

More information about networks can be found [here](https://lczero.org/play/networks/)
