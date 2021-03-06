# Frequently Asked Questions

### **Q**: Why some posts were missing? / Why did the bot respond to me so slowly?

**A**: Due to Telegram's restrictions, if too many messages are sent in a short period, the bot will get flood-controlled and have to wait for a certain time. Though the bot will retry, if still gets flood controlled, the message will be dropped. **Avoid subscribing to too many feeds, <u>especially in channels and groups</u> (they have a much stricter flood control threshold).**

### **Q**: How to use the bot in my channel or group?

**A**: Just add the bot to your channel or group and send commands. In a channel, "Post Messages" permission is required. If you are an anonymous administrator of a group, the bot needs to be an administrator too (no permission needed) to verify your identity.

### **Q**: The command list in Telegram "Menu" is outdated!

**A**: Send `/lang` and select language again. The bot will update your command list.

### **Q**: How is the performance of the bot? It appears to have a slight memory leak problem.

**A**: The bot is designed to be asynchronous, so it is lightweight and fast. Even if there are over 6000 feeds, the bot can still run on a single core VPS, with an incredibly low load average (~0.2) and approximate 350MB memory usage. The bot can still work fine in such a condition and its stability and usability will not be influenced. As for the memory leak problem, it is a [known issue](https://github.com/kurtmckee/feedparser/issues/287) of an upstream library `feedparser`, and it is not a bug of the bot.

### **Q**: Why do I still receive notifications even if I mute the subscription?

**A**: "Muted" notification is not aimed to disable the notifications, but to **make the notifications with no sound**. Due to the limitation of Telegram, disabling notifications completely on the sender side is not possible.
