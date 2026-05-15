# @parallel/rayon — Data Parallelism for Zeta

Auto-converted from [rayon](https://crates.io/crates/rayon) v1.12.0 via [Dark Factory](https://github.com/murphsicles/dark-factory).

## Usage
```zeta
use @parallel/rayon::prelude::*;

fn main() {
    let mut v = vec![1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
    v.par_iter().for_each(|x| println("{}", x));
}
```

## Components
- **rayon** (1.12.0): ParallelIterator, IndexedParallelIterator, join, scope, par_iter, par_sort
- **rayon-core** (1.13.0): ThreadPool, Registry, work-stealing thread pool

## Stats
- ~18,125 lines of Zeta total across both packages
- 0 unsupported items
