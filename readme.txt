Redis Datatypes:
    - Strings
    - Lists
    - Sets
    - Sorted Sets
    - Hashes
    - Bitmaps
    - Hyperlogs
    - Geospatial Indexes

Advantages Of Redis:
    - VERY Flexible
    - No schemes & Column Names
    - Very Fast : Can perform around 110,000 SETs per second, about 81,000 GETs per seconds
    - Rich Datatype Support
    - Cashing and Disk Persistence

Redis & Security
    - Designed to be accessed by trusted clients
    - Do not allow external access / Internet exposure
    - Simple authentication can be setup
    - Can be restricted to certain interfaces
    - Data encryption not supported

Command line:

    - ping
    - echo ""
    - SET key value
    - GET key
    - INCR key
    - DECR key
    - EXISTS key
    - DEL key
    - FLUSHALL
    - EXPIRE key 50(integer in seconds)
    - TTL key
    - SETEX key 50(integer in seconds) value
    - PERSIST key
    - MSET key value key value etc
    - APPEND key value
    - RENAME key key
    - CLEAR
    - LPUSH mylist value
    - LRANGE mylist 0 -1
    - RPUSH mylist value
    - LLEN mylist
    - LPOP mylist
    - RPOP mylist
    - LINSERT mylist BEFORE value

    - SADD setKey value
    - SISMEMBER setKey value
    - SMEMBERS setKey
    - SCARD setKey
    - SMOVE setKey anotherSetKey value
    - SREM setKey value

    - ZADD setKey sortValue value
    - ZRANK setKey value
    - ZRANGE setKey 0 -1
    - ZINCBY setKey 1 value

    - HSET user:edward name "Edward Gizbreht"
    - HSET user:edward email "ed.gizbreht@gmail.com"
    - HGET user:edward name
    - HGET user:edward email
    - HGETALL user:edward
    - HMSET user:andrew name "ANDREW" email "andrew@mail.com" age "25"
    - HGETALL user:andrew
    - HKEYS user:andrew
    - HVALS user:andrew
    - HINCRBY user:andrew age 1
    - HDEL user:edward name
    - HLEN user:edward