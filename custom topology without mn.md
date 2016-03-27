### mininet- Custom Topology without MN
source : https://www.youtube.com/watch?v=yHUNeyaQKWY&index=2&list=PLyiXK9gbG3lCGVMsxNGidIabUnZeOq9hD

<pre>
mininet@10-0-2-15:~/mininet/examples$ 
</pre>

open the file in the directory emptynet.py , emptynet.py open the file in the directory <b>/mininet/examples$</b> then open it with nano editor

<pre>
mininet@10-0-2-15:~/mininet/examples$<b>nano emptynet.py</b> 
</pre>

<pre>
#!/usr/bin/python

"""
This example shows how to create an empty Mininet object
(without a topology object) and add nodes to it manually.
"""

from mininet.net import Mininet
from mininet.node import Controller
from mininet.cli import CLI
from mininet.log import setLogLevel, info

def emptyNet():

    "Create an empty network and add nodes to it."

    net = Mininet( controller=Controller )

    info( '*** Adding controller\n' )
    net.addController( 'c0' )

    info( '*** Adding hosts\n' )
    h1 = net.addHost( 'h1', ip='10.0.0.1' )
    h2 = net.addHost( 'h2', ip='10.0.0.2' )

    info( '*** Adding switch\n' )
    s3 = net.addSwitch( 's3' )

    info( '*** Creating links\n' )
    net.addLink( h1, s3 )
    net.addLink( h2, s3 )

    info( '*** Starting network\n')
    net.start()

    info( '*** Running CLI\n' )
    CLI( net )
    info( '*** Stopping network' )

if __name__ == '__main__':
    setLogLevel( 'info' )
    emptyNet()

</pre>

####Default Controller
<pre>
<b>
net = Mininet( controller=Controller )

    info( '*** Adding controller\n' )
    net.addController( 'c0' )
</b>
</pre>

####Host
<pre>
<b>
 info( '*** Adding hosts\n' )
    h1 = net.addHost( 'h1', ip='10.0.0.1' )
    h2 = net.addHost( 'h2', ip='10.0.0.2' )
</b>
</pre>