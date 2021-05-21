Monitor Procrastinate in a real environment
-------------------------------------------

The baseline: a smoke test
^^^^^^^^^^^^^^^^^^^^^^^^^^

The command line interface gives a basic monitoring available through the console.

.. code-block:: console

    $ procrastinate healthchecks
    App configuration: OK
    DB connection: OK
    Found procrastinate_jobs table: OK

The administration shell
^^^^^^^^^^^^^^^^^^^^^^^^

The procrastinate shell is a tool to administrate jobs and overview queues and tasks.
It is an interactive shell that you can run with the following command.

*Experimental feature*.

.. code-block:: console

    $ procrastinate shell
    Welcome to the procrastinate shell.   Type help or ? to list commands.

    procrastinate> help

    Documented commands (type help <topic>):
    ========================================
    EOF  cancel  exit  help  list_locks  list_jobs  list_queues  list_tasks  retry

As usual, you should use ``--app`` argument or ``PROCRASTINATE_APP`` environment
variable to specify the application you want to use (see `command_line`).

There are commands to list all the jobs (``list_jobs``), tasks (``list_tasks``),
queues (``list_queues``) and locks (``list_locks``).
And commands to retry (``retry``) & cancel (``cancel``) a specific job.

You can get help for a specific command *cmd* by typing ``help cmd``.

The administration web portal
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

*Not yet, maybe someday.*
