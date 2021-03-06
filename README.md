

[logo]: https://cdn.cai.tools.sap/brand/sapcai/sap-cai-black.svg "SAP Conversational AI"

![alt text][logo]
 
# 🚨 Sunset of Open Source SDKs for SAP Conversational AI 
 
SAP Conversational AI provides several SDKs, which are all open-source and hosted on GitHub.  
Starting from January 2021, please note that we inform you that the SDKs will not be available anymore and the public repository of the project will be archived from GitHub.  

## ✨ Why are we sunsetting our SDKs? 
 
Firstly, we noticed over the past year that these SDKs were not used much by our users.  
This is because our platform usage has become easier, including the APIs. 

Secondly, our APIs have undergone major changes. We would need to adapt the SDKs in order to keep them working, which will lead to a significant cost from our side. 

Hence, we decided to sunset this open source version starting from January 2021.  
 
## ✨ What does it mean for me as a user? 
 
Any changes in our API’s will not be reflected in our SDKs. Hence, the code might not work unless you adjust the same.  

## ✨ What are the next steps? 
 
If you are interested in taking the ownership of the project on GitHub, please get in touch with us and we can discuss the process. Otherwise, if there are no objections from anyone, we would archive the project following the open source sunset process.  

Please use the platform SAP Answers if you have any other questions related to this topic. 
 
Happy bot building! 
 
The SAP Conversational AI team

---

# SAP Conversational AI - SDK Ruby

SAP Conversational AI official SDK in Ruby

## Synospis

This module is a wrapper around the [SAP Conversational AI](https://cai.tools.sap) API, and allows you to:
* [Analyse your text](https://github.com/SAPConversationalAI/SDK-Ruby/wiki/01---Analyse-text)
* [Manage a conversation](https://github.com/SAPConversationalAI/SDK-Ruby/wiki/02---Manage-conversation)
* [Receive and send messages](https://github.com/SAPConversationalAI/SDK-Ruby/wiki/03---Receive-and-send-messages)

## Installation

This gem supports ruby 2.3+.

```bash
gem install Sapcai
```

You can now use the SDK in your code. All you need is your bot's token. In case you have enabled our versioning feature in the settings of your bot, you can refer to our [versioning documentation](https://cai.tools.sap/docs/concepts/versioning) to learn how to select the appropriate token for you versions and environments.

Using the entire SDK:
```ruby
require 'sapcai'

client = Sapcai::Client.new('YOUR_TOKEN')

client.request.analyse_text('Hi')
client.connect.broadcast_message('Hello')
```

Extracting one single API:
```ruby
require 'sapcai'

request = Sapcai::Request.new('YOUR_TOKEN')
request.analyse_text('Hi')

connect = Sapcai::Connect.new('YOUR_TOKEN')
connect.broadcast_message('Hi')
```

## More

You can view the whole API reference at [cai.tools.sap/docs/](https://cai.tools.sap/docs/api-reference).

You can follow us on Twitter at [@sapcai](https://twitter.com/sapcai) for updates and releases.


## License

Copyright (c) [2019] [SAP Conversational AI](https://cai.tools.sap)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to tsuse, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
