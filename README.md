# Awesome Concurrency

# Sub-lists

- [Libraries](libs.md)

---

## Memory consistency models

- [Atomic vs. Non-Atomic Operations](https://preshing.com/20130618/atomic-vs-non-atomic-operations/)
- [Atomic reference counting (with Zig code samples)](https://ravendb.net/articles/atomic-reference-counting-with-zig-code-samples)
- [Memory Barriers: a Hardware View for Software Hackers](http://www.puppetmastertrading.com/images/hwViewForSwHackers.pdf)
- [Memory Models: A Case For Rethinking Parallel Languages and Hardware](https://cacm.acm.org/magazines/2010/8/96610-memory-models-a-case-for-rethinking-parallel-languages-and-hardware/pdf)
- [Java Memory Model](https://docs.oracle.com/javase/specs/jls/se7/html/jls-17.html#jls-17.4)
- [Foundations of the C++ Concurrency Memory Model](http://www.hpl.hp.com/techreports/2008/HPL-2008-56.pdf)
- [Explanation of the Linux-Kernel Memory Consistency Model](https://github.com/torvalds/linux/tree/master/tools/memory-model/Documentation)
  - [Frightening Small Children and Disconcerting Grown-ups: Concurrency in the Linux Kernel](http://pauillac.inria.fr/~maranget/papers/asplos2018.pdf)
- [Memory Models](https://research.swtch.com/mm) by [Russ Cox](https://research.swtch.com/)
  - [Hardware MM](https://research.swtch.com/hwmm)
  - [Programming Language MM](https://research.swtch.com/plmm)
  - [Updating the Go MM](https://research.swtch.com/gomm)
- [Repairing Sequential Consistency in C/C++11](https://plv.mpi-sws.org/scfix/paper.pdf) + [P0668R5: Revising the C++ memory model](https://www.open-std.org/jtc1/sc22/wg21/docs/papers/2018/p0668r5.html)
- [A Promising Semantics for Relaxed-Memory Concurrency](https://sf.snu.ac.kr/promise-concurrency/)
- [Bounding Data Races in Space and Time](https://kcsrk.info/papers/pldi18-memory.pdf) + [Multicore OCaml Memory model](https://v2.ocaml.org/manual/memorymodel.html)
- [C++ Memory Ordering at Compile Time](https://preshing.com/20120625/memory-ordering-at-compile-time/)
- [The Problem of Programming Language Concurrency Semantics](https://www.cl.cam.ac.uk/~jp622/the_problem_of_programming_language_concurrency_semantics.pdf)
- [Understandnig Atomics and Memory Ordering](http://kprotty.me/2021/04/08/understanding-atomics-and-memory-ordering.html)
- [Weak memory concurrency in C/C++11](https://youtu.be/mOqu8vGSysc)
- [Weak Memory Consistency](https://people.mpi-sws.org/~viktor/wmc/)
- [Weakly Consistent Concurrency](https://www.cs.tau.ac.il/~orilahav/seminar18/index.html)
- [Memory Order in C++](https://www.sobyte.net/post/2022-06/cpp-memory-order/)
- [Atomics And Concurrency](https://redixhumayun.github.io/systems/2024/01/03/atomics-and-concurrency.html)
- [A Relaxed Guide to memory_order_relaxed - by Paul McKenney & Hans Boehm](https://www.youtube.com/watch?v=cWkUqK71DZ0)

### Examples

#### C++

- [`intro.multithread`](https://eel.is/c++draft/intro.multithread)
- [`atomics.order`](https://eel.is/c++draft/atomics.order)
- [`atomics.fences`](https://eel.is/c++draft/atomics.fences)
- [`std::memory_order`](https://en.cppreference.com/w/cpp/atomic/memory_order)
- [C++ reference - Memory Model](https://en.cppreference.com/w/cpp/language/memory_model)

[Index](cpp-mm-index.md)

#### Rust

- [The Rust Reference / Memory model](https://doc.rust-lang.org/reference/memory-model.html)
- [The Rustonomicon / Atomics](https://doc.rust-lang.org/nomicon/atomics.html)

#### Java 

- [Java Memory Model](https://docs.oracle.com/javase/specs/jls/se7/html/jls-17.html#jls-17.4)

#### Go

- [Go Memory Model](https://golang.org/ref/mem)
- [Don't be clever](https://golang.org/ref/mem#tmp_1)

#### D

- [D Memory Model](https://dlang.org/spec/intro.html#memory-model)
- [D Wiki - C++ to D Concurrency](https://wiki.dlang.org/Programming_in_D_for_C%2B%2B_Programmers#Concurrency)

#### LLVM

- [LLVM Atomic Instructions and Concurrency Guide](https://llvm.org/docs/Atomics.html)

### Atomics impl

- [C/C++11 mappings to processors](https://www.cl.cam.ac.uk/~pes20/cpp/cpp0xmappings.html)
- [The JSR-133 Cookbook for Compiler Writers](http://gee.cs.oswego.edu/dl/jmm/cookbook.html)

----

## Futures

- [Futures and Promises](http://dist-prog-book.com/chapter/2/futures.html)
- [Your Server as a Function](https://monkey.org/~marius/funsrv.pdf), [Systems Programming at Twitter](https://monkey.org/~marius/talks/twittersystems/#1), [Finagle – Concurrent Programming with Futures](https://twitter.github.io/finagle/guide/Futures.html)
- [Futures for C++11 at Facebook](https://engineering.fb.com/developer-tools/futures-for-c-11-at-facebook/), [Folly Futures](https://github.com/facebook/folly/blob/master/folly/docs/Futures.md), 
- [Zero-cost futures in Rust](http://aturon.github.io/blog/2016/08/11/futures/), [Designing futures for Rust](http://aturon.github.io/blog/2016/09/07/futures-design/), [RFC](https://github.com/rust-lang/rfcs/blob/master/text/2592-futures.md)

## Fibers

- [Fibers in C++: Understanding the basics](https://agraphicsguynotes.com/posts/fiber_in_cpp_understanding_the_basics/)
- [Fibers, Oh My!](https://graphitemaster.github.io/fibers/)
- [Project Loom: Fibers and Continuations for the Java Virtual Machine](https://cr.openjdk.java.net/~rpressler/loom/Loom-Proposal.html)
- [State of Loom, Part 1](http://cr.openjdk.java.net/~rpressler/loom/loom/sol1_part1.html), [Part 2](http://cr.openjdk.java.net/~rpressler/loom/loom/sol1_part2.html)
- [C++ / Distinguishing coroutines and fibers](https://wg21.link/n4024)
- [C++ / Fibers under the magnifying glass](https://wg21.link/p1364)
- [Lightweight concurrency in lua](https://wingolog.org/archives/2018/05/16/lightweight-concurrency-in-lua)
- [D - Fibers](http://ddili.org/ders/d.en/fibers.html)

## Coroutines

### Stackless
- [Stackless Coroutine in Asio](http://think-async.com/Asio/asio-1.28.0/doc/asio/reference/coroutine.html)
- [On Duff's Device and Coroutines](https://research.swtch.com/duff)

### Assymmetric Transfer
- [Coroutine Theory](https://lewissbaker.github.io/2017/09/25/coroutine-theory)
- [Writing custom C++20 coroutine systems](https://www.chiark.greenend.org.uk/~sgtatham/quasiblog/coroutines-c++20/)
- [Revisiting Coroutines by Ana Lúcia de Moura and Roberto Ierusalimschy](http://www.inf.puc-rio.br/~roberto/docs/MCC15-04.pdf)

## Stacks

- [Segmented Stacks in LLVM](https://llvm.org/docs/SegmentedStacks.html)
- [Rust / Abandoning segmented stacks in Rust](https://mail.mozilla.org/pipermail/rust-dev/2013-November/006314.html)
- [Go / How Stacks are Handled in Go](https://blog.cloudflare.com/how-stacks-are-handled-in-go/), [Continious Stacks Design Doc](https://docs.google.com/document/d/1wAaf1rYoM4S4gtnPh0zOlGzWtrZFQ5suE8qr2sD8uWQ/pub)
- [Rust / Futures and Segmented Stacks](https://without.boats/blog/futures-and-segmented-stacks/)
- [Continuation Passing for C - A space-efficient implementation of concurrency](https://www.irif.fr/~jch/cpc.pdf)
- [C++ / call/cc (call-with-current-continuation): A low-level API for stackful context switching](https://www.open-std.org/jtc1/sc22/wg21/docs/papers/2017/p0534r3.pdf)

## Schedulers

- [Making the Tokio scheduler 10x faster](https://tokio.rs/blog/2019-10-scheduler/)
- [Rust / Work-Stealing Scheduler Discussion](https://github.com/rust-lang/rust/issues/3095)
- [Scalable Go Scheduler Design Doc](https://docs.google.com/document/d/1TTj4T2JO42uD5ID9e89oa0sLKhJYD0Y_kqxDv3I3XMw/edit)
- [Dmitry Vyukov — Go scheduler: Implementing language with lightweight concurrency](https://www.youtube.com/watch?v=-K11rY57K7k)
- [GopherCon 2020: Austin Clements - Pardon the Interruption: Loop Preemption in Go 1.14](https://www.youtube.com/watch?v=1I1WmeSjRSw)
- ["Runtime scheduling: theory and reality" by Eben Freeman](https://www.youtube.com/watch?v=8g9fG7cApbc)

### Impls

- [Golang] [Runtime](https://golang.org/src/runtime/proc.go)
- [Rust] [Tokio Multi-Threaded Runtime](https://github.com/tokio-rs/tokio/blob/master/tokio/src/runtime/scheduler/multi_thread/worker.rs)
- [Dlang] [Phobos - Multiple Declarations](https://github.com/dlang/phobos/blob/master/std/concurrency.d#L1287)
- [Kotlin] [Coroutine Runtime](https://github.com/Kotlin/kotlinx.coroutines/blob/master/kotlinx-coroutines-core/jvm/src/scheduling/CoroutineScheduler.kt)
- [Scala] [Cats Effect](https://github.com/typelevel/cats-effect/blob/series/3.x/core/jvm/src/main/scala/cats/effect/unsafe/WorkStealingThreadPool.scala)

## Channels

- [Go channels on steroids](https://docs.google.com/document/d/1yIAYmbvL3JxOKOjuCyon7JhW4cSv1wy5hC0ApeGMV9s/pub)
- [Scalable FIFO Channels for Programming via Communicating Sequential Processes](https://nkoval.com/publications/europar19-channels.pdf)
- [Fast and Scalable Channels in Kotlin Coroutines](https://arxiv.org/pdf/2211.04986.pdf)

## Asynchronous Programming

- [Асинхронность в программировании](https://habr.com/ru/company/jugru/blog/446562/)
- [Асинхронность: назад в будущее](https://habr.com/ru/post/201826/)
- [Kotlin Coroutines Proposal](https://github.com/Kotlin/KEEP/blob/master/proposals/coroutines.md)
- [Zero-cost futures in Rust](http://aturon.github.io/blog/2016/08/11/futures/), [Designing futures for Rust](http://aturon.github.io/blog/2016/09/07/futures-design/)

### Async / await

- C#: [Механика asnyc/await в C#](https://habr.com/ru/post/260217/)
- Kotlin: [Coroutines / Implementation details](https://github.com/Kotlin/KEEP/blob/master/proposals/coroutines.md#implementation-details)
- C++:
  - [Understanding operator co_await](https://lewissbaker.github.io/2017/11/17/understanding-operator-co-await)
  - [Understanding the promise type](https://lewissbaker.github.io/2018/09/05/understanding-the-promise-type)
  - [Understanding the Compiler Transform](https://lewissbaker.github.io/2022/08/27/understanding-the-compiler-transform)
  - [Understanding Symmetric Transfer](https://lewissbaker.github.io/2020/05/11/understanding_symmetric_transfer)

#### Syntax
- [What Color is Your Function?](https://journal.stuffwithstuff.com/2015/02/01/what-color-is-your-function/), [Hacker news](https://news.ycombinator.com/item?id=8984648)
- C#: [Asynchrony in C# 5 Part Six: Whither async?](https://docs.microsoft.com/en-us/archive/blogs/ericlippert/asynchrony-in-c-5-part-six-whither-async)
- Rust: [A final proposal for await syntax](https://boats.gitlab.io/blog/post/await-decision/), [Await Syntax Write Up](https://paper.dropbox.com/doc/Await-Syntax-Write-Up--AcIbhZ1tPTCloXb2fmFpBTt~Ag-t9NlOSeI4RQ8AINsaSSyJ)
- Kotlin: [How do you color your functions?](https://medium.com/@elizarov/how-do-you-color-your-functions-a6bb423d936d)
- Zig: [What is Zig's “Colorblind” Async/Await?](https://kristoff.it/blog/zig-colorblind-async-await/)

## Structured Concurrency

- [Notes on structured concurrency, or: Go statement considered harmful](https://vorpus.org/blog/notes-on-structured-concurrency-or-go-statement-considered-harmful/)
- [Structured Concurrency Group](https://trio.discourse.group/c/structured-concurrency), [Resources](https://trio.discourse.group/t/structured-concurrency-resources/21)
- [Roman Elizarov – Structured concurrency](https://medium.com/@elizarov/structured-concurrency-722d765aa952)
- [Lewis Baker – Structured Concurrency: Writing Safer Concurrent Code with Coroutines and Algorithms](https://www.youtube.com/watch?v=1Wy5sq3s2rg)
- [Eric Niebler – Structured Concurrency](https://ericniebler.com/2020/11/08/structured-concurrency/)
- [Josua Wuyts - Tree-Structured Concurrency](https://blog.yoshuawuyts.com/tree-structured-concurrency/)
- [Sebastiaan Koppe - Structured Concurrency in D(Video)](https://youtu.be/hJhNhIeq29U)

## Cancellation

- [Timeouts and cancellation for humans](https://vorpus.org/blog/timeouts-and-cancellation-for-humans/#cancel-scopes-trio-s-human-friendly-solution-for-timeouts-and-cancellation)

## Data race detection

- [ThreadSanitizer – data race detection in practice](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/35604.pdf), [compiler-rt/lib/tsan/rtl](https://github.com/llvm-mirror/compiler-rt/tree/master/lib/tsan/rtl)
- [FastTrack: Efficient and Precise Dynamic Race Detection](https://users.soe.ucsc.edu/~cormac/papers/pldi09.pdf)

## Verification

- [Dynamic Partial-Order Reduction for Model Checking Software](https://patricegodefroid.github.io/public_psfiles/popl2005.pdf)
- [Finding and Reproducing Heisenbugs in Concurrent Programs](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/osdi2008-CHESS.pdf)
- [CDSCHECKER: Checking Concurrent Data Structures Written with C/C++ Atomics](http://demsky.eecs.uci.edu/publications/c11modelcheck.pdf)
- [How We Test Concurrent Primitives in Kotlin Coroutines](https://blog.jetbrains.com/kotlin/2021/02/how-we-test-concurrent-primitives-in-kotlin-coroutines/)

### Tools

- Rust: [Loom - concurrency permutation testing](https://github.com/tokio-rs/loom)
- Kotlin: [Lincheck - framework for testing concurrent](https://github.com/Kotlin/kotlinx-lincheck)

## Fearless Concurrency

- Rust: [Fearless Concurrency](https://doc.rust-lang.org/book/ch16-00-concurrency.html)
- Pony: [Reference capabilities](https://www.ponylang.io/learn/#reference-capabilities)
- C++: [Clang Thread-Safety Analysis](https://research.google.com/pubs/archive/42958.pdf)
- D: [Fearless - Safe Concurrency in D](https://atilaoncode.blog/2018/11/06/implementing-rusts-stdsyncmutex-in-d/)
- [Joe Duffy (Project Midori) – 15 Years of Concurrency](http://joeduffyblog.com/2016/11/30/15-years-of-concurrency/)

---

## Consistency models for concurrent objects

- [Linearizability: A Correctness Condition for Concurrent Objects ](https://cs.brown.edu/~mph/HerlihyW90/p463-herlihy.pdf)
- [Consistency Models Map](https://jepsen.io/consistency)
- [Linearizability versus Serializability](http://www.bailis.org/blog/linearizability-versus-serializability/)
- [Strong consistency models](https://aphyr.com/posts/313-strong-consistency-models)

---

## Lock-freedom

### Data Structures / Algorithms

- [Simple, Fast, and Practical Non-Blocking and Blocking Concurrent Queue Algorithms](https://www.cs.rochester.edu/~scott/papers/1996_PODC_queues.pdf)
- [A Scalable Lock-free Stack Algorithm](https://people.csail.mit.edu/shanir/publications/Lock_Free.pdf)
- [The Baskets Queue](https://people.csail.mit.edu/shanir/publications/Baskets%20Queue.pdf)
- [Lock-free deques and doubly linked lists](http://www.cse.chalmers.se/~tsigas/papers/Lock-Free-Deques-Doubly-Lists-JPDC.pdf)
- [A Practical Multi-Word Compare-and-Swap Operation](https://www.cl.cam.ac.uk/research/srg/netos/papers/2002-casn.pdf)

### Memory Management

- [Hazard Pointers: Safe Memory Reclamation for Lock-Free Objects](https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.395.378&rep=rep1&type=pdf)
- [Epoch-Based Memory Reclamation](http://csng.cs.toronto.edu/publication_files/0000/0159/jpdc07.pdf)
- [Differential Reference Counting](http://www.1024cores.net/home/lock-free-algorithms/object-life-time-management/differential-reference-counting)
- [Implementing a Lock-free `atomic_shared_ptr`](https://github.com/brycelelbach/cppnow_presentations_2016/blob/master/01_wednesday/implementing_a_lock_free_atomic_shared_ptr.pdf)
- [folly / `AtomicSharedPtr`](https://github.com/facebook/folly/blob/master/folly/concurrency/AtomicSharedPtr.h)
- [Automem Hands Free RAII in D](https://dlang.org/blog/2017/04/28/automem-hands-free-raii-for-d/)

### Misc

- [Roman Elizarov — Lock-Free Algorithms for Kotlin Coroutines](https://www.youtube.com/watch?v=W2dOOBN1OQI)
- [Lock-free структуры данных](https://habr.com/en/post/195770/)
- [LockFree Programming a_Mental Model - Xorvoid](https://xorvoid.com/lockfree_programming_a_mental_model.html)
- [Zig's I/O and Concurrency Story by King Protty](https://www.youtube.com/watch?v=Ul8OO4vQMTw) [Video]
- [CppCon 2016 - "Elegant Asynchronous Code" by Nat Goodspeed](https://www.youtube.com/watch?v=e-NUmyBou8Q) [Video]

---

## Transactions
 
- [ Martin Kleppmann – Transactions: myths, surprises and opportunities](https://www.youtube.com/watch?v=5ZjhNTM8XU8), [slides & references](https://martin.kleppmann.com/2015/09/26/transactions-at-strange-loop.html)
- [A Critique of ANSI SQL Isolation Levels](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/tr-95-51.pdf)
- [Serializable Isolation for Snapshot Databases](https://ses.library.usyd.edu.au/bitstream/2123/5353/1/michael-cahill-2009-thesis.pdf)
- [What Write Skew Looks Like](https://www.cockroachlabs.com/blog/what-write-skew-looks-like/)
- [A Read-Only Transaction Anomaly Under Snapshot Isolation](https://www.cs.umb.edu/~poneil/ROAnom.pdf)
- [Google Percolator](https://storage.googleapis.com/pub-tools-public-publication-data/pdf/36726.pdf)
- [Serializable Snapshot Isolation in PostgreSQL](https://drkp.net/papers/ssi-vldb12.pdf)
- [PostgreSQL SSI Implementation Notes](https://github.com/postgres/postgres/blob/master/src/backend/storage/lmgr/README-SSI)
- [A History of Transaction Histories](https://ristret.com/s/f643zk/history_transaction_histories) 

#### Demystifying Database Systems
- [An Introduction to Transaction Isolation Levels](https://fauna.com/blog/introduction-to-transaction-isolation-levels)
- [Correctness Anomalies Under Serializable Isolation](https://fauna.com/blog/demystifying-database-systems-correctness-anomalies-under-serializable-isolation)
- [Introduction to Consistency Levels](https://fauna.com/blog/demystifying-database-systems-introduction-to-consistency-levels) 
- [Isolation levels vs. Consistency levels](https://fauna.com/blog/demystifying-database-systems-part-4-isolation-levels-vs-consistency-levels)

## Hardware Transactional Memory
- [Maurice Herlihy – Transactional Memory](https://www.youtube.com/watch?v=ZkUrl8BZHjk), [slides](http://neerc.ifmo.ru/sptcc/slides/slides-herlihy.pdf)
- [Gil Tene – Understanding Hardware Transactional Memory](https://www.youtube.com/watch?v=0jy4Sc_IY7o)
- [Is Parallel Programming Hard, And, If So, What Can You Do About It?](https://mirrors.edge.kernel.org/pub/linux/kernel/people/paulmck/perfbook/perfbook.html), 17.3
- [Глава 16 – Programming with Intel Transactional Synchronization Extensions](https://software.intel.com/sites/default/files/managed/39/c5/325462-sdm-vol-1-2abcd-3abcd.pdf)
- [Глава 15 – Intel TSX Recommendations](https://software.intel.com/sites/default/files/managed/9e/bc/64-ia-32-architectures-optimization-manual.pdf)
- [TSX Anti-Patterns](https://software.intel.com/en-us/articles/tsx-anti-patterns-in-lock-elision-code)
- [Lock Elision Implementation Guide](https://sourceware.org/glibc/wiki/LockElisionGuide)

## Software Transactional Memory

- [D] [Software Transactional Memory in D (Video)](https://www.youtube.com/watch?v=2P3OUuBEBNc) by Brad Roberts
- [C++] [CppCon 2015 - “Transactional Memory in Practice"](https://www.youtube.com/watch?v=k20nWb9fHj0) by Brett Hall
- [Scala, ZIO] [Introduction to Software Transactional Memory](https://zio.dev/reference/stm/)
- [A (brief) retrospective on transactional memory](https://joeduffyblog.com/2010/01/03/a-brief-retrospective-on-transactional-memory/) by Joe Duffy

## IO
- [Lord of io_uring](https://unixism.net/loti/)
- [A Universal I/O Abstraction for C++](https://cor3ntin.github.io/posts/iouring/#reactors-select-poll-epoll)
- [A Programmer-Friendly I/O Abstraction Over io_uring and kqueue](https://tigerbeetle.com/blog/a-friendly-abstraction-over-iouring-and-kqueue/)

---

## Acknowledgments

**Author:** [Roman Lipovsky](https://gitlab.com/Lipovsky)
Original repository: [from Gitlab - Awesome-Concurrency](https://gitlab.com/Lipovsky/awesome-concurrency)
