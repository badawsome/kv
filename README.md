# KV (WIP)
a key-value storage service.


## Target

1. Support put(k, v), get(k), delete(k).
2. Support compare-and-swap option.
3. Support number operation.
4. Support read-after-write consistency option. 
5. Multi media write support.(memory cache, disk log).
6. Single thread in the lowest layer.

### Advance target

1. With version, support rollback and commit.
2. Support complex data structure in cache, queue/hash table/rank table.
3. Support cluster, with raft consensus algorithm.
4. Support partition, with raft center cluster dispatcher.
5. Support auto-scale, with load balancer.
6. Support transaction.
7. Support multi-row storage.

## Road Map

1. Impl basic disk read and write with leveldb.
2. Impl basic memory read and write with redis.
3. Impl basic service based on RESP(REdis Serialization Protocol) and epoll IO / std net lib.
4. Rewrite without dependencies with rust.
5. TBD...