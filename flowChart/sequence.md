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
[![](https://mermaid.ink/img/eyJjb2RlIjoic2VxdWVuY2VEaWFncmFtXG4gICAgQ3VzdG9tZXItPj4rQXBwTW9iaWxlOiBTY2FuIFFSQ29kZVxuICAgIEFwcE1vYmlsZS0-PitDdXN0b21lcjogSGksIHdoYXQgZG8geW91IG5lZWQ_XG4gICAgQ3VzdG9tZXItPj4rQXBwTW9iaWxlOiBCaWxsIFBsZWFzZVxuICAgIEFwcE1vYmlsZS0-PitBUEk6IFNlbmQgTWVzc2FnZShiaWxsKVxuICAgIEFQSS0-PitTZW5kZXJTTVM6U2VuZCBTTVNcbiAgICBBUEktPj4rU2VuZGVyU2xhY2s6U2VuZCBNZXNzYWdlXG4gICAgQVBJLT4-K1NlbmRlcldoYXRzQXBwOlNlbmQgTWVzc2FnZVxuICAgIEFQSS0-PitSZWNvcmRlcjpSZWNvcmQgQ2FsbFxuICAgIFNlbmRlclNNUy0-PitBUEk6U2VuZCBTTVNcbiAgICBTZW5kZXJTbGFjay0-PitBUEk6U2VuZCBNZXNzYWdlXG4gICAgU2VuZGVyV2hhdHNBcHAtPj4rQVBJOlNlbmQgTWVzc2FnZVxuICAgIFJlY29yZGVyLT4-K0FQSTpSZWNvcmQgQ2FsbFxuICAgIEFQSS0-PitDdXN0b21lcjogWW91ciBNZXNzYWdlIHdhcyBzZW5kZWQgICIsIm1lcm1haWQiOnsidGhlbWUiOiJkZWZhdWx0In19)](https://mermaid-js.github.io/mermaid-live-editor/#/edit/eyJjb2RlIjoic2VxdWVuY2VEaWFncmFtXG4gICAgQ3VzdG9tZXItPj4rQXBwTW9iaWxlOiBTY2FuIFFSQ29kZVxuICAgIEFwcE1vYmlsZS0-PitDdXN0b21lcjogSGksIHdoYXQgZG8geW91IG5lZWQ_XG4gICAgQ3VzdG9tZXItPj4rQXBwTW9iaWxlOiBCaWxsIFBsZWFzZVxuICAgIEFwcE1vYmlsZS0-PitBUEk6IFNlbmQgTWVzc2FnZShiaWxsKVxuICAgIEFQSS0-PitTZW5kZXJTTVM6U2VuZCBTTVNcbiAgICBBUEktPj4rU2VuZGVyU2xhY2s6U2VuZCBNZXNzYWdlXG4gICAgQVBJLT4-K1NlbmRlcldoYXRzQXBwOlNlbmQgTWVzc2FnZVxuICAgIEFQSS0-PitSZWNvcmRlcjpSZWNvcmQgQ2FsbFxuICAgIFNlbmRlclNNUy0-PitBUEk6U2VuZCBTTVNcbiAgICBTZW5kZXJTbGFjay0-PitBUEk6U2VuZCBNZXNzYWdlXG4gICAgU2VuZGVyV2hhdHNBcHAtPj4rQVBJOlNlbmQgTWVzc2FnZVxuICAgIFJlY29yZGVyLT4-K0FQSTpSZWNvcmQgQ2FsbFxuICAgIEFQSS0-PitDdXN0b21lcjogWW91ciBNZXNzYWdlIHdhcyBzZW5kZWQgICIsIm1lcm1haWQiOnsidGhlbWUiOiJkZWZhdWx0In19)
