# Wireshark_notes

- The basic tool for observing the messages exchanged between executing protocol entities is called a `packet sniffer`
    - It observes messages being sent and received by applications and protocols, but **never** sends packets itself
    - Instead, it receives/sent `a copy of packets`

- Structure of a packet sniffer:
1. **packet capture library**: receives a copy of every **link-layer** frame that is sent from or received by your computer
    - Reacall: messages exchanged by higher layer protocols (HTTP, TCP...) are eventually `encapsulated` in `link-layer` frames
    - Hence, **capturing all link-layer frames** thus gives you all messages sent/received across the monitored link from/by all protocols and applications executing in your computer

2. **packet analyzer**: displays the `contents` of all fields within a protocol message

## Wireshark packet sniffer
- Wireshark is a **packet analyzer** that uses a **packet capture library**
- Allowing us to `display` the contents of messages being sent/received from/by protocols at different levels of the `protocol stack`

### Getting Wireshark
- Download and install the Wireshark software: http://www.wireshark.org/download.html

### Running Wireshark
- under the `Capture section`, there is a list of **interfaces**
- Example: “Wi-Fi en0” which is the `interface for Wi-Fi access`. 

### Five major components in Wireshark interface 
![Screen Shot 2023-03-02 at 2 22 29 PM](https://user-images.githubusercontent.com/75557717/222572975-fc6ceb81-7aef-4f15-bc69-a757bd84ba72.png)
