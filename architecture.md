                                                  # NexusWave OS — Architecture Diagram

## High Level Flow

                +----------------+
                |   Observer     |
                |  (Signals)     |
                +-------+--------+
                        |
                        v
+--------------------------------------------------+
|                  Kernel                          |
|                                                  |
|  Scheduling  |  State  |  Quotas  |  Governance  |
+------------------+-------------------------------+
                   |
                   v
            +--------------+
            |   Planner    |
            |  (Goals →    |
            |   Tasks)     |
            +------+-------+
                   |
                   v
            +--------------+
            |  Executor    |
            | (Execution) |
            +--------------+

All actions pass through the kernel.
State is persisted after every step.
Signals are emitted continuously.

