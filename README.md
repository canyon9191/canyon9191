this is code to a file flooder



interface: "ens18"

sequences:
    one:
        send: true
        delay: 0
        time: 60

        eth:
            smac: "1a:c4:df:70:d8:a6"
            dmac: "ae:21:14:4b:3a:6d"

        ip:
            protocol: udp
            srcip: "10.50.0.3"
            dstip: "10.50.0.4"

            # Set static values for better performance.
            ttl:
                min: 64
                max: 64

            id:
                min: 0
                max: 0

        udp:
            srcport: 27000
            dstport: 8898

        payload:
            length:
                min: 61000
                max: 61000
                static: true
