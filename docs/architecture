# architecture

           (Home Router / ISP)
                  ^
                  |
            Host OS Internet
                  ^
                  |
        VirtualBox NAT (DC01 NIC1)
                  ^
                  |
      +--------------------------+
      | DC01 - Windows Server 2019|
      | AD DS / DNS / DHCP / RRAS |
      | NIC1: NAT (External)      |
      | NIC2: ADLAB (Internal)    |
      +--------------------------+
                  ^
                  |
        Internal Network: ADLAB
           172.16.0.0/24
                  ^
                  |
      +--------------------------+
      | CLIENT1 - Windows 10 Pro |
      | NIC1: ADLAB (Internal)   |
      +--------------------------+
