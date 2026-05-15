# @parallel/rayon — Data Parallelism for Zeta

Auto-converted from [rayon](https://crates.io/crates/rayon) v1.12.0 / [rayon-core](https://crates.io/crates/rayon-core) v1.13.0 via [Dark Factory](https://github.com/murphsicles/dark-factory).

## Features

| Feature | Description |
|---------|-------------|
| **ParallelIterator** | Map, filter, reduce, fold, zip, chain, flatten, inspect, for_each, find, any, all, position, min/max, sum, product (40+ adapters) |
| **IndexedParallelIterator** | Splittable parallel iterators for slice, Vec, array, range, String |
| **join/scope** | Fork-join parallelism — recursive divide-and-conquer |
| **par_sort** | Parallel quicksort/merge-sort hybrid for slices and Vecs |
| **par_iter** | Automatic parallel iteration for Vec, slice, String, Range, HashMap, HashSet, BTree collections, LinkedList, VecDeque, arrays |
| **ThreadPool** | Configurable work-stealing thread pool with capacity and panic handling |

## Usage
```zeta
use @parallel/rayon::prelude::*;

let sum: i32 = vec![1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
    .par_iter()
    .filter(|x| x > 5)
    .map(|x| x * 2)
    .sum();
```

## Stats: 104 source files, ~17,014 lines across 2 packages, 0 unsupported items

## License
MIT