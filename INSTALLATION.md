# 🚀 Quick Guide - Smart Sender

## Installation in 3 Steps

### 📦 Option 1: Install XPI File (RECOMMENDED)

1. **Open Thunderbird**

2. **Go to Add-ons**
   - Click the menu ☰ (top right)
   - Select "Add-ons and Themes"
   - Or press `Ctrl+Shift+A`

3. **Install the addon**
   - Click the ⚙️ (gear) icon in the top right
   - Select "Install Add-on From File..."
   - Choose the `smart-sender.xpi` file
   - Confirm installation

✅ Done! The addon is active and ready to use.

---

### 🔧 Option 2: Debug Mode (for developers)

1. **Open Thunderbird**

2. **Go to Add-ons**
   - Menu ☰ → "Add-ons and Themes"

3. **Enable debug mode**
   - Click ⚙️ (gear)
   - Select "Debug Add-ons"

4. **Load the addon**
   - Click "Load Temporary Add-on..."
   - Go to the `smart-sender` folder
   - Select the `manifest.json` file

⚠️ **Note:** With this method the addon deactivates when you close Thunderbird.

---

## 🎯 How to use

**You don't need to do anything!** The addon learns automatically as you use Thunderbird.

### Example:

1. **First email to a new recipient:**
   - To: `john.doe@company.com`
   - From: `your.work@business.com`
   - Send the email ✅
   - Smart Sender memorizes this association

2. **Subsequent emails:**
   - Open new email
   - To: `john.doe@company.com`
   - Smart Sender automatically switches sender to `your.work@business.com` ⚡
   - Continue writing normally!

---

## ❓ Frequently Asked Questions

### Does the addon work immediately?
No, it needs to "learn" first. Send a few emails normally, then it will start suggesting the right account.

### Can I see what it has learned?
Yes! Click the Smart Sender button in the compose window toolbar to see all associations.

### What if I want to use a different account?
You can always manually change the account! Smart Sender doesn't block anything.

### Where is the data stored?
On your computer, in the Thunderbird profile. It never goes online.

---

## 🐛 Problems?

If something doesn't work:

1. **Check that the addon is active**
   - Go to "Add-ons and Themes"
   - Look for "Smart Sender"
   - Verify it's enabled

2. **Look at the logs**
   - Menu ☰ → More → Debug Console
   - Look for messages starting with "Smart Sender"

3. **Restart Thunderbird**
   - Sometimes you just need to close and reopen

---

## 🔄 Updating the Addon

### If installed via XPI file:

1. **Remove old version**
   - Add-ons → Smart Sender
   - Click `⋯` → "Remove"

2. **Install new version**
   - Gear icon ⚙️ → "Install Add-on From File..."
   - Select the new `smart-sender.xpi`

✅ **Your data is safe!** Associations remain in the Thunderbird profile.

### If loaded as temporary:

1. Close Thunderbird
2. Replace files in the `smart-sender` folder
3. Reopen Thunderbird
4. Reload the addon in Debug Add-ons

---

## 📊 Version

**Smart Sender v1.0.0**  
Compatible with Thunderbird 128+

Enjoy! 🎉
