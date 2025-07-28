# 🎯 Qalam Survey Auto-Fill Scripts 🤖
*Because clicking "Good" 47 times isn't anyone's idea of fun!*

```
    ╔══════════════════════════════════════════╗
    ║  🎪 WELCOME TO THE SURVEY AUTOMATION    ║
    ║      CIRCUS OF PRODUCTIVITY! 🎪         ║
    ╚══════════════════════════════════════════╝
```

## 🎬 What's This Magic Show About?

Transform your boring survey-filling experience from this:
```
😩 Click... click... "Good"... click... "Good"... *yawn*... click...
```

To THIS:
```
✨ *POOF!* ✨ All surveys filled! Time for coffee! ☕
```

---

## 🚀 **FEATURES THAT'LL BLOW YOUR MIND** 🚀

```
    🔍 AUTO-DETECTION     │  Finds surveys like a bloodhound
    🎯 AUTO-FILL          │  Fills forms faster than The Flash  
    💬 AUTO-COMMENT       │  Drops "Good" like it's hot
    📤 AUTO-SUBMIT        │  Sends it off to cyber-space
    🔄 AUTO-NAVIGATION    │  Rinse and repeat, baby!
```

---

## 🎪 **INSTALLATION CIRCUS** 🎪

### 🎭 **Step 1: Get Your Tampermonkey Sidekick**

Pick your browser weapon of choice:

```
🌟 Chrome Warriors    → Chrome Web Store
🦊 Firefox Fighters  → Firefox Add-ons  
🔷 Edge Enthusiasts  → Microsoft Edge Add-ons
```

> **🎪 RINGMASTER'S TIP:** Don't forget to toggle on Developer Mode and pin Tampermonkey to your browser! It's like giving your circus performer a spotlight! 🎯

### 🎪 **Step 2: Install the Magic Scripts**

```
┌─ SCRIPT INSTALLATION DANCE ─┐
│                              │
│ 1. 👆 Click Tampermonkey     │
│ 2. 🆕 "Create a new script"  │
│ 3. 🗑️  Delete template code   │
│ 4. 📋 Copy-paste Script #1   │
│ 5. 💾 Save (Ctrl+S)         │
│ 6. 🔄 Repeat for Script #2   │
│                              │
└──────────────────────────────┘
```

---

## 🎊 **HOW TO USE THIS MAGICAL CONTRAPTION** 🎊

```
🎯 MISSION CONTROL SEQUENCE:
═══════════════════════════════

Step 1: 🚪 Log into Qalam NUST
Step 2: 🧭 Navigate to: qalam.nust.edu.pk/student/qa/feedback  
Step 3: 🍿 Grab popcorn and watch the magic happen!
Step 4: ☕ Make coffee while robots do your work

    ┌─────────────────────────────┐
    │   🤖 BEEP BOOP WORKING...   │
    │                             │
    │   ▓▓▓▓▓▓▓▓▓▓ 100%          │
    │                             │
    │   ✅ All surveys complete!   │
    └─────────────────────────────┘
```

---

## 🎨 **CUSTOMIZATION PLAYGROUND** 🎨

### 🎯 **Change Your Rating Style**

Want to be more generous with your ratings? Here's the treasure map:

```javascript
// 🎪 THE MAGIC HAPPENS HERE 🎪
for (const [index, row] of rows.entries()) {
    const radios = row.querySelectorAll('input[type="radio"]');
    if (radios.length > 0) {
        radios[0].checked = true;  // 👈 THE MAGIC NUMBER!
        // 🎭 RATING PERSONALITY OPTIONS:
        // radios[0] = "Meh, it's okay" 😐
        // radios[1] = "Pretty decent" 🙂  
        // radios[2] = "Not bad at all" 😊
        // radios[3] = "Actually quite good!" 😄
        // radios[4] = "ABSOLUTELY FANTASTIC!" 🤩
        
        radios[0].dispatchEvent(new Event('change', { bubbles: true }));
        console.log(`✅ Selected first option for row ${index + 1}`);
    }
}
```

### 💬 **Customize Your Comments**

Tired of "Good"? Spice it up!

```javascript
// 🎪 COMMENT CUSTOMIZATION STATION 🎪
commentField.value = "Good";  

// 🎭 ALTERNATIVE PERSONALITIES:
// "Absolutely brilliant!" 🌟
// "10/10 would recommend" ⭐  
// "This exceeded my expectations!" 🚀
// "Simply outstanding work!" 👏
// "Keep up the excellent work!" 💪
```

---

## 🔧 **WHEN THINGS GO WONKY** 🔧

```
🚨 TROUBLESHOOTING HEADQUARTERS 🚨
═══════════════════════════════════

🔍 Problem Detective Mode:
   Press F12 → Check Console → Look for error messages

🏗️ Structure Changed?
   Qalam updated? Scripts might need a tune-up!

⚔️ Script Wars?  
   Check for conflicting scripts in the neighborhood

🛠️ Manual Override:
   Some surveys are special snowflakes ❄️
```

---

## ⚠️ **IMPORTANT CIRCUS RULES** ⚠️

```
┌────────────────────────────────────┐
│  🎪 RESPONSIBLE AUTOMATION RULES   │
│                                    │
│  📚 Educational purposes only      │
│  🤝 Use ethically & responsibly    │  
│  📅 Works as of April 2025*        │
│  🔄 May need updates if UI changes │
│                                    │
│  *Subject to Qalam's mood swings   │
└────────────────────────────────────┘
```

---

## 🎪 **THE CREDITS ROLL** 🎪

```
    🎬 STARRING 🎬
    
    💻 MIT License        │ The legal superhero
    🤖 GPT Assistant      │ The creative genius  
    🎯 You                │ The awesome user!
    
    🎪 SPECIAL THANKS TO COFFEE ☕ 
    For making this README possible at 2 AM
```

---

```
╔══════════════════════════════════════════════════════════╗
║                                                          ║
║   🎊 CONGRATULATIONS! YOU'RE NOW A SURVEY NINJA! 🎊     ║
║                                                          ║
║        May your surveys be swift and your               ║
║           coffee be strong! ☕✨                        ║
║                                                          ║
╚══════════════════════════════════════════════════════════╝
```

---

