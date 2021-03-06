CHANGELOG
=========

1.1.4 (Oct 3, 2014)
====================

* Improvements
    * Strictly checked routing-table between manager-node and other nodes
    * Implemented the data diagnosis function of a storage-node
    * [#249](https://github.com/leo-project/leofs/issues/249) ``leo_manager`` Improve whereis command
* Fixed Bugs
    * [#246](https://github.com/leo-project/leofs/issues/246) ``leo_storage`` Could not recursively creating directory
    * [#247](https://github.com/leo-project/leofs/issues/247) ``leo_storage`` Start normally even if error occur
    * [#250](https://github.com/leo-project/leofs/issues/250) ``leo_statistics`` leo_statistics_sampler can be down under very high load
* Used libraries
    * leo project
        * [leo_backend-db v1.1.2](https://github.com/leo-project/leo_backend_db.git)
        * [leo_cache v0.6.0](https://github.com/leo-project/leo_cache.git)
        * [leo_commons v1.1.0](https://github.com/leo-project/leo_commons.git)
        * [leo_dcerl v0.2.11](https://github.com/leo-project/leo_dcerl.git)
        * [leo_logger v1.1.2](https://github.com/leo-project/leo_logger.git)
        * [leo_mcerl v0.4.1](https://github.com/leo-project/leo_mcerl.git)
        * [leo_mq v1.0.10](https://github.com/leo-project/leo_mq.git)
        * [leo_object_storage v1.1.5](https://github.com/leo-project/leo_object_storage.git)
        * [leo_ordning_reda v0.10.9](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_redundant_manager 1.8.9](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_rpc v0.8.10](https://github.com/leo-project/leo_rpc.git)
        * [leo_pod v0.6.2](https://github.com/leo-project/leo_pod.git)
        * [leo_s3_libs v1.1.3](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v1.0.7](https://github.com/leo-project/leo_statistics.git)
        * [savanna_agent v0.4.4](https://github.com/leo-project/savanna_agent.git)
        * [savanna_commons v0.8.6](https://github.com/leo-project/savanna_commons.git)
        * [erpcgen v0.2.3](https://github.com/leo-project/erpcgen.git)
        * [nfs_rpc_server v0.2.2](https://github.com/leo-project/nfs_rpc_server.git)
        * [leo_gateway v1.1.4](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v1.1.4](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v1.1.4](https://github.com/leo-project/leo_storage.git)
    * others
        * [bitcask v1.7.0](https://github.com/basho/bitcask.git)
        * [cowboy v0.8.6](https://github.com/extend/cowboy.git)
        * [cowlib v0.6.2](https://github.com/extend/cowboy.git)
        * [eleveldb v1.4.10](https://github.com/basho/eleveldb.git)
        * [folsom v0.8.1](https://github.com/boundary/folsom.git)
        * [jiffy v0.8.5](https://github.com/davisp/jiffy.git)
        * [lz4 v0.2.2](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlng-lz4)


1.1.3 (Sep 12, 2014)
====================

* Improved
    * Implement the "rollback" command, which is able to rollback state of a storage node from 'detach' to 'running'
* Fixed Bugs
    * [#236](https://github.com/leo-project/leofs/issues/236) ``leo_redundant_manager`` - storage node empty after 1.1.2 update and compaction
    * [#237](https://github.com/leo-project/leofs/issues/237) ``leo_manager`` - Cannot complete the re-balance objects and the recover-node command
    * [#238](https://github.com/leo-project/leofs/issues/238) ``leo_manager`` - Failed to migrate mnesia data when upgrading LeoFS from pre2 to 1.1.2
    * [#241](https://github.com/leo-project/leofs/issues/241) ``leo_gateway`` - Change the default ram cache capasity from 1GB to 256MB
    * [#242](https://github.com/leo-project/leofs/issues/242) ``leo_gateway`` - leo_garteway process could be down when receiving an invalid request
    * [#243](https://github.com/leo-project/leofs/issues/243) ``leo_storage`` - leo_gateway could respond 500 instead of 404
* Used libraries
    * leo project
        * [leo_backend-db v1.1.1](https://github.com/leo-project/leo_backend_db.git)
        * [leo_cache v0.4.24](https://github.com/leo-project/leo_cache.git)
        * [leo_commons v1.0.5](https://github.com/leo-project/leo_commons.git)
        * [leo_dcerl v0.2.10](https://github.com/leo-project/leo_dcerl.git)
        * [leo_logger v1.0.5](https://github.com/leo-project/leo_logger.git)
        * [leo_mcerl v0.4.0](https://github.com/leo-project/leo_mcerl.git)
        * [leo_mq v1.0.9](https://github.com/leo-project/leo_mq.git)
        * [leo_object_storage v1.1.3](https://github.com/leo-project/leo_object_storage.git)
        * [leo_ordning_reda v0.10.8](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_redundant_manager v1.8.8](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_rpc v0.8.9](https://github.com/leo-project/leo_rpc.git)
        * [leo_pod v0.6.2](https://github.com/leo-project/leo_pod.git)
        * [leo_s3_libs v1.1.2](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v1.0.6](https://github.com/leo-project/leo_statistics.git)
        * [savanna_agent v0.4.3](https://github.com/leo-project/savanna_agent.git)
        * [savanna_commons v0.8.5](https://github.com/leo-project/savanna_commons.git)
        * [erpcgen v0.2.3](https://github.com/leo-project/erpcgen.git)
        * [nfs_rpc_server v0.2.2](https://github.com/leo-project/nfs_rpc_server.git)
        * [leo_gateway v1.1.3](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v1.1.3](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v1.1.3](https://github.com/leo-project/leo_storage.git)
    * others
        * [bitcask v1.7.0](https://github.com/basho/bitcask.git)
        * [cowboy v0.8.6](https://github.com/extend/cowboy.git)
        * [cowlib v0.6.2](https://github.com/extend/cowboy.git)
        * [eleveldb v1.4.10](https://github.com/basho/eleveldb.git)
        * [folsom v0.8.1](https://github.com/boundary/folsom.git)
        * [jiffy v0.8.5](https://github.com/davisp/jiffy.git)
        * [lz4 v0.2.2](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlng-lz4)


1.1.2 (Sep 4, 2014)
===================

* Improved
    * ``leo_object_storage`` - Improved the compaction mechanism
        * It absolutely minimized time required for lock of a storage during data-compaction
* Fixed Bugs
    * [#225](https://github.com/leo-project/leofs/issues/225) ``leo_manager`` - The history command may cause VM to crash
        * We've provided the [tools/vacuum_history](https://github.com/leo-project/leofs_utils/tree/develop/tools/vacuum_history)
    * [#229](https://github.com/leo-project/leofs/issues/229) ``leo_gateway`` - Can't upload file name with space or other character got 403 forbidden
    * [#230](https://github.com/leo-project/leofs/issues/230) ``leo_gateway`` - COPY request fail when the source path include urlencoded characters
    * [#234](https://github.com/leo-project/leofs/issues/234) ``leo_gateway`` - Unexpected error may occur when responding 403/404
    * [#235](https://github.com/leo-project/leofs/issues/235) ``leo_storage`` - MDC replication could cause VM to crash (in narrow band width network - 100Mbps)
* Used libraries
    * leo project
        * [leo_backend-db v1.1.1](https://github.com/leo-project/leo_backend_db.git)
        * [leo_cache v0.4.24](https://github.com/leo-project/leo_cache.git)
        * [leo_commons v1.0.5](https://github.com/leo-project/leo_commons.git)
        * [leo_dcerl v0.2.10](https://github.com/leo-project/leo_dcerl.git)
        * [leo_logger v1.0.5](https://github.com/leo-project/leo_logger.git)
        * [leo_mcerl v0.4.0](https://github.com/leo-project/leo_mcerl.git)
        * [leo_mq v1.0.9](https://github.com/leo-project/leo_mq.git)
        * [leo_object_storage v1.1.3](https://github.com/leo-project/leo_object_storage.git)
        * [leo_ordning_reda v0.10.8](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_redundant_manager v1.8.7](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_rpc v0.8.9](https://github.com/leo-project/leo_rpc.git)
        * [leo_pod v0.6.2](https://github.com/leo-project/leo_pod.git)
        * [leo_s3_libs v1.1.2](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v1.0.6](https://github.com/leo-project/leo_statistics.git)
        * [savanna_agent v0.4.3](https://github.com/leo-project/savanna_agent.git)
        * [savanna_commons v0.8.5](https://github.com/leo-project/savanna_commons.git)
        * [erpcgen v0.2.3](https://github.com/leo-project/erpcgen.git)
        * [nfs_rpc_server v0.2.2](https://github.com/leo-project/nfs_rpc_server.git)
        * [leo_gateway v1.1.2](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v1.1.2](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v1.1.2](https://github.com/leo-project/leo_storage.git)
    * others
        * [bitcask v1.7.0](https://github.com/basho/bitcask.git)
        * [cowboy v0.8.6](https://github.com/extend/cowboy.git)
        * [cowlib v0.6.2](https://github.com/extend/cowboy.git)
        * [eleveldb v1.4.10](https://github.com/basho/eleveldb.git)
        * [folsom v0.8.1](https://github.com/boundary/folsom.git)
        * [jiffy v0.8.5](https://github.com/davisp/jiffy.git)
        * [lz4 v0.2.2](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlng-lz4)


1.1.1 (Aug 21, 2014)
=========================

* Improved
    * [leofs-adm](https://github.com/leo-project/leofs/blob/master/leofs-adm)
        * Supported FreeBSD
        * Able to set *host* and *port* of the Manager node
    * The compaction mechanism
        * Added *raw-file-path* in collapsed-object-log during executing data-compaction
* Fixed Bugs
    * [#219](https://github.com/leo-project/leofs/issues/219) ``leo_gateway`` ``leo_s3_libs`` - Access Denied error when putting a file to a bucket with the same name
    * [#222](https://github.com/leo-project/leofs/issues/222) ``leo_gateway`` - Discard unnecessary object with the compaction after failure of storing a large object
    * [#223](https://github.com/leo-project/leofs/issues/223) ``leo_object_storage`` - Not match checksum of an large-object-parent after executed the rebalance command and the recover-node command
    * ``leo_manager`` - Manager node could not modify Gateway node's ring-hash.
        * The issue appeared v1.1.0.
    * ``leo_object_storage`` - The compaction command might fail when an object container has broken objects at its head
        * It's absolutely rare case
    * ``leo_redundant_manager`` - Manager could not generate RING when taking over objects from a detach-node to a attach-node (a new node)
* Used libraries
    * leo project
        * [leo_backend-db v1.0.8](https://github.com/leo-project/leo_backend_db.git)
        * [leo_cache v0.4.23](https://github.com/leo-project/leo_cache.git)
        * [leo_commons v1.0.4](https://github.com/leo-project/leo_commons.git)
        * [leo_dcerl v0.2.10](https://github.com/leo-project/leo_dcerl.git)
        * [leo_logger v1.0.4](https://github.com/leo-project/leo_logger.git)
        * [leo_mcerl v0.4.0](https://github.com/leo-project/leo_mcerl.git)
        * [leo_mq v1.0.8](https://github.com/leo-project/leo_mq.git)
        * [leo_object_storage v1.1.2](https://github.com/leo-project/leo_object_storage.git)
        * [leo_ordning_reda v0.10.5](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_redundant_manager v1.8.6](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_rpc v0.8.8](https://github.com/leo-project/leo_rpc.git)
        * [leo_pod v0.6.2](https://github.com/leo-project/leo_pod.git)
        * [leo_s3_libs v1.1.1](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v1.0.5](https://github.com/leo-project/leo_statistics.git)
        * [savanna_agent v0.4.2](https://github.com/leo-project/savanna_agent.git)
        * [savanna_commons v0.8.4](https://github.com/leo-project/savanna_commons.git)
        * [erpcgen v0.2.3](https://github.com/leo-project/erpcgen.git)
        * [nfs_rpc_server v0.2.2](https://github.com/leo-project/nfs_rpc_server.git)
        * [leo_gateway v1.1.1](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v1.1.1](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v1.1.1](https://github.com/leo-project/leo_storage.git)
    * others
        * [bitcask v1.7.0](https://github.com/basho/bitcask.git)
        * [cowboy v0.8.6](https://github.com/extend/cowboy.git)
        * [cowlib v0.6.2](https://github.com/extend/cowboy.git)
        * [eleveldb v1.4.10](https://github.com/basho/eleveldb.git)
        * [folsom v0.8.1](https://github.com/boundary/folsom.git)
        * [jiffy v0.8.5](https://github.com/davisp/jiffy.git)
        * [lz4 v0.2.2](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlng-lz4)


1.1.0 (Aug 6, 2014)
=========================

* New Features
    * Implement [NFS Support](http://leo-project.net/leofs/docs/configuration_5.html) as one of LeoFS protocols, which is the alpha version.
        * We have checked this mechanism with *CentOS 6.5* and *Ubuntu Server 14.04 LTS* but we're goinng to investigate other OS such as *FreeBSD* and *SmartOS*.
        * **NOTE:** Changed [the configuration of the protocol](https://github.com/leo-project/leo_gateway/blob/develop/priv/leo_gateway.conf#L46) from ``http.handler`` to ``protocol``
    * The  [leofs-adm](https://github.com/leo-project/leofs/blob/master/leofs-adm) script
        * This command makes administrative operations of LeoFS very easy.
* Improved
    * Refactored all libraries and applications using *dialyzer*
* Fixed Bugs
    * [#142](https://github.com/leo-project/leofs/issues/142) ``leo_manager`` - Unknown Behavior - Could not retrieve RING
    * [#193](https://github.com/leo-project/leofs/issues/193) ``leo_gateway`` - PUT with REPLACE could leave a source file
    * [#199](https://github.com/leo-project/leofs/issues/199) ``leo_storage`` - An object in a sub directory (2 layer and over) could not be removed with DragonDisk
    * [#207](https://github.com/leo-project/leofs/issues/207) ``leo_object_storage`` - Compaction may fail when an AVS is corrupted
    * [#208](https://github.com/leo-project/leofs/issues/208) ``leo_object_storage`` - Compaction may leave stale objects which size are larger than the chunk size
    * ``leo-storage`` Multi data center replication may fail without notifying errors under a narrow bandwidth and very high-load.

* Used libraries
    * leo project
        * [leo_backend-db v1.0.8](https://github.com/leo-project/leo_backend_db.git)
        * [leo_cache v0.4.23](https://github.com/leo-project/leo_cache.git)
        * [leo_commons v1.0.4](https://github.com/leo-project/leo_commons.git)
        * [leo_dcerl v0.2.10](https://github.com/leo-project/leo_dcerl.git)
        * [leo_logger v1.0.4](https://github.com/leo-project/leo_logger.git)
        * [leo_mcerl v0.4.0](https://github.com/leo-project/leo_mcerl.git)
        * [leo_mq v1.0.8](https://github.com/leo-project/leo_mq.git)
        * [leo_object_storage v1.1.0](https://github.com/leo-project/leo_object_storage.git)
        * [leo_ordning_reda v0.10.5](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_redundant_manager v1.8.4](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_rpc v0.8.8](https://github.com/leo-project/leo_rpc.git)
        * [leo_pod v0.6.2](https://github.com/leo-project/leo_pod.git)
        * [leo_s3_libs v1.1.0](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v1.0.4](https://github.com/leo-project/leo_statistics.git)
        * [savanna_agent v0.4.2](https://github.com/leo-project/savanna_agent.git)
        * [savanna_commons v0.8.4](https://github.com/leo-project/savanna_commons.git)
        * [erpcgen v0.2.2](https://github.com/leo-project/erpcgen.git)
        * [nfs_rpc_server v0.2.1](https://github.com/leo-project/nfs_rpc_server.git)
        * [leo_gateway v1.1.0](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v1.1.0](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v1.1.0](https://github.com/leo-project/leo_storage.git)
    * others
        * [bitcask v1.7.0](https://github.com/basho/bitcask.git)
        * [cowboy v0.8.6](https://github.com/extend/cowboy.git)
        * [cowlib v0.6.2](https://github.com/extend/cowboy.git)
        * [eleveldb v1.4.10](https://github.com/basho/eleveldb.git)
        * [folsom v0.8.1](https://github.com/boundary/folsom.git)
        * [jiffy v0.8.5](https://github.com/davisp/jiffy.git)
        * [lz4 v0.2.2](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlng-lz4)


1.0.2 (May 9, 2014)
=========================

* Fixed Bugs
    * [#189](https://github.com/leo-project/leofs/issues/189) ``leo_object_storage`` - Actual disk usage is different from the manager-console.
    * [#188](https://github.com/leo-project/leofs/issues/188) ``leo_object_storage`` - When existing large objects in a leo_storage, data loss of which happend with the compaction command.
* Used libraries
    * leo project
        * [leo_backend-db v1.0.3](https://github.com/leo-project/leo_backend_db.git)
        * [leo_cache v0.4.20](https://github.com/leo-project/leo_cache.git)
        * [leo_commons v1.0.1](https://github.com/leo-project/leo_commons.git)
        * [leo_dcerl v0.2.7](https://github.com/leo-project/leo_dcerl.git)
        * [leo_logger v1.0.2](https://github.com/leo-project/leo_logger.git)
        * [leo_mcerl v0.2.9](https://github.com/leo-project/leo_mcerl.git)
        * [leo_mq v1.0.3](https://github.com/leo-project/leo_mq.git)
        * [leo_object_storage v1.0.4](https://github.com/leo-project/leo_object_storage.git)
        * [leo_ordning_reda v0.10.3](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_redundant_manager v1.8.1](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_rpc v0.8.3](https://github.com/leo-project/leo_rpc.git)
        * [leo_pod v0.6.0](https://github.com/leo-project/leo_pod.git)
        * [leo_s3_libs v1.0.1](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v1.0.x](https://github.com/leo-project/leo_statistics.git)
        * [savanna_agent v0.2.2](https://github.com/leo-project/savanna_agent.git)
        * [savanna_commons v0.6.3](https://github.com/leo-project/savanna_commons.git)
        * [leo_gateway v1.0.2](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v1.0.2](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v1.0.2](https://github.com/leo-project/leo_storage.git)
    * others
        * [bitcask v1.6.7](https://github.com/basho/bitcask.git)
        * [cowboy v0.8.6](https://github.com/extend/cowboy.git)
        * [eleveldb v1.4.7](https://github.com/basho/eleveldb.git)
        * [folsom v0.8.1](https://github.com/boundary/folsom.git)
        * [jiffy v0.8.5](https://github.com/davisp/jiffy.git)
        * [lz4 v0.1.1](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlng-lz4)


1.0.1 (May 8, 2014)
=========================

* Improved
    * [#183](https://github.com/leo-project/leofs/issues/183) ``leo_storage`` - Replication messages could be sent between storage nodes more than necessary
    * [#176](https://github.com/leo-project/leofs/issues/176) ``leo_center``  - Supported LeoFS v1.0
    * [#167](https://github.com/leo-project/leofs/issues/167) ``leo_storage`` - Automatically synchronization of objects between a local cluster and another remote cluster could fail
    * [#165](https://github.com/leo-project/leofs/issues/165) ``leo_manager`` - Could not modify ``cluster_id``, ``dc_id`` after leo_manger started
    * [#140](https://github.com/leo-project/leofs/issues/140) ``leo_gateway`` - Supported for ``s3gof3r`` as S3-Client
* Fixed Bugs
    * Corrected termination of applications
    * [#187](https://github.com/leo-project/leofs/issues/187) ``leo_storage`` - Could not work the ``rebalance`` and ``recover`` command
    * [#186](https://github.com/leo-project/leofs/issues/186) ``leo_storage`` - Could not correctly finish the ``compaction`` command when exists large-objects
    * [#185](https://github.com/leo-project/leofs/issues/185) ``leo_manager`` - Failed to execute the ``delete-endpoint`` command
    * [#184](https://github.com/leo-project/leofs/issues/183) ``leo_manager`` - Failed to execute the ``update-acl`` command
    * [#182](https://github.com/leo-project/leofs/issues/182) ``leo_manager`` - When status of a storage is ``restarted``, issuing compaction could cause data loss
    * [#173](https://github.com/leo-project/leofs/issues/173) ``leo_manager`` - Could not migrate data from leofs-1.0.0-pre3 ro leofs-1.0.0
    * [#171](https://github.com/leo-project/leofs/issues/171) ``leo_gateway`` - Head-method with PHP client could not work.
    * [#160](https://github.com/leo-project/leofs/issues/160) ``leo_manager`` - Failed to upgrade from v0.14.6 to v1.0.0
    * [#153](https://github.com/leo-project/leofs/issues/153) ``leo_gateway`` - When using s3cmd, GET operation for larger than 5MB object gives error at leo_gateway
* Used libraries
    * leo project
        * [leo_backend-db v1.0.3](https://github.com/leo-project/leo_backend_db.git)
        * [leo_cache v0.4.20](https://github.com/leo-project/leo_cache.git)
        * [leo_commons v1.0.1](https://github.com/leo-project/leo_commons.git)
        * [leo_dcerl v0.2.7](https://github.com/leo-project/leo_dcerl.git)
        * [leo_logger v1.0.2](https://github.com/leo-project/leo_logger.git)
        * [leo_mcerl v0.2.9](https://github.com/leo-project/leo_mcerl.git)
        * [leo_mq v1.0.3](https://github.com/leo-project/leo_mq.git)
        * [leo_object_storage v1.0.3](https://github.com/leo-project/leo_object_storage.git)
        * [leo_ordning_reda v0.10.3](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_redundant_manager v1.8.1](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_rpc v0.8.3](https://github.com/leo-project/leo_rpc.git)
        * [leo_pod v0.6.0](https://github.com/leo-project/leo_pod.git)
        * [leo_s3_libs v1.0.1](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v1.0.x](https://github.com/leo-project/leo_statistics.git)
        * [savanna_agent v0.2.2](https://github.com/leo-project/savanna_agent.git)
        * [savanna_commons v0.6.3](https://github.com/leo-project/savanna_commons.git)
        * [leo_gateway v1.0.1](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v1.0.1](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v1.0.1](https://github.com/leo-project/leo_storage.git)
    * others
        * [bitcask v1.6.7](https://github.com/basho/bitcask.git)
        * [eleveldb v1.4.7](https://github.com/basho/eleveldb.git)
        * [cowboy v0.8.6](https://github.com/extend/cowboy.git)
        * [folsom v0.8.1](https://github.com/boundary/folsom.git)
        * [jiffy v0.8.5](https://github.com/davisp/jiffy.git)
        * [lz4 v0.1.1](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlng-lz4)


1.0.0 (Apr 2, 2014)
=========================

* New features
    * Multi datacenter replication (1st phase)
        * Realized async-replication between clusters
            * After sent stacked objects to a remote-cluster, receive the list of metadatas from a remote-cluster, then compare them with local-cluster. Eventually, an inconsistent object is recovered.
            * Provided easy operation of multi-datacenter replication with leo-manager's console
            * After joined a new cluster, automatically synchronize objects between local-cluster and a remote-cluster
        * Provided ``recover cluster`` which is able to fix inconsistency objects with remote-cluster
    * [#139](https://github.com/leo-project/leofs/issues/139) Implemented the Bucket ACL
* Improved
    * ``leo_backend_db`` Bump bitcask to v1.6.7
    * ``leo_object_storage`` Updated compaction, handling an object for the multi-dc replication
    * ``leo_ordning_reda`` Updated handle-send interface for the multi-dc replication
    * ``leo_rpc`` Improved to check-in pools into leo_pod
* Fixed Bugs
    * [#144](https://github.com/leo-project/leofs/issues/143) - Failure occurred when running snmpwalk
    * [#146](https://github.com/leo-project/leofs/issues/146) - No retry when receiving a head request
    * [#148](https://github.com/leo-project/leofs/issues/148) - AWS-clients of PHP and Node.js could not copy object properly copied file became 0byte
    * [#151](https://github.com/leo-project/leofs/issues/151) - ``whereis-command`` had not been recorded on history table
    * [#162](https://github.com/leo-project/leofs/issues/162) - Able to get removed user on the manager-console
    * [#163](https://github.com/leo-project/leofs/issues/163) - ``update-acl`` and ``get-acl`` methods unexpected to display the permission messages
* Used libraries
    * leo project
        * [leo_backend-db v1.0.2](https://github.com/leo-project/leo_backend_db.git)
        * [leo_cache v0.4.20](https://github.com/leo-project/leo_cache.git)
        * [leo_commons v1.0.1](https://github.com/leo-project/leo_commons.git)
        * [leo_dcerl v0.2.7](https://github.com/leo-project/leo_dcerl.git)
        * [leo_logger v1.0.1](https://github.com/leo-project/leo_logger.git)
        * [leo_mcerl v0.2.9](https://github.com/leo-project/leo_mcerl.git)
        * [leo_mq v1.0.2](https://github.com/leo-project/leo_mq.git)
        * [leo_object_storage v1.0.1](https://github.com/leo-project/leo_object_storage.git)
        * [leo_ordning_reda v0.10.2](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_redundant_manager v1.8.0](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_rpc v0.8.2](https://github.com/leo-project/leo_rpc.git)
        * [leo_pod v0.4.8](https://github.com/leo-project/leo_pod.git)
        * [leo_s3_libs v1.0.1](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v1.0.1](https://github.com/leo-project/leo_statistics.git)
        * [savanna_agent v0.2.1](https://github.com/leo-project/savanna_agent.git)
        * [savanna_commons v0.6.2](https://github.com/leo-project/savanna_commons.git)
        * [APPLICATION]
        * [leo_gateway v1.0.0](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v1.0.0](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v1.0.0](https://github.com/leo-project/leo_storage.git)
    * others
        * [bitcask v1.6.7](https://github.com/basho/bitcask.git)
        * [cowboy v0.8.6](https://github.com/extend/cowboy.git)
        * [folsom v0.8.1](https://github.com/boundary/folsom.git)
        * [jiffy v0.8.5](https://github.com/davisp/jiffy.git)
        * [lz4 v0.1.1](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlng-lz4)


1.0.0-pre3 (Feb 20, 2014)
=========================

* Improved
    * `leo_manager` Able to plug functions in order to realize to build another manager
    * `leo_redundant_manager` Improved the performance of the membership and the rebalance
    * `leo_redundant_manager` Modified that restrict membership of a node, the state of which is not running
    * `leo_statistics` Switch the function of statistics to [savanna_commons](https://github.com/leo-project/savanna_commons), which isan Erlang based metrics server.
    * `leo_ordning_reda` Improved the function of object stacking
    * `leo_ordning_reda` Improved efficiency of termination of a process
* Fixed Bugs
    * `leo_gateway` Fixed to escape xml elements correctly with xmerl_lib:export_text
    * `leo_gateway` Modified the http response body format when responding a http error status according to the S3 spec(http://docs.aws.amazon.com/AmazonS3/latest/API/ErrorResponses.html#RESTErrorResponses)
    * `leo_manager` [#116](https://github.com/leo-project/leofs/issues/116) Implement new sync mechanism in Manager, which is able to maintain hard consistency of the rings
    * `libcutil (cache-lib)` [#123](https://github.com/leo-project/leofs/issues/123) Add `-fPIC` to CFLAGS
    * `leo_backend_db` [#129](https://github.com/leo-project/leofs/issues/129) Fixed to remove all files in a bucket when deleting it(only occured in case using leveldb as metadata storage)
    * `leo_gateway` [#130](https://github.com/leo-project/leofs/issues/130) Fixed wrong access log formats when operationg a large-object
    * `leo_manager`,`leo_storage`,`leo_gateway` [#131](https://github.com/leo-project/leofs/issues/131) Wrote the version number in the source of configurations
    * `leo_gateway` [#136](https://github.com/leo-project/leofs/issues/136) Support that move and copy a large object with S3-Client(s)
    * `leo_object_storage` Fixed to handle invalid data blocks while doing compaction
    * `leo_rpc` Fixed to close a tcp socket properly in any cases
    * `leo_gateway` [#140](https://github.com/leo-project/leofs/issues/140) Fixed to return 206 status when responding a partial body
* Used libraries
    * leo project
        * [leo_backend-db v1.0.0](https://github.com/leo-project/leo_backend_db.git)
        * [leo_cache v0.4.19](https://github.com/leo-project/leo_cache.git)
        * [leo_commons v1.0.0](https://github.com/leo-project/leo_commons.git)
        * [leo_dcerl v0.2.7](https://github.com/leo-project/leo_dcerl.git)
        * [leo_logger v1.0.0](https://github.com/leo-project/leo_logger.git)
        * [leo_mcerl v0.2.9](https://github.com/leo-project/leo_mcerl.git)
        * [leo_mq v1.0.0](https://github.com/leo-project/leo_mq.git)
        * [leo_object_storage v1.0.0](https://github.com/leo-project/leo_object_storage.git)
        * [leo_ordning_reda v0.10.0](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_pod v0.4.7](https://github.com/leo-project/leo_pod.git)
        * [leo_redundant_manager v1.4.1](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_rpc v0.8.0](https://github.com/leo-project/leo_rpc.git)
        * [leo_s3_libs v0.12.28](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v1.0.0](https://github.com/leo-project/leo_statistics.git)
        * [savanna_commons v0.4.3](https://github.com/leo-project/savanna_commons.git)
        * [leo_gateway v1.0.0-pre3](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v1.0.0-pre3](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v1.0.0-pre3](https://github.com/leo-project/leo_storage.git)
    * others
        * [bitcask v1.6.7](https://github.com/basho/bitcask.git)
        * [cowboy v0.8.6](https://github.com/extend/cowboy.git)
        * [eleveldb v1.4.7](https://github.com/basho/eleveldb)
        * [folsom v0.8.1](https://github.com/boundary/folsom.git)
        * [jiffy v0.8.5](https://github.com/davisp/jiffy.git)
        * [lz4 v0.1.1](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlng-lz4)


1.0.0-pre2 (Jan 22, 2014)
=========================

* New Features
     * Implemented for Multi DC Replication
         * Synchronize configuration and staus of remote cluster(s) after joined each other
         * Regularly check status of remote cluster(s)
         * Add the commands of Multi DC Replication in Manager
              * 'join-cluster' and 'remove-cluster'
* Improved
     * The performance of the prefix search, which like a "ls"
     * Changed format of the metadata because of improvement of the prefix search
     * Removed Elasticsearch integration in the logger
* Fixed Bugs
     * Unexpected response from leo_storage to leo_gateway when an object wan not found
     * Respond an error with deletion of an object when it was not found
* Used libraries
    * leo project
        * [leo_backend-db v0.14.5](https://github.com/leo-project/leo_backend_db.git)
        * [leo_cache v0.4.17](https://github.com/leo-project/leo_cache.git)
        * [leo_commons v0.14.10](https://github.com/leo-project/leo_commons.git)
        * [leo_dcerl v0.2.7](https://github.com/leo-project/leo_dcerl.git)
        * [leo_logger v0.12.8](https://github.com/leo-project/leo_logger.git)
        * [leo_mcerl v0.2.9](https://github.com/leo-project/leo_mcerl.git)
        * [leo_mq v0.12.25](https://github.com/leo-project/leo_mq.git)
        * [leo_object_storage v0.14.11](https://github.com/leo-project/leo_object_storage.git)
        * [leo_ordning_reda v0.8.19](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_pod v0.4.7](https://github.com/leo-project/leo_pod.git)
        * [leo_redundant_manager v1.4.0](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_rpc v0.6.2](https://github.com/leo-project/leo_rpc.git)
        * [leo_s3_libs v0.12.27](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v0.14.9](https://github.com/leo-project/leo_statistics.git)
        * [leo_gateway v1.0.0-pre2](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v1.0.0-pre2](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v1.0.0-pre2](https://github.com/leo-project/leo_storage.git)
    * others
        * [bitcask v1.6.4](https://github.com/basho/bitcask.git)
        * [cowboy v0.8.6](https://github.com/extend/cowboy.git)
        * [folsom v0.8.0](https://github.com/boundary/folsom.git)
        * [jiffy v0.8.5](https://github.com/davisp/jiffy.git)
        * [lz4 v0.1.1](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlng-lz4)


1.0.0-pre1 (Dec 27, 2013)
=========================

* Improved
   * Revised the replicator and the read-repairer for the multi data center replicaion
   * [#113](https://github.com/leo-project/leofs/issues/113) Modified the configuration of limit of large-object length
      * "limit length" = ${large_object.chunked_obj_len} * ${large_object.max_chunked_objs}
   * Improve the function of "rebalance-command"
   * Improve the function of "start-command"
   * Added "dump-ring" on the manager console
* Fixed Bugs
   * Fixed that a rebalance msg can be lost during rebalance with a 0.02% possibility
   * Fixed that not retrieved a bucket-info when stopping all managers
* Used libraries
    * leo project
        * [leo_backend-db v0.14.2](https://github.com/leo-project/leo_backend_db.git)
        * [leo_cache v0.4.16](https://github.com/leo-project/leo_cache.git)
        * [leo_commons v0.14.9](https://github.com/leo-project/leo_commons.git)
        * [leo_dcerl v0.2.7](https://github.com/leo-project/leo_dcerl.git)
        * [leo_logger v0.12.6](https://github.com/leo-project/leo_logger.git)
        * [leo_mcerl v0.2.9](https://github.com/leo-project/leo_mcerl.git)
        * [leo_mq v0.12.23](https://github.com/leo-project/leo_mq.git)
        * [leo_object_storage v0.14.8](https://github.com/leo-project/leo_object_storage.git)
        * [leo_ordning_reda v0.8.18](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_redundant_manager v1.2.6](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_s3_libs v0.12.25](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v0.14.8](https://github.com/leo-project/leo_statistics.git)
        * [leo_gateway v1.0.0-pre1](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v1.0.0-pre1](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v1.0.0-pre1](https://github.com/leo-project/leo_storage.git)
    * others
        * [bitcask v1.6.4](https://github.com/basho/bitcask.git)
        * [cowboy v0.8.6](https://github.com/extend/cowboy.git)
        * [folsom v0.8.0](https://github.com/boundary/folsom.git)
        * [jiffy v0.8.5](https://github.com/davisp/jiffy.git)
        * [lz4 v0.1.1](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlng-lz4)


0.16.8 (Dec 12, 2013)
=====================

* Improved
  * [#109](https://github.com/leo-project/leofs/issues/109) Moved to "ini-file" configuration, which no longer use Erlang-specific syntax. Using [cuttlefish](https://github.com/basho/cuttlefish) to realize this function.
  * [#110](https://github.com/leo-project/leofs/issues/110) Supported [erlcloud](https://github.com/gleber/erlcloud) for Erlang users
  * [Supported Mac OS X](https://github.com/leo-project/libcutil/pull/2) which was contributed from Jeff Li
* Fixed Bugs
  * [#102](https://github.com/leo-project/leofs/issues/102) Happened timeout when uploading a large object
  * [#108](https://github.com/leo-project/leofs/issues/108) Happened not relocation of object(s) when removing a node and executing rebalance then add same node
  * [#111](https://github.com/leo-project/leofs/issues/111) Could not upload large size file
  * Fixed that not migrated "Bucket Table"
  * Fixed that an exception of compaction happened rarely
* Used libraries
    * leo project
        * [leo_backend-db v0.14.2](https://github.com/leo-project/leo_backend_db.git)
        * [leo_cache v0.4.16](https://github.com/leo-project/leo_cache.git)
        * [leo_commons v0.14.9](https://github.com/leo-project/leo_commons.git)
        * [leo_dcerl v0.2.7](https://github.com/leo-project/leo_dcerl.git)
        * [leo_logger v0.12.6](https://github.com/leo-project/leo_logger.git)
        * [leo_mcerl v0.2.9](https://github.com/leo-project/leo_mcerl.git)
        * [leo_mq v0.12.22](https://github.com/leo-project/leo_mq.git)
        * [leo_object_storage v0.14.8](https://github.com/leo-project/leo_object_storage.git)
        * [leo_ordning_reda v0.8.18](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_redundant_manager v1.2.5](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_s3_libs v0.12.24](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v0.14.7](https://github.com/leo-project/leo_statistics.git)
        * [leo_gateway v0.16.8](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v0.16.8](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v0.16.8](https://github.com/leo-project/leo_storage.git)
    * others
        * [bitcask v1.6.4](https://github.com/basho/bitcask.git)
        * [cowboy v0.8.6](https://github.com/extend/cowboy.git)
        * [folsom](https://github.com/boundary/folsom.git)
        * [jiffy](https://github.com/davisp/jiffy.git)
        * [lz4 v0.1.1](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlng-lz4)


0.16.5 (Nov 26, 2013)
=====================

* Improved
   * S3-API related
      * [#103] (https://github.com/leo-project/leofs/issues/103) Able to change password on Manager console
      * [#105] (https://github.com/leo-project/leofs/issues/105) Able to change an owner of a bucket
      * [#106] (https://github.com/leo-project/leofs/issues/106) Rename *set-endpoint* to *add-endpoint* in order to unify it and other commands
      * Multicast *update-acl* to Gateway's node(s)
      * Multicast *delete-bucket* to Gateway's node(s)
   * Other
      * Revised that manage redundant nodes toward the multi data center replication
        * Supported that manage previous and current members in a cluster in order not to happen lost data during the period of relocation of data
        * Able to recover that Manager failed to send massage of relocation from Manager to Storage(s)
        * Reduced costs of relocation of data than previous version
      * [#98] (https://github.com/leo-project/leofs/issues/98) Made a bucket name compatible with the AWS-S3 naming rule of US-region
      * [#99] (https://github.com/leo-project/leofs/issues/99) Able to set log-directory of *leo-redundant-manager*
      * Supported Ubuntu-13.10 (include Ubuntu Server 13.10)
* Fixed Bugs
  * [#94] (https://github.com/leo-project/leofs/issues/94) Happened an error when parsing XML document with S3's Java-Client
  * [#95] (https://github.com/leo-project/leofs/issues/95) Could not resume storage node
  * [#96] (https://github.com/leo-project/leofs/issues/96) Happened an error when Gateway is requested from *boto*
  * [#97] (https://github.com/leo-project/leofs/issues/97) Could not upload an object when including a bucket name in a path
  * [#100] (https://github.com/leo-project/leofs/issues/100) Broken records after update from 0.14.9 to 0.16.0
* Used libraries
    * leo project
        * [leo_backend-db v0.14.1](https://github.com/leo-project/leo_backend_db.git)
        * [leo_cache v0.4.14](https://github.com/leo-project/leo_cache.git)
        * [leo_commons v0.14.8](https://github.com/leo-project/leo_commons.git)
        * [leo_dcerl v0.2.5](https://github.com/leo-project/leo_dcerl.git)
        * [leo_logger v0.12.5](https://github.com/leo-project/leo_logger.git)
        * [leo_mcerl v0.2.7](https://github.com/leo-project/leo_mcerl.git)
        * [leo_mq v0.12.21](https://github.com/leo-project/leo_mq.git)
        * [leo_object_storage v0.14.7](https://github.com/leo-project/leo_object_storage.git)
        * [leo_ordning_reda v0.8.17](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_redundant_manager v1.2.3](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_s3_libs v0.12.21](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v0.14.6](https://github.com/leo-project/leo_statistics.git)
        * [leo_gateway v0.16.5](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v0.16.5](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v0.16.5](https://github.com/leo-project/leo_storage.git)
    * others
        * [bitcask v1.6.2](https://github.com/basho/bitcask.git)
        * [cowboy v0.8.6](https://github.com/extend/cowboy.git)
        * [folsom](https://github.com/boundary/folsom.git)
        * [jiffy](https://github.com/davisp/jiffy.git)
        * [lz4 v0.1.1](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlng-lz4)


0.16.0 (Oct 25, 2013)
=====================

* New Features
    * Gateway
        * Supported GET/PUT ACL a Bucket [S3-API]
        * (Beta) Able to output access-logs to Elasticsearch in order to realize to access-log analysis with Kibana
    * Other
        * Implemented SmartOS packager (Contributed by Heinz N. Gies - [Project FiFo](http://project-fifo.net/))
* Improved
    * Manager
        * Supported single 'Manager'
        * Supported to check # of detached node before executing detach-command
* Used libraries
    * leo project
        * [leo_backend-db v0.14.1](https://github.com/leo-project/leo_backend_db.git)
        * [leo_cache v0.4.13](https://github.com/leo-project/leo_cache.git)
        * [leo_commons v0.14.8](https://github.com/leo-project/leo_commons.git)
        * [leo_dcerl v0.2.4](https://github.com/leo-project/leo_dcerl.git)
        * [leo_logger v0.12.5](https://github.com/leo-project/leo_logger.git)
        * [leo_mcerl v0.2.6](https://github.com/leo-project/leo_mcerl.git)
        * [leo_mq v0.12.20](https://github.com/leo-project/leo_mq.git)
        * [leo_object_storage v0.14.7](https://github.com/leo-project/leo_object_storage.git)
        * [leo_ordning_reda v0.8.17](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_redundant_manager v1.0.4](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_s3_libs v0.12.17](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v0.14.6](https://github.com/leo-project/leo_statistics.git)
        * [leo_gateway v0.16.0](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v0.16.0](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v0.16.0](https://github.com/leo-project/leo_storage.git)
    * others
        * [bitcask v1.6.2](https://github.com/basho/bitcask.git)
        * [cowboy v0.8.6](https://github.com/extend/cowboy.git)
        * [folsom](https://github.com/boundary/folsom.git)
        * [jiffy](https://github.com/davisp/jiffy.git)
        * [lz4 v0.1.1](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlng-lz4)


0.14.9 (Sep 27, 2013)
=====================

* Improved
    * Supported Erlang/OTP R16B02
    * Increased performance of leo_redundant_manager

* Used libraries
    * leo project
        * [leo_backend-db v0.14.0](https://github.com/leo-project/leo_backend_db.git)
        * [leo_cache v0.4.12](https://github.com/leo-project/leo_cache.git)
        * [leo_commons v0.14.6](https://github.com/leo-project/leo_commons.git)
        * [leo_dcerl v0.2.4](https://github.com/leo-project/leo_dcerl.git)
        * [leo_logger v0.12.3](https://github.com/leo-project/leo_logger.git)
        * [leo_mcerl v0.2.6](https://github.com/leo-project/leo_mcerl.git)
        * [leo_mq v0.12.19](https://github.com/leo-project/leo_mq.git)
        * [leo_object_storage v0.14.6](https://github.com/leo-project/leo_object_storage.git)
        * [leo_ordning_reda v0.8.16](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_redundant_manager v1.0.3](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_s3_libs v0.12.15](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v0.14.5](https://github.com/leo-project/leo_statistics.git)
        * [leo_gateway v0.14.14](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v0.14.9](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v0.14.7](https://github.com/leo-project/leo_storage.git)
    * others
        * [bitcask v1.6.2](https://github.com/basho/bitcask.git)
        * [cowboy v0.8.6](https://github.com/extend/cowboy.git)
        * [folsom](https://github.com/boundary/folsom.git)
        * [jiffy](https://github.com/davisp/jiffy.git)
        * [lz4 v0.1.1](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlng-lz4)



0.14.8 (Sep 12, 2013)
=====================

* Bugs Fixed
    * Gateway
        * Deletion failed with s3cmd in the case of not existed a targate file
        * OOM with access-log output
    * Manager
        * Start failed in the case of not reached the message from the Manager to storage-node(s)
        * Not removed a member(storage-node) when its status was 'attached'

* Used libraries
    * leo project
        * [leo_backend-db v0.12.17](https://github.com/leo-project/leo_backend_db.git)
        * [leo_cache v0.4.11](https://github.com/leo-project/leo_cache.git)
        * [leo_commons v0.14.4](https://github.com/leo-project/leo_commons.git)
        * [leo_dcerl v0.2.3](https://github.com/leo-project/leo_dcerl.git)
        * [leo_logger v0.12.2](https://github.com/leo-project/leo_logger.git)
        * [leo_mcerl v0.2.5](https://github.com/leo-project/leo_mcerl.git)
        * [leo_mq v0.12.18](https://github.com/leo-project/leo_mq.git)
        * [leo_object_storage v0.14.5](https://github.com/leo-project/leo_object_storage.git)
        * [leo_ordning_reda v0.8.15](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_redundant_manager v1.0.2](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_s3_libs v0.12.14](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v0.14.4](https://github.com/leo-project/leo_statistics.git)
        * [leo_gateway v0.14.13](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v0.14.8](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v0.14.6](https://github.com/leo-project/leo_storage.git)
    * others
        * [bitcask v1.6.2](https://github.com/basho/bitcask.git)
        * [cowboy v0.8.6](https://github.com/extend/cowboy.git)
        * [folsom](https://github.com/boundary/folsom.git)
        * [jiffy](https://github.com/davisp/jiffy.git)
        * [lz4 v0.1.1](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlng-lz4)


0.14.7 (Aug 23, 2013)
=====================

* Improved
    * Gateway
        * Able to output access-log

* Used libraries
    * leo project
        * [leo_backend-db v0.12.17](https://github.com/leo-project/leo_backend_db.git)
        * [leo_cache v0.4.10](https://github.com/leo-project/leo_cache.git)
        * [leo_commons v0.14.4](https://github.com/leo-project/leo_commons.git)
        * [leo_dcerl v0.2.3](https://github.com/leo-project/leo_dcerl.git)
        * [leo_logger v0.12.1](https://github.com/leo-project/leo_logger.git)
        * [leo_mcerl v0.2.4](https://github.com/leo-project/leo_mcerl.git)
        * [leo_mq v0.12.18](https://github.com/leo-project/leo_mq.git)
        * [leo_object_storage v0.14.5](https://github.com/leo-project/leo_object_storage.git)
        * [leo_ordning_reda v0.8.15](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_redundant_manager v1.0.2](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_s3_libs v0.12.14](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v0.14.4](https://github.com/leo-project/leo_statistics.git)
        * [leo_gateway v0.14.12](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v0.14.7](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v0.14.5](https://github.com/leo-project/leo_storage.git)
    * others
        * [bitcask v1.6.2](https://github.com/basho/bitcask.git)
        * [cowboy v0.8.6](https://github.com/extend/cowboy.git)
        * [folsom](https://github.com/boundary/folsom.git)
        * [jiffy](https://github.com/davisp/jiffy.git)
        * [lz4 v0.1.1](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlng-lz4)


0.14.6 (July 11, 2013)
======================

* Improved
    * Able to set the max number of requests allowed in a single keep-alive session

* Bugs Fixed
    * Gateway
        * Fixed to respond HTTP-headers properly when using *disk-cache*
    * Manager
        * Fixed changed status from *running* to *restarted* when restarted leo-manager

* Used libraries
    * leo project
        * [leo_backend-db v0.12.17](https://github.com/leo-project/leo_backend_db.git)
        * [leo_cache v0.4.10](https://github.com/leo-project/leo_cache.git)
        * [leo_commons v0.14.4](https://github.com/leo-project/leo_commons.git)
        * [leo_dcerl v0.2.3](https://github.com/leo-project/leo_dcerl.git)
        * [leo_logger v0.10.12](https://github.com/leo-project/leo_logger.git)
        * [leo_mcerl v0.2.4](https://github.com/leo-project/leo_mcerl.git)
        * [leo_mq v0.12.18](https://github.com/leo-project/leo_mq.git)
        * [leo_object_storage v0.14.5](https://github.com/leo-project/leo_object_storage.git)
        * [leo_ordning_reda v0.8.15](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_redundant_manager v1.0.2](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_s3_libs v0.12.14](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v0.14.4](https://github.com/leo-project/leo_statistics.git)
        * [leo_gateway v0.14.11](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v0.14.6](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v0.14.4](https://github.com/leo-project/leo_storage.git)
    * others
        * [bitcask v1.6.2](https://github.com/basho/bitcask.git)
        * [cowboy v0.8.6](https://github.com/extend/cowboy.git)
        * [folsom](https://github.com/boundary/folsom.git)
        * [jiffy](https://github.com/davisp/jiffy.git)
        * [lz4 v0.1.1](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlng-lz4)


0.14.5 (July 8, 2013)
=====================

* Bugs Fixed
    * Gateway
        * Gateways may respond an HTTP response with a wrong MIME type as "plain/text" when requested an uppercase filename extension such as "*.JPG" and "*.PNG" from clients
        * Fixed an error handlings properly when processing a large file with disk cache

* Used libraries
    * leo project
        * [leo_backend-db v0.12.17](https://github.com/leo-project/leo_backend_db.git)
        * [leo_cache v0.4.10](https://github.com/leo-project/leo_cache.git)
        * [leo_commons v0.14.4](https://github.com/leo-project/leo_commons.git)
        * [leo_dcerl v0.2.3](https://github.com/leo-project/leo_dcerl.git)
        * [leo_logger v0.10.12](https://github.com/leo-project/leo_logger.git)
        * [leo_mcerl v0.2.4](https://github.com/leo-project/leo_mcerl.git)
        * [leo_mq v0.12.18](https://github.com/leo-project/leo_mq.git)
        * [leo_object_storage v0.14.5](https://github.com/leo-project/leo_object_storage.git)
        * [leo_ordning_reda v0.8.15](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_redundant_manager v1.0.2](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_s3_libs v0.12.14](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v0.14.4](https://github.com/leo-project/leo_statistics.git)
        * [leo_gateway v0.14.10](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v0.14.5](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v0.14.4](https://github.com/leo-project/leo_storage.git)
    * others
        * [bitcask v1.6.2](https://github.com/basho/bitcask.git)
        * [cowboy v0.8.6](https://github.com/extend/cowboy.git)
        * [folsom](https://github.com/boundary/folsom.git)
        * [jiffy](https://github.com/davisp/jiffy.git)
        * [lz4 v0.1.1](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlng-lz4)


0.14.4 (June 28, 2013)
=======================

* Improved
    * Supported [Erlang/OTP R16B01](http://www.erlang.org/news/54)
    * Gateway
        * Optimize the slab size for normal use cases

* Used libraries
    * leo project
        * [leo_backend-db v0.12.16](https://github.com/leo-project/leo_backend_db.git)
        * [leo_cache v0.4.9](https://github.com/leo-project/leo_cache.git)
        * [leo_commons v0.14.3](https://github.com/leo-project/leo_commons.git)
        * [leo_dcerl v0.2.3](https://github.com/leo-project/leo_dcerl.git)
        * [leo_logger v0.10.11](https://github.com/leo-project/leo_logger.git)
        * [leo_mcerl v0.2.4](https://github.com/leo-project/leo_mcerl.git)
        * [leo_mq v0.12.17](https://github.com/leo-project/leo_mq.git)
        * [leo_object_storage v0.14.4](https://github.com/leo-project/leo_object_storage.git)
        * [leo_ordning_reda v0.8.14](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_redundant_manager v1.0.1](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_s3_libs v0.12.13](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v0.14.3](https://github.com/leo-project/leo_statistics.git)
        * [leo_gateway v0.14.7](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v0.14.3](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v0.14.3](https://github.com/leo-project/leo_storage.git)
    * others
        * [bitcask v1.6.2](https://github.com/basho/bitcask.git)
        * [cowboy v0.8.6](https://github.com/extend/cowboy.git)
        * [folsom](https://github.com/boundary/folsom.git)
        * [jiffy](https://github.com/davisp/jiffy.git)
        * [lz4 v0.1.1](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlng-lz4)


0.14.3 (June 21, 2013)
=======================

* Improved
    * Improved redundant-manager's performance when retrieving redundancies by up to 20%
        * Changed method of retrieving redundancies from *ets* to worker-processes
    * Make a parameter of consumption of queue's message interval into the application config
    * Replace obsolete functions *crypto:sha|md5* with *crypto:hash*

* Fixed Bugs
    * Manager
        * Some problem with bucket names format
    * Storage
        * The number of queue messages can be wrong value
            * Needed to call *bitcask:merge/1* after relaunch the storage process
        * Compaction-function can fail - "did not match data" when a target file is corrupted

* Used libraries
    * leo project
        * [leo_backend-db v0.12.16](https://github.com/leo-project/leo_backend_db.git)
        * [leo_cache v0.4.8](https://github.com/leo-project/leo_cache.git)
        * [leo_commons v0.14.3](https://github.com/leo-project/leo_commons.git)
        * [leo_dcerl v0.2.3](https://github.com/leo-project/leo_dcerl.git)
        * [leo_logger v0.10.11](https://github.com/leo-project/leo_logger.git)
        * [leo_mcerl v0.2.3](https://github.com/leo-project/leo_mcerl.git)
        * [leo_mq v0.12.17](https://github.com/leo-project/leo_mq.git)
        * [leo_object_storage v0.14.4](https://github.com/leo-project/leo_object_storage.git)
        * [leo_ordning_reda v0.8.14](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_redundant_manager v1.0.1](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_s3_libs v0.12.13](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v0.14.3](https://github.com/leo-project/leo_statistics.git)
        * [leo_gateway v0.14.5](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v0.14.3](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v0.14.3](https://github.com/leo-project/leo_storage.git)
    * others
        * [bitcask v1.6.2](https://github.com/basho/bitcask.git)
        * [cowboy v0.8.6](https://github.com/extend/cowboy.git)
        * [folsom](https://github.com/boundary/folsom.git)
        * [jiffy](https://github.com/davisp/jiffy.git)
        * [lz4 v0.1.1](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlng-lz4)


0.14.2 (June 7, 2013)
=======================

* New Features
    * Supported rack-awareness replica placement

* Improved
    * Gateway
        * Improved cache-libs, which are mem-cache and disc-cache.
            * Refactoring codes - Getting rid of duplicate codes to "libcutil"
            * Using file:sendfile/2 when retrieving an object from disk cache(dcerl)
        * Improve S3-API's compatibility
            * Supported "Range request API" for a large object
            * Supported retrieving object-list
        * Upgrade Cowboy to v0.8.5
    * Storage
        * Improved data-compaction
            * Performance tuning
            * Avoid polluting OS page caches during compaction
        * Modified the launch process
            * Able to retry connection with manager(s)
    * Manager
        * Supported to Able to remove gateway-node from manager's console when the state of specified node is ‘stop’
        * Supported system-data backup/restore (mnesia)
        * Supported taking over manager(s) for affected hardware failure
        * Supported taking over storage-node when having attach/detach nodes in operation
            * Able to take over from detach-node's files to attach-node

* Fixed Bugs
    * Gateway
        * Reply empty response unintentionally when using some s3-clients

* Used libraries
    * leo project
        * [leo_backend-db v0.12.14](https://github.com/leo-project/leo_backend_db.git)
        * [leo_cache v0.4.7](https://github.com/leo-project/leo_cache.git)
        * [leo_commons v0.14.1](https://github.com/leo-project/leo_commons.git)
        * [leo_dcerl v0.2.2](https://github.com/leo-project/leo_dcerl.git)
        * [leo_logger v0.10.10](https://github.com/leo-project/leo_logger.git)
        * [leo_mcerl v0.2.2](https://github.com/leo-project/leo_mcerl.git)
        * [leo_mq v0.12.15](https://github.com/leo-project/leo_mq.git)
        * [leo_object_storage v0.14.3](https://github.com/leo-project/leo_object_storage.git)
        * [leo_ordning_reda v0.8.13](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_redundant_manager v0.14.2](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_s3_libs v0.12.10](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v0.14.2](https://github.com/leo-project/leo_statistics.git)
        * [leo_gateway v0.14.4](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v0.14.2](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v0.14.2](https://github.com/leo-project/leo_storage.git)
    * others
        * [bitcask v1.6.2](https://github.com/basho/bitcask.git)
        * [cowboy v0.8.5](https://github.com/extend/cowboy.git)
        * [folsom](https://github.com/boundary/folsom.git)
        * [jiffy](https://github.com/davisp/jiffy.git)
        * [lz4 v0.1.1](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlng-lz4)


0.14.1-1 (May 8, 2013)
=======================

* Improved
    * Gateway
        * Upgrade Ranch and Cowboy to latest version
* Fix Bugs
    * Gateway
        * Reply empty response unintentionally when using some s3 clients
            * "leo_gateway" stored a "0-byte length object" into the cache when put an large-object(over 5MB) from clients. So We supported to remove a registered object from the cache.


0.14.1 (Apr 15, 2013)
=====================

* Improved
    * Gateway
        * Commonize request-handler for easily creating APIs
        * Improve cache-controller which was replaced from ecache to leo_cache
        * Improve performance
            * Upgrade Ranch and Cowboy to latest version
    * Storage
        * Improved phased data-compaction
            * To realize non-blocking data-compaction
                * before: Making compaction per an "object-storage-file"
                * after: Making compaction per an object
    * Manager/Storage
        * Implement judgment of precondition in rebalance-comamnd
        * Implemented ``recover-command`` in Manager
            * To realize:
                * synchronize a file: ``recover file ${file-path}``
                * recover a target-node files: ``recover node ${storage-node}``
                * recover target-node RING: ``recover ring ${storage-node}``
* Fix Bugs
    * NOT worked ``s3cmd`` by degraded
    * Stored wrong file-path with REST-API by degraded

* Used libraries
    * leo project
        * [leo_cache v0.4.4](https://github.com/leo-project/leo_cache.git)
        * [leo_commons v0.12.12](https://github.com/leo-project/leo_commons.git)
        * [leo_backend-db v0.12.11](https://github.com/leo-project/leo_backend_db.git)
        * [leo_object_storage v0.14.1](https://github.com/leo-project/leo_object_storage.git)
        * [leo_mq v0.12.12](https://github.com/leo-project/leo_mq.git)
        * [leo_ordning_reda v0.8.11](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_redundant_manager v0.12.19](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_s3_libs v0.12.8](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v0.10.11](https://github.com/leo-project/leo_statistics.git)
        * [leo_logger v0.10.8](https://github.com/leo-project/leo_logger.git)
        * [leo_gateway v0.14.1](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v0.14.1](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v0.14.1](https://github.com/leo-project/leo_storage.git)
        * [cherly v0.12.5](https://github.com/leo-project/cherly.git)
        * [dcerl v0.4.1](https://github.com/leo-project/dcerl.git)
    * others
        * [bitcask](https://github.com/basho/bitcask.git)
        * [cowboy v0.8.3](https://github.com/extend/cowboy.git)
        * [folsom](https://github.com/boundary/folsom.git)
        * [jiffy](https://github.com/davisp/jiffy.git)
        * [lz4 v0.1.1](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlng-lz4)


0.14.0 (Mar 20, 2013)
=====================

* Improved
    * Upgrade Cowboy from 0.6.2(foked/add patches) to 0.8.2(original)
        * Improved put/get large-object performance
    * Support recovery of manager-status-monitor after network partition occured

* Fix bugs
    * Recovery objects (Storage)
        * Ignore ``detach-status`` from replication-message
    * Not handle ``compaction-start command`` invalid argument on Manager-console

* Used libraries
    * leo project
        * [leo_commons v0.12.11](https://github.com/leo-project/leo_commons.git)
        * [leo_backend-db v0.12.10](https://github.com/leo-project/leo_backend_db.git)
        * [leo_object_storage v0.12.29](https://github.com/leo-project/leo_object_storage.git)
        * [leo_mq v0.12.11](https://github.com/leo-project/leo_mq.git)
        * [leo_ordning_reda v0.8.10](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_redundant_manager v0.12.18](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_s3_libs v0.12.7](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v0.10.10](https://github.com/leo-project/leo_statistics.git)
        * [leo_logger v0.10.7](https://github.com/leo-project/leo_logger.git)
        * [leo_gateway v0.14.0](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v0.14.0](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v0.14.0](https://github.com/leo-project/leo_storage.git)
        * [ecache v0.10.15](https://github.com/leo-project/ecache.git)
        * [cherly v0.12.4](https://github.com/leo-project/cherly.git)
    * others
        * [bitcask](https://github.com/basho/bitcask.git)
        * [cowboy v0.8.2](https://github.com/extend/cowboy.git)
        * [folsom](https://github.com/boundary/folsom.git)
        * [jiffy](https://github.com/davisp/jiffy.git)
        * [lz4 v0.1.1](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlng-lz4)


0.14.0-RC2 (Mar 14, 2013)
========================

* Improved
    * Improved cache-mechanism (Gateway)
        * Support Layered Cache, First cache-layer is RAM and Secondary cache-layer is SSD (or HDD)
        * This version realized that cache-destination is decided by object-size
             * Need to set [gateway's configuration](http://www.leofs.org/docs/install.html#leofs-gateway)

* Fix bugs
    * Incorrect judgement of active storage-node
        * Possibility of including node(s) of ``attached (status)``

* Used libraries
    * leo project
        * [leo_commons v0.12.11](https://github.com/leo-project/leo_commons.git)
        * [leo_backend-db v0.12.10](https://github.com/leo-project/leo_backend_db.git)
        * [leo_object_storage v0.12.29](https://github.com/leo-project/leo_object_storage.git)
        * [leo_mq v0.12.11](https://github.com/leo-project/leo_mq.git)
        * [leo_ordning_reda v0.8.10](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_redundant_manager v0.12.17](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_s3_libs v0.12.7](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v0.10.10](https://github.com/leo-project/leo_statistics.git)
        * [leo_logger v0.10.7](https://github.com/leo-project/leo_logger.git)
        * [leo_gateway v0.14.0-RC2](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v0.14.0-RC2](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v0.14.0-RC2](https://github.com/leo-project/leo_storage.git)
        * [ecache v0.10.14](https://github.com/leo-project/ecache.git)
        * [cherly v0.12.4](https://github.com/leo-project/cherly.git)
    * others
        * [bitcask](https://github.com/basho/bitcask.git)
        * [cowboy v0.6.2](https://github.com/leo-project/cowboy.git) - forked from [extend/cowboy](https://github.com/extend/cowboy)
        * [folsom](https://github.com/boundary/folsom.git)
        * [jiffy](https://github.com/davisp/jiffy.git)
        * [lz4 v0.1.1](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlng-lz4)

0.14.0-RC1 (Mar 5, 2013)
========================

* Improved
    * Improved cache-mechanism (Gateway)
        * According to improving efficiency of object-cache-pool, LeoFS-Gateway was able to store an object up to 8MB into the RAM
    * Improved data-compaction related processes (Storage, Manager)
        * Realized compact a part of data-storage, which called "phased data-compaction"
        * Realized ``suspend`` and ``resume`` data-compaction, also able to comfirm status of processes
    * Supported recovery from temporally network unlink #1 (Storage, Manager)
        * Automatically recovered target-node(s), which status transition from ``stop`` to ``running``

* Fix bugs
    * Cannot consume queueing-message(s) when storage cluster has a detached node
        * Resolved that messages of a detached node ignored

* Used libraries
    * leo project
        * [leo_commons v0.12.10](https://github.com/leo-project/leo_commons.git)
        * [leo_backend-db v0.12.9](https://github.com/leo-project/leo_backend_db.git)
        * [leo_object_storage v0.12.28](https://github.com/leo-project/leo_object_storage.git)
        * [leo_mq v0.12.9](https://github.com/leo-project/leo_mq.git)
        * [leo_ordning_reda v0.8.9](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_redundant_manager v0.12.15](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_s3_libs v0.12.6](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v0.10.9](https://github.com/leo-project/leo_statistics.git)
        * [leo_logger v0.10.6](https://github.com/leo-project/leo_logger.git)
        * [leo_gateway v0.14.0-RC1](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v0.14.0-RC1](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v0.14.0-RC1](https://github.com/leo-project/leo_storage.git)
        * [ecache v0.10.8](https://github.com/leo-project/ecache.git)
        * [cherly v0.12.4](https://github.com/leo-project/cherly.git)
    * others
        * [bitcask](https://github.com/basho/bitcask.git)
        * [cowboy v0.6.2](https://github.com/leo-project/cowboy.git) - forked from [extend/cowboy](https://github.com/extend/cowboy)
        * [folsom](https://github.com/boundary/folsom.git)
        * [jiffy](https://github.com/davisp/jiffy.git)
        * [lz4 v0.1.1](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlng-lz4)


0.12.7 (Dec 26, 2012)
---------------------

* Improve performances
    * Storage Performance Tuning#6
        * Related libs: [leo_storage, leo_object_storage]
        * Reduced compaction-cost
             * Able to execution of parallel comaction
                 * Get maximum performance by setting a appropriate number corresponding with number of cores.
* Improve
    * Gateway:
        * The optimal timeout according to file size set up.
        * Modified default cache mode from 'http' to 'inner'
    * Storage:
        * Modified completion of storage for restriction of file destruction
            * When shutting down storage, in charge of storage-process close files
        * Refactor message-queue functions
            * Unified read-failure's queue and write-failure's queue
* Fix bugs
    * Storage:
        * Overwrite an object during rebalance
            * Always check the version(clock) of object
        * Fix haystacks reopen correctly when failing compaction
    * Manager-Console
        * Crush get-endpoints when no-records
        * Crush get-users when no-records

* Used libraries
    * leo project
        * [leo_commons v0.12.6](https://github.com/leo-project/leo_commons.git)
        * [leo_backend-db v0.12.2](https://github.com/leo-project/leo_backend_db.git)
        * [leo_object_storage v0.12.16](https://github.com/leo-project/leo_object_storage.git)
        * [leo_mq v0.12.2](https://github.com/leo-project/leo_mq.git)
        * [leo_ordning_reda v0.8.5](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_redundant_manager v0.12.4](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_s3_libs v0.12.2](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v0.10.6](https://github.com/leo-project/leo_statistics.git)
        * [leo_logger v0.10.3](https://github.com/leo-project/leo_logger.git)
        * [leo_gateway v0.12.9](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v0.12.9](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v0.12.9](https://github.com/leo-project/leo_storage.git)
        * [ecache v0.10.5](https://github.com/leo-project/ecache.git)
        * [cherly v0.12.0](https://github.com/leo-project/cherly.git)
    * others
        * [bitcask](https://github.com/basho/bitcask.git)
        * [cowboy v0.6.2](https://github.com/leo-project/cowboy.git) - forked from [extend/cowboy](https://github.com/extend/cowboy)
        * [folsom](https://github.com/boundary/folsom.git)
        * [jiffy](https://github.com/davisp/jiffy.git)
        * [lz4 v0.1.1](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlang-lz4)


0.12.5 (Dec 7, 2012)
---------------------

* Improve performances
    * Storage Performance Tuning#5
        * Related libs: [leo_storage, leo_object_storage]
        * Reduced using spawn/1 in replicator #2
* Improve
    * Able to monitor VM-values on Leo Manager's console
    * Deprecate parameterized module in leo_object_storage
        * Reference: http://www.erlang.org/news/35
    * Modified re-launch storage process
        * When regularly stop the storage-process, It writes current status in a file. Then it restarts the storage-process when reading the file.
    * Able to post a large part of an object to LeoFS with multipart-upload API.
* Fix bugs
    * Respond invalid "Etag" from the gateway when using multipart-upload API.
    * Possibility of file-destruction
        * Termination of storages for the restriction of file-destruction
            * Related libs: [leo_storage, leo_object_storage]

* Used libraries
    * leo project
        * [leo_commons v0.12.6](https://github.com/leo-project/leo_commons.git)
        * [leo_backend-db v0.12.0](https://github.com/leo-project/leo_backend_db.git)
        * [leo_object_storage v0.12.12](https://github.com/leo-project/leo_object_storage.git)
        * [leo_mq v0.12.0](https://github.com/leo-project/leo_mq.git)
        * [leo_ordning_reda v0.8.4](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_redundant_manager v0.12.1](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_s3_libs v0.12.0](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v0.10.6](https://github.com/leo-project/leo_statistics.git)
        * [leo_logger v0.10.2](https://github.com/leo-project/leo_logger.git)
        * [leo_gateway v0.12.6](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v0.12.6](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v0.12.6](https://github.com/leo-project/leo_storage.git)
        * [ecache v0.10.3](https://github.com/leo-project/ecache.git)
        * [cherly v0.10.2](https://github.com/leo-project/cherly.git)
    * others
        * [bitcask](https://github.com/basho/bitcask.git)
        * [cowboy v0.6.2](https://github.com/leo-project/cowboy.git) - forked from [extend/cowboy](https://github.com/extend/cowboy)
        * [folsom](https://github.com/boundary/folsom.git)
        * [jiffy](https://github.com/davisp/jiffy.git)
        * [lz4 v0.1.1](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlang-lz4)


0.12.4 (Nov 21, 2012)
---------------------

* Improve performances
    * Storage Performance Tuning#4
        * Target libs: [leo_storage, leo_object_storage]
        * Reduced using spawn/1 in replicator #1
        * Used rpc:cast/4 for async-replication
* Improve
    * Able to retrieve leofs-uesrs from manager-console
    * NOT allow duplication registration of a user-account into the s3-credential
* Fix bugs
    * Fail rebalance and compaction when exists chunked objects in the storage
    * Manager-console crashed when inputed invalid parameter(s)

* Used libraries
    * leo project
        * [leo_commons v0.12.5](https://github.com/leo-project/leo_commons.git)
        * [leo_backend-db v0.10.8](https://github.com/leo-project/leo_backend_db.git)
        * [leo_object_storage v0.12.11](https://github.com/leo-project/leo_object_storage.git)
        * [leo_mq v0.10.5](https://github.com/leo-project/leo_mq.git)
        * [leo_ordning_reda v0.8.3](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_redundant_manager v0.12.0](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_s3_libs v0.10.7](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v0.10.5](https://github.com/leo-project/leo_statistics.git)
        * [leo_logger v0.10.1](https://github.com/leo-project/leo_logger.git)
        * [leo_gateway v0.12.5](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v0.12.5](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v0.12.5](https://github.com/leo-project/leo_storage.git)
        * [ecache v0.10.2](https://github.com/leo-project/ecache.git)
        * [cherly v0.10.1](https://github.com/leo-project/cherly.git)
    * others
        * [bitcask](https://github.com/basho/bitcask.git)
        * [cowboy v0.6.2](https://github.com/leo-project/cowboy.git) - forked from [extend/cowboy](https://github.com/extend/cowboy)
        * [folsom](https://github.com/boundary/folsom.git)
        * [jiffy](https://github.com/davisp/jiffy.git)
        * [lz4 v0.1.1](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlang-lz4)


0.12.3 (Nov 9, 2012)
--------------------

* Improve performances
    * Storage Performance Tuning#3
        * Reduced using list_to_binary/1 - [leo_storage, leo_object_storage]
        * Unified internal storage data-type to "binary"
* Improve S3 compatibility
    * Support Multipart upload an object (large-object)
* New feature
    * Able to monitor (SNMP)
        * Sum of objects/storage-node
        * Sum of object-length/storage-node
* Fix bugs
    * Deletion of chunked objects (large-object)
    * Fail rebalance when exists a restarting node
        * Adjust the start timing of RPC for reject requests from remote-node(s)

* Used libraries
    * leo project
        * [leo_commons v0.12.5](https://github.com/leo-project/leo_commons.git)
        * [leo_backend-db v0.10.8](https://github.com/leo-project/leo_backend_db.git)
        * [leo_object_storage v0.12.10](https://github.com/leo-project/leo_object_storage.git)
        * [leo_mq v0.10.5](https://github.com/leo-project/leo_mq.git)
        * [leo_ordning_reda v0.8.3](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_redundant_manager v0.12.0](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_s3_libs v0.10.6](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v0.10.5](https://github.com/leo-project/leo_statistics.git)
        * [leo_logger v0.10.1](https://github.com/leo-project/leo_logger.git)
        * [leo_gateway v0.12.4](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v0.12.4](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v0.12.4](https://github.com/leo-project/leo_storage.git)
        * [ecache v0.10.1](https://github.com/leo-project/ecache.git)
        * [cherly v0.10.0](https://github.com/leo-project/cherly.git)
    * others
        * [bitcask](https://github.com/basho/bitcask.git)
        * [cowboy v0.6.2](https://github.com/leo-project/cowboy.git) - forked from [extend/cowboy](https://github.com/extend/cowboy)
        * [folsom](https://github.com/boundary/folsom.git)
        * [jiffy](https://github.com/davisp/jiffy.git)
        * [lz4 v0.1.1](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlang-lz4)


0.12.2 (Nov 2, 2012)
--------------------

* Improve performances
    * Storage Performance Tuning#2
        * Revised put operation
* Improve S3 compatibility
    * Support deletion of a bucket
    * Support [s3cmd](http://s3tools.org/s3cmd) (s3-client)
* Fix bugs
    * Gateway:
        * NOT able to store object-cache because data-type is replaced from string to binary with 0.12.1
    * Storage "Compaction"
        * When excuting compact-command, Objects to be removed remain (chunked objects)
* Used libraries
    * leo project
        * [leo_commons v0.12.3](https://github.com/leo-project/leo_commons.git)
        * [leo_backend-db v0.10.7](https://github.com/leo-project/leo_backend_db.git)
        * [leo_object_storage v0.12.9](https://github.com/leo-project/leo_object_storage.git)
        * [leo_mq v0.10.4](https://github.com/leo-project/leo_mq.git)
        * [leo_ordning_reda v0.8.2](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_redundant_manager v0.10.4](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_s3_libs v0.10.5](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v0.10.4](https://github.com/leo-project/leo_statistics.git)
        * [leo_logger v0.10.0](https://github.com/leo-project/leo_logger.git)
        * [leo_gateway v0.12.3](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v0.12.3](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v0.12.3](https://github.com/leo-project/leo_storage.git)
        * [ecache v0.10.1](https://github.com/leo-project/ecache.git)
        * [cherly v0.10.0](https://github.com/leo-project/cherly.git)
    * others
        * [bitcask](https://github.com/basho/bitcask.git)
        * [cowboy v0.6.2](https://github.com/leo-project/cowboy.git) - forked from [extend/cowboy](https://github.com/extend/cowboy)
        * [folsom](https://github.com/boundary/folsom.git)
        * [jiffy](https://github.com/davisp/jiffy.git)
        * [lz4 v0.1.1](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlang-lz4)


0.12.1  (Oct 25, 2012)
----------------------

* Improve performances
    * Storage Performance Tuning#1
        * Reduced overhead
            * Modified replicator/repairer from gen_server to module
            * Revised data-flow from storage-engine to object/metadata storage
    * Reduced using list_to_binary/1
        * Modified bucket-related libs: [leo_gateway,leo_manager,leo_s3_libs]
    * Compressor/Decompressor replace from snappy to lz4
* Fix bugs
    * Has omissions an object of rebalance
    * Fixed S3 releated:
        * NOT able to remove an endpoint
        * Able to add a bucket with NOT exists access-key

* Used libraries
    * leo project
        * [leo_commons v0.12.0](https://github.com/leo-project/leo_commons.git)
        * [leo_backend-db v0.10.4](https://github.com/leo-project/leo_backend_db.git)
        * [leo_object_storage v0.12.4](https://github.com/leo-project/leo_object_storage.git)
        * [leo_mq v0.10.2](https://github.com/leo-project/leo_mq.git)
        * [leo_ordning_reda v0.8.0](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_redundant_manager v0.10.2](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_s3_libs v0.10.3](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v0.10.2](https://github.com/leo-project/leo_statistics.git)
        * [leo_logger v0.9.8](https://github.com/leo-project/leo_logger.git)
        * [leo_gateway v0.12.1](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v0.12.2](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v0.12.1](https://github.com/leo-project/leo_storage.git)
        * [ecache v0.10.1](https://github.com/leo-project/ecache.git)
        * [cherly v0.10.0](https://github.com/leo-project/cherly.git)
    * others
        * [bitcask](https://github.com/basho/bitcask.git)
        * [cowboy v0.6.2](https://github.com/leo-project/cowboy.git) - forked from [extend/cowboy](https://github.com/extend/cowboy)
        * [folsom](https://github.com/boundary/folsom.git)
        * [jiffy](https://github.com/davisp/jiffy.git)
        * [lz4 v0.1.1](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlang-lz4)


0.12.0 (Oct 20, 2012)
----------------------

* New feature - Large Object Support
    * Handled from a few bytes an object to a few GB an object
* Improve performances
    * Gateway Performance Tuning
        * HTTP-Server replace from Mochiweb to Cowboy
        * Reduced using list_to_binary/1
    * Revised order of system launch
        * before: Managers -> Storage -> Gateway
        * after : Managers -> Storage|Gateway
    * Changed type of key from string to binary
* Fix bugs
    * S3-API related
        * Overwrited bucket-info by NOT owners
        * When put-operation, NOT returned 'ETag' header
    * Compaction
        * When excuting compact-command, Objects to be removed partly may remain
* Used libraries
    * leo project
        * [leo_commons v0.12.0](https://github.com/leo-project/leo_commons.git)
        * [leo_backend-db v0.10.4](https://github.com/leo-project/leo_backend_db.git)
        * [leo_object_storage v0.12.3](https://github.com/leo-project/leo_object_storage.git)
        * [leo_mq v0.10.2](https://github.com/leo-project/leo_mq.git)
        * [leo_ordning_reda v0.6.1](https://github.com/leo-project/leo_ordning_reda.git)
        * [leo_redundant_manager v0.10.2](https://github.com/leo-project/leo_redundant_manager.git)
        * [leo_s3_libs v0.10.2](https://github.com/leo-project/leo_s3_libs.git)
        * [leo_statistics v0.10.1](https://github.com/leo-project/leo_statistics.git)
        * [leo_logger v0.9.7](https://github.com/leo-project/leo_logger.git)
        * [leo_gateway v0.12.0](https://github.com/leo-project/leo_gateway.git)
        * [leo_manager v0.12.0](https://github.com/leo-project/leo_manager.git)
        * [leo_storage v0.12.0](https://github.com/leo-project/leo_storage.git)
        * [ecache v0.10.1](https://github.com/leo-project/ecache.git)
        * [cherly v0.10.0](https://github.com/leo-project/cherly.git)
    * others
        * [bitcask](https://github.com/basho/bitcask.git)
        * [cowboy v0.6.2](https://github.com/leo-project/cowboy.git) - forked from [extend/cowboy](https://github.com/extend/cowboy)
        * [folsom](https://github.com/boundary/folsom.git)
        * [jiffy](https://github.com/davisp/jiffy.git)
        * [lz4 v0.1.1](https://github.com/leo-project/erlang-lz4.git) - forked from [szktty/erlang-lz4](https://github.com/szktty/erlang-lz4)
        * [snappy](https://github.com/fdmanana/snappy-erlang-nif.git)


0.10.2 (Sep 25, 2012)
----------------------

* Improve performances
    * NOT used "proplists:get_value" function
        * Replace from "proplists:get_value/2,3" to "lists:keyfind/2"
    * Related libs:
        * leo_gateway
        * leo_storage
        * leo_manager
        * leo_logger
        * leo_mq
        * leo_object_storage
        * leo_ordning_reda
        * leo_redundant_manager
        * leo_s3_libs
        * leo_statistics
* Improve leo_manager
    * Support output of json-format
    * Support multi-ports TCP-server
        * for CUI console
        * for Application (JSON-Format)
* Improve leo_storage
    * Support plural devices
    * Reduced rebalance/recover costs
        * Support compression of stacked objects and decompresson of received objects (Using snappy)
* Fix bugs
    * leo-gateway related (S3-related):
        * Create bucket from 'Dragon Disk'
        * When using cowboy can send bad values(not iodata)


0.10.1 (Sep 12, 2012)
---------------------

* Improve leo_hex performances
    * "binary_to_hex" function
    * Related libs:
        * leo_gateway
        * leo_object_storage
        * leo_redundant_manager
    * By this correspondence, LeoFS's performance improved 20% up.
* Improve leo_manager
    * Format of output from manager-console
        * Commands:
            * "status"
            * "whereis"
* Improve performance of "storage-stats" in manager-console
* Fix bugs
    * A handling error in S3-libs


0.10.0 (Aug 30, 2012)
---------------------

* Improve S3-API's compatibility
    * Add S3-authentication
    * Add S3-bucket
* Add S3-related command in LeoFS's manager
    * "s3-gen-key" : Generate a S3 key pair(AccessKeyID and SecretAccessKey)
    * "s3-set-endpoint" : Register a new S3 Endpoint
    * "s3-delete-endpoint" : Delete a S3 Endpoint
    * "s3-get-endpoints" : Retrieve all of S3 Endpoints registered
    * "s3-get-buckets" : Retrieve all of Buckets registered
* Improve order of system launch
    * Remove "attach command" in manager - After Storage launched, the node's state is automatically changed to "attached"
* Improve rebalance-function's performance which is about 5 times compare with v0.9.1
* Improve compact-function. Restrain storage's load when compact objects.
* Fix bugs
    * Deletion of Zero bytes in Storage
    * Behavior after the restart of Manager
    * Re-register procs into the Manager's monitor


0.9.1 (Jul 13, 2012)
--------------------

* Remove "apps" directory in leofs - Modified "reltool.config"
* Fix 'shadow vars'
* Remove ZMQ log-appender and AMQP log-appender for leo_logger, They will be provided LeoFS's sub projects.
* Improve - In order to be able to extend "LeoFS's Object Container's file format".


0.9.0  (Jul 4, 2012)
--------------------

* Initial release
