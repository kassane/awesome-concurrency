## Memory consistency models

- [Memory Barriers: a Hardware View for Software Hackers](http://www.puppetmastertrading.com/images/hwViewForSwHackers.pdf)
- [Memory Models: A Case For Rethinking Parallel Languages and Hardware](https://cacm.acm.org/magazines/2010/8/96610-memory-models-a-case-for-rethinking-parallel-languages-and-hardware/pdf)
- [Go Memory Model](https://golang.org/ref/mem), [Don't be clever](https://golang.org/ref/mem#tmp_1)
- [Java Memory Model](https://docs.oracle.com/javase/specs/jls/se7/html/jls-17.html#jls-17.4)
- [Foundations of the C++ Concurrency Memory Model](http://www.hpl.hp.com/techreports/2008/HPL-2008-56.pdf)
- [Explanation of the Linux-Kernel Memory Consistency Model](https://github.com/torvalds/linux/tree/master/tools/memory-model/Documentation) 
- [The Problem of Programming Language Concurrency Semantics](https://www.cl.cam.ac.uk/~jp622/the_problem_of_programming_language_concurrency_semantics.pdf)
- [Weak memory concurrency in C/C++11](https://youtu.be/mOqu8vGSysc)
- [Weak Memory Consistency](https://people.mpi-sws.org/~viktor/wmc/)
- [Weakly Consistent Concurrency](https://www.cs.tau.ac.il/~orilahav/seminar18/index.html)

## Futures

- [Futures and Promises](http://dist-prog-book.com/chapter/2/futures.html)
- [Your Server as a Function](https://monkey.org/~marius/funsrv.pdf), [Systems Programming at Twitter](https://monkey.org/~marius/talks/twittersystems/#1), [Finagle – Concurrent Programming with Futures](https://twitter.github.io/finagle/guide/Futures.html)
- [Futures for C++11 at Facebook](https://engineering.fb.com/developer-tools/futures-for-c-11-at-facebook/), [Folly Futures](https://github.com/facebook/folly/blob/master/folly/docs/Futures.md), 
- [Zero-cost futures in Rust](http://aturon.github.io/blog/2016/08/11/futures/), [Designing futures for Rust](http://aturon.github.io/blog/2016/09/07/futures-design/), [RFC](https://github.com/rust-lang/rfcs/blob/master/text/2592-futures.md)

## Fibers

- [Project Loom: Fibers and Continuations for the Java Virtual Machine](https://cr.openjdk.java.net/~rpressler/loom/Loom-Proposal.html)
- [State of Loom, Part 1](http://cr.openjdk.java.net/~rpressler/loom/loom/sol1_part1.html), [Part2](http://cr.openjdk.java.net/~rpressler/loom/loom/sol1_part2.html)

## Coroutines

### Stackless
- [Stackless Coroutine in Asio](http://think-async.com/Asio/asio-1.12.2/doc/asio/reference/coroutine.html)
- [On Duff's Device and Coroutines](https://research.swtch.com/duff)

### Assymmetric Transfer
- [Coroutine Theory](https://lewissbaker.github.io/2017/09/25/coroutine-theory)
- [C++ Coroutines: Understanding operator co_await](https://lewissbaker.github.io/2017/11/17/understanding-operator-co-await)
- [C++ Coroutines: Understanding the promise type](https://lewissbaker.github.io/2018/09/05/understanding-the-promise-type)

## Asynchronous Programming

- [Асинхронность в программировании](https://habr.com/ru/company/jugru/blog/446562/)
- [Асинхронность: назад в будущее](https://habr.com/ru/post/201826/)
- [Kotlin Coroutines Proposal](https://github.com/Kotlin/KEEP/blob/master/proposals/coroutines.md)
- [Zero-cost futures in Rust](http://aturon.github.io/blog/2016/08/11/futures/), [Designing futures for Rust](http://aturon.github.io/blog/2016/09/07/futures-design/)

### Async / await

- C#: [Механика asnyc/await в C#](https://habr.com/ru/post/260217/)
- Kotlin: [Coroutines / Implementation details](https://github.com/Kotlin/KEEP/blob/master/proposals/coroutines.md#implementation-details)
- C++: [Understanding operator co_await](https://lewissbaker.github.io/2017/11/17/understanding-operator-co-await), [Understanding the promise type](https://lewissbaker.github.io/2018/09/05/understanding-the-promise-type)

#### Syntax
- [What Color is Your Function?](https://journal.stuffwithstuff.com/2015/02/01/what-color-is-your-function/), [Hacker news](https://news.ycombinator.com/item?id=8984648)
- C#: [Asynchrony in C# 5 Part Six: Whither async?](https://docs.microsoft.com/en-us/archive/blogs/ericlippert/asynchrony-in-c-5-part-six-whither-async)
- Rust: [A final proposal for await syntax](https://boats.gitlab.io/blog/post/await-decision/), [Await Syntax Write Up](https://paper.dropbox.com/doc/Await-Syntax-Write-Up--AcIbhZ1tPTCloXb2fmFpBTt~Ag-t9NlOSeI4RQ8AINsaSSyJ)
- Kotlin: [How do you color your functions?](https://medium.com/@elizarov/how-do-you-color-your-functions-a6bb423d936d)

## Structured Concurrency

* [Notes on structured concurrency, or: Go statement considered harmful](https://vorpus.org/blog/notes-on-structured-concurrency-or-go-statement-considered-harmful/)
* [Roman Elizarov – Structured concurrency](https://medium.com/@elizarov/structured-concurrency-722d765aa952)
* [Structured Concurrency Group](https://trio.discourse.group/c/structured-concurrency), [Resources](https://trio.discourse.group/t/structured-concurrency-resources/21)


## Consistency models for concurrent objects

- [Linearizability: A Correctness Condition for Concurrent Objects ](https://cs.brown.edu/~mph/HerlihyW90/p463-herlihy.pdf)
- [Consistency Models Map](https://jepsen.io/consistency)
- [Linearizability versus Serializability](http://www.bailis.org/blog/linearizability-versus-serializability/)
- [Strong consistency models](https://aphyr.com/posts/313-strong-consistency-models)

## Transactions
 
- [ Martin Kleppmann – Transactions: myths, surprises and opportunities](https://www.youtube.com/watch?v=5ZjhNTM8XU8), [слайды и ссылки](https://martin.kleppmann.com/2015/09/26/transactions-at-strange-loop.html)
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

- [Maurice Herlihy – Transactional Memory](https://www.youtube.com/watch?v=ZkUrl8BZHjk), [слайды](http://neerc.ifmo.ru/sptcc/slides/slides-herlihy.pdf)
- [Gil Tene – Understanding Hardware Transactional Memory](https://www.youtube.com/watch?v=0jy4Sc_IY7o)
- [Is Parallel Programming Hard, And, If So, What Can You Do About It?](https://mirrors.edge.kernel.org/pub/linux/kernel/people/paulmck/perfbook/perfbook.html), 17.3
- [Глава 16 – Programming with Intel Transactional Synchronization Extensions](https://software.intel.com/sites/default/files/managed/39/c5/325462-sdm-vol-1-2abcd-3abcd.pdf)
- [Глава 15 – Intel TSX Recommendations](https://software.intel.com/sites/default/files/managed/9e/bc/64-ia-32-architectures-optimization-manual.pdf)
- [TSX Anti-Patterns](https://software.intel.com/en-us/articles/tsx-anti-patterns-in-lock-elision-code)
- [Lock Elision Implementation Guide](https://sourceware.org/glibc/wiki/LockElisionGuide)
