# net
## donaldmcdougal's Java Network Utilities

Here is some code to help get you started:

    package com.donaldmcdougal.utils.net;
    
    import java.io.IOException;
    import java.net.InetAddress;
    
    public class App
    {
        public static void main(String[] args) throws IOException
        {
            InetAddress addr = NetUtils.guessLocalNetworkAddress();
            System.out.println("**********************************");
            System.out.println("Canonical host name: " + addr.getCanonicalHostName());
            System.out.println("Host address: " + addr.getHostAddress());
            System.out.println("Host name: " + addr.getHostName());
            System.out.println("Is any local address: " + addr.isAnyLocalAddress());
            System.out.println("Is link local: " + addr.isLinkLocalAddress());
            System.out.println("Is loopback: " + addr.isLoopbackAddress());
            System.out.println("Is multicast global: " + addr.isMCGlobal());
            System.out.println("Is multicast link local: " + addr.isMCLinkLocal());
            System.out.println("Is multicast node local: " + addr.isMCNodeLocal());
            System.out.println("Is multicast org local: " + addr.isMCOrgLocal());
            System.out.println("Is multicast site local: " + addr.isMCSiteLocal());
            System.out.println("Is multicast: " + addr.isMulticastAddress());
            System.out.println("Is reachable: " + addr.isReachable(30000));
            System.out.println("Is site local: " + addr.isSiteLocalAddress());
            System.out.println("**********************************");
        }
    }

Look at the source to learn more about the library.  There is only one class file.

To build a jar file of the project, first make sure Maven is installed, and then,
in a command line, change to the root directory of the project, and then type
'mvn package' and press the Enter key.
