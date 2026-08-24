                         INTERNET
                             |
                             |
                        Public IP
                             |
                             v
                    +----------------+
                    |  Jump Server   |
                    | Public +       |
                    | Private IP     |
                    +-------+--------+
                            |
                            |
                    +-------v--------+
                    | Azure Firewall |
                    +-------+--------+
                            |
                     +------v------+
                     |   VNet      |
                     | 10.0.0.0/16 |
                     +------+------+
                            |
                 +----------+----------+
                 |                     |
                 v                     v
          Jump Subnet          Workload Subnet
                                    |
                              Internal VMs
