### InnoDB

```
mysql> SHOW ENGINE INNODB STATUS\G;
*************************** 1. row ***************************
  Type: InnoDB
  Name:
Status:
=====================================
2022-02-14 09:43:39 140012787037952 INNODB MONITOR OUTPUT
=====================================
Per second averages calculated from the last 18 seconds
-----------------
BACKGROUND THREAD
-----------------
srv_master_thread loops: 113 srv_active, 0 srv_shutdown, 285258 srv_idle
srv_master_thread log flush and writes: 0
----------
SEMAPHORES
----------
OS WAIT ARRAY INFO: reservation count 55952
OS WAIT ARRAY INFO: signal count 58812
RW-shared spins 0, rounds 0, OS waits 0
RW-excl spins 0, rounds 0, OS waits 0
RW-sx spins 0, rounds 0, OS waits 0
Spin rounds per wait: 0.00 RW-shared, 0.00 RW-excl, 0.00 RW-sx
------------
TRANSACTIONS
------------
Trx id counter 1942
Purge done for trx's n:o < 1936 undo n:o < 0 state: running but idle
History list length 0
LIST OF TRANSACTIONS FOR EACH SESSION:
---TRANSACTION 421487916481752, not started
0 lock struct(s), heap size 1128, 0 row lock(s)
---TRANSACTION 421487916480944, not started
0 lock struct(s), heap size 1128, 0 row lock(s)
---TRANSACTION 421487916480136, not started
0 lock struct(s), heap size 1128, 0 row lock(s)
--------
FILE I/O
--------
I/O thread 0 state: waiting for i/o request (insert buffer thread)
I/O thread 1 state: waiting for i/o request (log thread)
I/O thread 2 state: waiting for i/o request (read thread)
I/O thread 3 state: waiting for i/o request (read thread)
I/O thread 4 state: waiting for i/o request (read thread)
I/O thread 5 state: waiting for i/o request (read thread)
I/O thread 6 state: waiting for i/o request (write thread)
I/O thread 7 state: waiting for i/o request (write thread)
I/O thread 8 state: waiting for i/o request (write thread)
I/O thread 9 state: waiting for i/o request (write thread)
Pending normal aio reads: [0, 0, 0, 0] , aio writes: [0, 0, 0, 0] ,
 ibuf aio reads:, log i/o's:, sync i/o's:
Pending flushes (fsync) log: 0; buffer pool: 0
3769212 OS file reads, 604639 OS file writes, 203136 OS fsyncs
0.00 reads/s, 0 avg bytes/read, 0.00 writes/s, 0.00 fsyncs/s
-------------------------------------
INSERT BUFFER AND ADAPTIVE HASH INDEX
-------------------------------------
Ibuf: size 1, free list len 0, seg size 2, 0 merges
merged operations:
 insert 0, delete mark 0, delete 0
discarded operations:
 insert 0, delete mark 0, delete 0
Hash table size 34679, node heap has 1 buffer(s)
Hash table size 34679, node heap has 1 buffer(s)
Hash table size 34679, node heap has 0 buffer(s)
Hash table size 34679, node heap has 0 buffer(s)
Hash table size 34679, node heap has 0 buffer(s)
Hash table size 34679, node heap has 0 buffer(s)
Hash table size 34679, node heap has 1 buffer(s)
Hash table size 34679, node heap has 1 buffer(s)
0.00 hash searches/s, 0.00 non-hash searches/s
---
LOG
---
Log sequence number          1946117363
Log buffer assigned up to    1946117363
Log buffer completed up to   1946117363
Log written up to            1946117363
Log flushed up to            1946117363
Added dirty pages up to      1946117363
Pages flushed up to          1946117363
Last checkpoint at           1946117363
485427 log i/o's done, 0.00 log i/o's/second
----------------------
BUFFER POOL AND MEMORY
----------------------

// The total memory allocated for the buffer pool in
bytes.
Total large memory allocated 0

// The total memory allocated for the InnoDB data
dictionary in bytes.
Dictionary memory allocated 461204

Buffer pool size   8192
Free buffers       1024
Database pages     7164
Old database pages 2624
Modified db pages  0
Pending reads      0
Pending writes: LRU 0, flush list 0, single page 0

// The total number of pages made young in the
buffer pool LRU list (moved to the head of sublist
of “new” pages).

// The total number of pages not made young in the
buffer pool LRU list (pages that have remained in
the “old” sublist without being made young).

Pages made young 1346, not young 342061449
0.00 youngs/s, 0.00 non-youngs/s
Pages read 3768664, created 93051, written 93925
0.00 reads/s, 0.00 creates/s, 0.00 writes/s
No buffer pool page gets since the last printout
Pages read ahead 0.00/s, evicted without access 0.00/s, Random read ahead 0.00/s
LRU len: 7164, unzip_LRU len: 0
I/O sum[0]:cur[0], unzip sum[0]:cur[0]

--------------
ROW OPERATIONS
--------------
0 queries inside InnoDB, 0 queries in queue
0 read views open inside InnoDB
Process ID=42080, Main thread ID=140011689203456 , state=sleeping
Number of rows inserted 8661245, updated 0, deleted 0, read 375192754
0.00 inserts/s, 0.00 updates/s, 0.00 deletes/s, 0.00 reads/s
Number of system rows inserted 219, updated 503, deleted 0, read 5396
0.00 inserts/s, 0.00 updates/s, 0.00 deletes/s, 0.00 reads/s
----------------------------
END OF INNODB MONITOR OUTPUT
============================
```

