# The Walker

I begin at the first intersection. The choice feels arbitrary—any starting point will do, the rules say. I mark this place visited in my mind. A small X where I cannot return.

Three paths extend from here. I must choose one.

The rule is simple: walk every intersection exactly once, never returning to any place I've already been. Connect them all in a single unbroken line. If I miss even one intersection, I fail. If I revisit even one intersection, I fail.

The paths do not tell me which choice is correct. They only tell me which directions exist.

I choose left.

---

The second intersection branches into two paths. I've come from one direction—now closed to me by the rule. Two options remain. I choose the path that feels like progress, though I have no evidence this is true.

I mark this intersection visited. Another X behind me, another door that will never open again.

The third intersection has four neighbors. One is where I just came from—forbidden. Three paths remain open.

I'm beginning to understand the shape of the problem. Each step forward closes a space behind me. Each intersection I mark shrinks the available graph. But I don't know if the path I'm building will connect to every remaining intersection. I only know I can't go back.

I choose straight ahead.

---

Seven intersections in, I reach a dead end.

Not a literal wall—there are paths extending from this intersection. But all of them lead to places I've already visited. All of them are forbidden by the rule. I cannot advance. I cannot complete.

This partial path—these seven intersections connected in sequence—is useless. The rule demands all intersections, not most. Partial success is still failure.

I retreat. I unmark the seventh intersection, erasing the X, opening it again for future attempts. I return to the sixth and try a different direction.

That direction also terminates. I retreat to the fifth.

At the fifth, I exhaust all alternative branches. I retreat to the fourth.

The fourth still has unexplored neighbors. I try one. It leads to a different sequence of intersections, but collapses three steps later. I retreat.

I retreat to the third intersection. I try the path I didn't take earlier.

---

I am starting to see the shape of what I'm searching through.

From each intersection, multiple paths branch. Each branch is a hypothesis: "this sequence might reach all intersections." Most hypotheses fail. When they fail, I retreat and try another branch.

But the number of possible sequences is staggering. If there are a handful of intersections, the number of possible orderings in which I might visit them grows faster than I can hold in mind. Each intersection adds more than another choice—it multiplies all previous choices by the number of remaining options.

I am not searching a small space. I am searching something that expands with every intersection added to the graph.

---

Midway through an attempt, I lose track of how many paths I've already tried from the starting intersection. I've retreated so many times that the early branches blur together. Was this sequence one I tested already? Or does it differ in the fourth step?

I keep notes, but the notes themselves become overwhelming. Each failed branch generates a record. The records accumulate. The act of tracking my attempts becomes its own obstacle.

I push forward on the current branch. It reaches fifteen intersections before collapsing. Fifteen Xs, carefully placed. Then the collapse. I retreat, erasing them one by one, searching for the last point where an unexplored option remains.

Most branches collapse earlier. Some collapse after just two or three intersections. But occasionally a branch extends deep—ten, twelve, fifteen intersections—before the available paths run out. These deep branches feel like progress, but they are just expensive failures. The time spent exploring them is time not spent on other branches that might succeed.

I do not know if a solution exists. The rules do not promise one. Some graphs contain a path that visits every intersection exactly once. Some graphs do not. The only way to know is to search.

---

I change starting positions. Maybe the first intersection I chose was wrong. Maybe a solution exists, but only if I begin elsewhere.

From the second intersection, I search. The branches unfold differently, but the pattern is the same: choose, advance, mark, collapse, retreat. The search tree grows and shrivels, grows and shrivels.

From the third intersection, I search. Same pattern. Different failures.

I try every intersection as a starting point. Some branches from some starting points extend farther than others, but none reach completion. Either the graph does not contain a solution, or I have not yet found the correct sequence among the vast number of possible sequences.

I cannot tell which.

---

There is a moment, late in the search, where I realize the scale of what I'm attempting.

If the graph has even a modest number of intersections—say, a few dozen—the number of possible sequences I might need to test is incomprehensibly large. Larger than the number of seconds I have to search. Larger than the number of seconds in a lifetime.

The algorithm is simple: try every possible ordering until one works or all fail. But "all fail" is not a reachable state in any practical sense. I cannot enumerate every possible path. I can only enumerate the paths I have time to check before exhaustion.

The search space is not just large. It is *explosive*. Each additional intersection multiplies the difficulty far beyond the addition of a single extra step.

---

I sit at an intersection I've returned to hundreds of times. This intersection has five neighbors. I've tried building paths from four of them. Each attempt has collapsed somewhere downstream—sometimes immediately, sometimes after extensive branching.

I try the fifth neighbor. It leads to a sequence I haven't fully explored. I advance, marking intersections, choosing paths, branching when necessary.

This sequence reaches eighteen intersections. Farther than most. I feel something almost like hope—maybe this is the branch that works.

The nineteenth intersection has no unvisited neighbors. The path terminates. I've visited eighteen intersections. The graph contains more than eighteen. This is not a solution.

I retreat. I erase the Xs. I return to the eighteenth intersection and try a different direction.

That direction collapses after two steps.

I retreat to the seventeenth.

---

The fatigue is not physical. It is structural. I am tired of branching. Tired of retreating. Tired of erasing marks I placed with care, only to place them differently and erase them again.

The graph does not care about my fatigue. It simply exists, a fixed structure of intersections and paths. The question—does a Hamiltonian path exist?—has a definite answer. Either yes or no. But discovering that answer requires searching a space so large that the distinction between "no solution exists" and "I haven't found it yet" collapses into indistinguishability.

I cannot prove the graph has no solution without exhausting every possible sequence from every possible starting point. I cannot prove it has a solution without finding one.

Verification is easy: if someone hands me a sequence and claims it visits every intersection exactly once, I can check that claim in linear time. Walk the sequence. Count the intersections. Confirm no revisits. Done.

Discovery is hard: finding that sequence in the first place requires searching an exponentially large space of possibilities, most of which lead nowhere.

---

I try a different strategy. Instead of depth-first search—advancing as far as possible before retreating—I try to think ahead. Which branches look promising? Which intersections have fewer neighbors and might become bottlenecks?

This heuristic helps slightly. I eliminate some obviously doomed branches earlier. But it doesn't solve the fundamental problem: I still don't know which sequence works, and I still have to search.

The heuristic reduces the size of the tree I explore, but it doesn't change the worst-case reality: the tree is enormous, and I might need to explore most of it.

---

Hours pass. Days, maybe. Time loses meaning when every moment is another branch, another collapse, another retreat.

I have tried thousands of partial paths. I have backtracked through hundreds of choice points. I have revisited the same intersections from different directions so many times that they blur into abstraction.

Some graphs, I know, have Hamiltonian paths. I've solved smaller ones. With five or six intersections, the search space is manageable. I can enumerate the possibilities by hand, find the solution if it exists, confirm its absence if it doesn't.

But this graph is larger. Not impossibly large—I could write down all the intersections on a single page. But large enough that the search space escapes my grasp.

---

I stop at an intersection I've marked and unmarked dozens of times. I look at the paths extending from it. I know where most of them lead—to sequences I've already tested, to collapses I've already witnessed.

One path remains untested from this position in this configuration. I could try it. It might work. More likely it will collapse like the others.

I stand at the intersection, aware that I have no way to know whether continuing the search will yield a solution or just more failures.

The graph is silent. The intersections do not hint at the answer. The paths do not glow when they're part of the solution. The structure simply exists, indifferent to my effort.

I choose the path. I advance.

Three steps later, it collapses.

I retreat.

---

Somewhere in the space I'm searching, either a solution exists or it doesn't. The answer is fixed, determined by the graph's structure. But I am trapped in the search, unable to exit except through exhaustion or luck.

The rules are simple. The goal is clear. The search is catastrophic.

I mark another intersection. I advance. I prepare to retreat.

The Walker continues, because the Walker does not know how to stop.

---
