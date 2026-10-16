# EventFlow – Large-Scale Event Management Platform

A DSA project: an event-management app (admin + user login, events, venues, volunteers, bookings) where each feature is powered by a real algorithm.

## Run
Open `index.html` in a browser (or deploy the folder with GitHub Pages).

- Admin login: `admin` / `admin123`
- User login: `user` / `user123`
- `lab.html` = interactive algorithm lab (24 demos, all six modules)

## Where each algorithm is used
| Module | Algorithm | Feature |
|---|---|---|
| M1 Strings | Aho-Corasick | Multi-keyword event search |
| M1 Strings | KMP | Duplicate event descriptions |
| M1 Strings | Rabin-Karp | Booking code search |
| M1 Strings | Z-Function | Repeated description detection |
| M3 DP | Levenshtein/Damerau | "Did you mean" spell correction |
| M4 Flow | Edmonds-Karp | Venue capacity analysis |
| M4 Flow | Bipartite Matching + König | Volunteer-to-event assignment |
| M5 NP | Vertex-Cover 2-approximation | Schedule conflict resolution |
| M6 Randomized/Parallel | Randomized QuickSort | Event popularity ranking |
| M6 Randomized/Parallel | Reservoir Sampling | Audit draw from registrations |
| M6 Randomized/Parallel | Blelloch Scan / Parallel Reduce | Cumulative registration counts |

All 24 algorithms (suffix structures, bitmask DP, matrix-chain, optimal BST, Dinic, SAT/CLIQUE reductions, Miller-Rabin, Brent's theorem, etc.) run in `lab.html`.

## Note
Front-end only demo. Data is stored in the browser's localStorage; a production version needs a backend and hashed passwords.
