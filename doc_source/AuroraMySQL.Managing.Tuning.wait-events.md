# Tuning Aurora MySQL with wait events<a name="AuroraMySQL.Managing.Tuning.wait-events"></a>

The following table summarizes the Aurora MySQL wait events that most commonly indicate performance problems\. The following wait events are a subset of the list in [Aurora MySQL wait events](AuroraMySQL.Reference.md#AuroraMySQL.Reference.Waitevents)\.


| Wait event | Description | 
| --- | --- | 
|  [cpu](ams-waits.cpu.md)  |  This event occurs when a thread is active in CPU or is waiting for CPU\.  | 
|  [io/socket/sql/client\_connection](ams-waits.client-connection.md)  |  This event occurs when a thread is in the process of handling a new connection\.  | 
|  [io/table/sql/handler](ams-waits.waitio.md)  |  This event occurs when work has been delegated to a storage engine\.   | 
|  [synch/mutex/innodb/aurora\_lock\_thread\_slot\_futex](ams-waits.waitsynch.md)  |  This event occurs when one session has locked a row for an update, and another session tries to update the same row\.  | 