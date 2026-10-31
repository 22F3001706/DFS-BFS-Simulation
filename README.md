# Search Stepper

A web page that runs depth-first search (DFS) and breadth-first search (BFS) one line at a time. You can see how the OPEN and CLOSED lists change at every step.

## Open it

Open https://22f3001706.github.io/DFS-BFS-Simulation/ in any browser. No install is needed. An internet connection is only used for fonts.

## Quick start

1. Pick a graph from the **Library** row.
2. Choose **DFS** or **BFS**.
3. Press **Next** to run one step. The highlighted pseudocode line shows what just happened.
4. Watch the lists on the right:
   - **N** is the node just taken off OPEN.
   - **OPEN** holds nodes waiting to be visited. The left end comes out next.
   - **CLOSED** holds nodes already visited.
   - **Visit order** is the sequence of visits so far.

## Controls

| Control | What it does |
|---|---|
| Next / Back | Move one step forward or backward. Arrow keys work too. |
| Play / Pause | Run the steps automatically. Speed is next to it. |
| Reset | Return to step 0. |
| Start / Goal | Choose where the search begins and, optionally, where it stops. |
| MoveGen order | Sets the order in which neighbours are returned: A to Z, Z to A, or shuffled. |
| Keep a CLOSED list | On: visited nodes are never added again. Off: every neighbour is added, so the search can loop. |

## Predict mode

1. Tick **Predict mode**.
2. After a node is visited, the page shows what MoveGen returns for it.
3. Click the node you think is popped next, on the graph or in OPEN.
4. A wrong guess gives a hint. **Reveal answer** shows the result.

## Check a visit order

Use **Could this be the visit order?** at the bottom of the page.

1. Type the nodes in order, for example `K E A E A`.
2. Leave **Start node is already visited** ticked if your list begins after the start node.
3. Choose how MoveGen behaves:
   - **Same order on every call**: a real function that repeats its answer.
   - **Any order on each call**: it may answer differently each time.
4. Read the result. If the order is impossible, the page shows where it breaks.

The check uses the algorithm, start node and CLOSED setting from the controls at the top.

## Tips

- Turn the CLOSED list off on the exam graph (start J, DFS) to see the search bounce between two nodes.
- On the "Short and long route" graph, switch the MoveGen order and compare DFS with BFS.
