# Elastisearch

## Elastisearch 查看shard情况

curl -XGET 172.16.206.82:9200/_cat/shards?h=index,shard,prirep,state,unassigned.reason| grep UNASSIGNED|sort #


