# PeerToPeerPicSharing PicPeer
This project is heavily based on multipeer networking using MultipeerConnectivity, which allows users to make direct connections to those nearby to them and share pictures with. 



Again, a few lines to help the nerds;


//
(serviceType: "vishy-projectcall", discoveryInfo: nil, session: mcSession)
func session(_ session: MCSession, peer peerID: MCPeerID, didChange state: MCSessionState) {
        switch state {
        
        case.connected:
            print("Connected: \(peerID.displayName)")
            
        case.connecting:
            print("Connecting: \(peerID.displayName)")
            
        case.notConnected:
            print("Not Connected: \(peerID.displayName)")
            
        @unknown default:
            print("Unknown state received: \(peerID.displayName)")
            
        }
    }
    
