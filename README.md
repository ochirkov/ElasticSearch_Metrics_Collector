ElasticSearch_Metrics_Collector
===============================

Usage:
-----

    elasticsearch_metrics <option> <metric>


Supported options:
    - cluster
    - node

Supported metrics by options:

    Cluster:
        - active_primary_shards
        - active_shards
        - number_of_pending_tasks
        - relocating_shards
        - status
        - unassigned_shards
        - number_of_nodes
        - heap_max_in_bytes
        - heap_used_in_bytes
    Node:
        - heap_pool_young_gen_mem
        - heap_pool_old_gen_mem
        - heap_pool_survivor_gen_mem
        - heap_max_in_bytes
        - heap_used_in_bytes
        - heap_used_percent
        - total_filter_cache_mem
        - total_field_data_mem
        - total_merges_mem


Example:
        Get cluster status:

        `$ elasticsearch_metrics cluster status`

        Get heap_used_in_bytes on current node:

        `$ elasticsearch_metrics node heap_used_in_bytes`
