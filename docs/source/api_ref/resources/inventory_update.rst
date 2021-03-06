Inventory Update
================

Description
-----------

This resource is used for managing and executing inventory updates via Tower.

Fields Table
------------
.. <table goes here>

+-----------------+----------------------------------------------------------------------------------------+----------------------------+----------+-------+-----------+---------+
|name             |type                                                                                    |help_text                   |read_only |unique |filterable |required |
+=================+========================================================================================+============================+==========+=======+===========+=========+
|inventory_source |Resource inventory_source                                                               |The inventory_source field. |False     |False  |True       |True     |
+-----------------+----------------------------------------------------------------------------------------+----------------------------+----------+-------+-----------+---------+
|name             |String                                                                                  |The name field.             |True      |False  |True       |False    |
+-----------------+----------------------------------------------------------------------------------------+----------------------------+----------+-------+-----------+---------+
|launch_type      |Choices: manual,relaunch,relaunch,callback,scheduled,dependency,workflow,sync,scm       |The launch_type field.      |True      |False  |True       |True     |
+-----------------+----------------------------------------------------------------------------------------+----------------------------+----------+-------+-----------+---------+
|status           |Choices: new,pending,waiting,running,successful,failed,error,canceled                   |The status field.           |True      |False  |True       |True     |
+-----------------+----------------------------------------------------------------------------------------+----------------------------+----------+-------+-----------+---------+
|job_explanation  |String                                                                                  |The job_explanation field.  |True      |False  |True       |False    |
+-----------------+----------------------------------------------------------------------------------------+----------------------------+----------+-------+-----------+---------+
|created          |String                                                                                  |The created field.          |True      |False  |True       |False    |
+-----------------+----------------------------------------------------------------------------------------+----------------------------+----------+-------+-----------+---------+
|elapsed          |String                                                                                  |The elapsed field.          |True      |False  |True       |False    |
+-----------------+----------------------------------------------------------------------------------------+----------------------------+----------+-------+-----------+---------+
|source           |Choices: ,file,scm,ec2,vmware,gce,azure,azure_rm,openstack,satellite6,cloudforms,custom |The source field.           |False     |False  |True       |True     |
+-----------------+----------------------------------------------------------------------------------------+----------------------------+----------+-------+-----------+---------+

.. <table goes here>

API Specification
-----------------
.. autoclass:: tower_cli.resources.inventory_update.Resource
   :members: cancel, delete, get, list, monitor, relaunch, status, wait
