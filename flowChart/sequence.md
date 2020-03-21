```mermaid
sequenceDiagram
    Customer->>+AppMobile: Scan QRCode
    AppMobile->>+Customer: Hi, what do you need?
    Customer->>+AppMobile: Bill Please
    AppMobile->>+API: Send Message(bill)
    API->>+SenderSMS:Send SMS
    API->>+SenderSlack:Send Message
    API->>+SenderWhatsApp:Send Message
    API->>+Recorder:Record Call
    SenderSMS->>+API:Send SMS
    SenderSlack->>+API:Send Message
    SenderWhatsApp->>+API:Send Message
    Recorder->>+API:Record Call
    API->>+Customer: Your Message was sended  
```