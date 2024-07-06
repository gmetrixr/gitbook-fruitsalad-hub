# Firewall Whitelisting

To ensure full functionality and seamless access to FruitSalad, certain hostnames need to be whitelisted in your organization's network.

Below is a list of hostnames that need to be added to your organization's whitelist:

## Essential

1. `learn.fruitsalad.ai` - This is the primary domain for accessing FruitSalad service
2. `*.fruitsalad.app` - The domains used by FruitSalad apps
3. `*.gmetri.com` - This is the domain of the underlying game engine
4. `*.vrgmetri.com` - This is the domain of the CDN used to serve assets

### **Multiplayer**

We use Agora as our service provider for all Multiplayer and Collaborative features. This is a must if you intend to use Multiplayer/Collaborative features such as Voice calls, Video calls, Screen-share, and Chat.

1. `*.agora.io`
2. `*.edge.agora.io`
3. `*.sd-rtn.com`
4. `*.edge.sd-rtn.com`
5. `web-1.ap.sd-rtn.com`
6. `web-2.ap.sd-rtn.com`
7. `ap-web-1.agora.io`
8. `ap-web-2.agora.io`
9. `webcollector-rtm.agora.io`
10. `logservice-rtm.agora.io`
11. `rtm.statscollector.sd-rtn.com`
12. `rtm.logservice.sd-rtn.com`

Additionally, you may also need to expose certain ports on your network if there are any restrictions added to the firewall

| Destination ports                                                                                                    | Port type |
| -------------------------------------------------------------------------------------------------------------------- | --------- |
| 80; 443; 3433; 4700 - 5000; 5668; 5669; 6080; 6443; 8667; 9591; 9593; 9601; 9667; 30011 - 30013 (for RTMP converter) | TCP       |
| 3478; 4700 - 5000                                                                                                    | UDP       |

## Optional Services <a href="#optional-services" id="optional-services"></a>

We use a number of services to keep GMetri systems functional and support advanced features.

### **Help / Support (Optional)**

These are required for any remote debugging issues at the user's end. We use Trackjs to collect any errors reported on users' devices.

1. `*.trackjs.com`

## Steps to Whitelist Hostnames:

1. **Consult IT Department:** Begin by consulting with your IT department or network administrator. They will have the necessary access and knowledge to make these changes.
2. **Add Hostnames to Whitelist:** Manually input each of the above hostnames into your whitelist settings. Ensure that all spellings are accurate to avoid any issues.
3. **Save and Apply Changes:** After adding all the required hostnames, save the changes and apply them to your network settings. It may take a few minutes for changes to propagate throughout your network.
4. **Verify Connectivity:** Try accessing FruitSalad from a device within your network to ensure that the whitelisting process has been successful. If you encounter any issues, recheck the entered hostnames for any inaccuracies.

### Need Assistance?

If you need further assistance or have questions about whitelisting these hostnames, please contact our support team at `support@fruitsalad.ai`. Our team is ready to assist you with any technical inquiries or guidance.
