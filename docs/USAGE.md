# 📖 Usage Guide

Complete usage guide for all tools in the **tele-latino** repository.

---

## 🧮 Calculator Tool

### How to Open

**Option 1: Online (Easiest)**
```
Visit: https://gettelelatino.com/
```

**Option 2: Local File**
1. Download the repository
2. Open `calculator.html` in your browser
3. Start using!

**Option 3: Development Server**
```bash
python -m http.server 8000
# Then visit: http://localhost:8000/calculator.html
```

---

### Basic Usage

#### Using Mouse/Touchscreen

1. **Enter Numbers**
   - Click number buttons (0-9)
   - Example: Click `5`, then `3` → Display shows `53`

2. **Choose Operation**
   - Click operator button: `+` `-` `×` `÷`
   - Example: After `53`, click `+`

3. **Enter Second Number**
   - Click more number buttons
   - Example: Click `2` → Display shows `2`

4. **Calculate Result**
   - Click `=` button
   - Example: `53 + 2 = 55` ✅

5. **Clear or Delete**
   - Click `AC` to clear everything
   - Click `DEL` to delete last digit

#### Step-by-Step Example

```
Step 1: Click 5                    Display: 5
Step 2: Click +                    Display: 5 +
Step 3: Click 3                    Display: 3
Step 4: Click =                    Display: 8 ✅
```

---

### Using Keyboard (Faster!)

The calculator supports full keyboard input!

| Key | Action | Example |
|-----|--------|---------|
| `0`-`9` | Enter numbers | Type `42` |
| `.` | Add decimal | Type `3.14` |
| `+` | Add | Type `10 + 5` |
| `-` | Subtract | Type `10 - 3` |
| `*` | Multiply | Type `5 * 6` |
| `/` | Divide | Type `20 / 4` |
| `Enter` or `=` | Calculate | Press to get result |
| `Backspace` | Delete last digit | `1234` → `123` |
| `Escape` or `C` | Clear all | Reset calculator |

---

### Keyboard Examples

**Example 1: Simple Addition**
```
Type: 15 + 8
Press: Enter
Result: 23 ✅
```

**Example 2: Decimal Numbers**
```
Type: 3.5 * 2
Press: Enter
Result: 7 ✅
```

**Example 3: Chain Calculations**
```
Type: 100 - 25
Press: Enter (Result: 75)
Type: + 50
Press: Enter
Result: 125 ✅
```

**Example 4: Correct a Mistake**
```
Type: 123 (oops, meant 12)
Press: Backspace
Type: 4
Result: 124 ✅
```

---

### Advanced Features

#### Decimal Numbers
- Supports unlimited decimal places
- Example: `3.14159 × 2 = 6.28318`
- Prevents multiple decimals: `3.14.15` → not allowed ✅

#### Long Calculations
- Chain operations together
- Example: `10 + 5` then press `×` (auto-calculates) → `× 3` → `=` gives `45`

#### View Previous Operation
- Top line shows your previous operation
- Helps you remember what you're calculating
- Example: Shows `15 +` while you enter the second number

#### Real-time Display
- Display updates instantly as you type
- Large, readable numbers
- Shows decimals and negative numbers clearly

---

### Common Calculations

#### Converting Temperatures (Quick Hack)
```
Celsius to Fahrenheit: (C × 9 ÷ 5) + 32
Example: 25°C
25 × 9 ÷ 5 + 32 = 77°F ✅
```

#### Calculating Percentages
```
Find 20% of 50:
50 × 20 ÷ 100 = 10 ✅

Calculate tip (15% of $80):
80 × 15 ÷ 100 = 12 ✅
```

#### Area & Volume
```
Rectangle area (length × width):
12 × 8 = 96 sq units ✅

Cube volume (length × width × height):
5 × 5 × 5 = 125 cubic units ✅
```

---

### Tips & Tricks

#### ⚡ Speed Tips
- Use keyboard for faster calculations
- Paste numbers with Ctrl+V (if supported)
- Chain operations without pressing `=`

#### 🎯 Accuracy
- Calculator uses JavaScript's precision
- Very large numbers might show in scientific notation
- For precise financial calculations, round to 2 decimals

#### 🔄 Undo Mistakes
- Press `Backspace` to delete last digit
- Press `Escape` to clear everything
- No true "undo" - start fresh with `Escape`

#### 💡 Keyboard Shortcuts
```
Quick Reference:
- Numbers: 0-9, .
- Operations: +, -, *, /
- Calculate: Enter or =
- Delete: Backspace
- Clear: Escape
```

---

### Troubleshooting

#### "Calculator not responding"
- ✅ Reload the page
- ✅ Clear browser cache
- ✅ Try a different browser

#### "Numbers appear weird"
- ✅ Very large calculations show in scientific notation (normal)
- ✅ This is how computers display huge numbers
- ✅ Example: `9999999999 × 9999999999 = 9.999999980000001e+19`

#### "Decimal precision issues"
- ✅ Computers have tiny rounding errors (normal)
- ✅ Example: `0.1 + 0.2` might show `0.30000000000000004`
- ✅ This is expected in all calculators

#### "Keyboard not working"
- ✅ Click in the calculator display area first
- ✅ Make sure NumLock is on (for number pad)
- ✅ Try mouse input instead

---

### Comparison with Other Calculators

| Feature | tele-latino | Windows Calc | Phone Calc |
|---------|-------------|--------------|-----------|
| Keyboard Support | ✅ Full | ✅ Full | ❌ Touch only |
| Responsive | ✅ All devices | ❌ Desktop only | ✅ Mobile |
| No Download | ✅ Browser-based | ❌ Windows only | ❌ App required |
| Beautiful Design | ✅ Modern UI | ❌ Plain | ⚠️ Basic |
| Open Source | ✅ Yes | ❌ No | ❌ No |

---

## 🎓 Learning the Code

Want to understand how the calculator works?

### HTML Structure (`calculator.html`)
```html
<!-- Display section -->
<div class="display">
  <div class="previous-operand">15 +</div>
  <div class="current-operand">8</div>
</div>

<!-- Buttons -->
<button onclick="appendNumber('7')">7</button>
<button onclick="chooseOperation('+')">+</button>
<button onclick="compute()">=</button>
```

### JavaScript Logic
```javascript
// Add number to display
function appendNumber(number) {
  currentOperand += number;
  updateDisplay();
}

// Choose an operation
function chooseOperation(op) {
  operation = op;
  previousOperand = currentOperand;
  currentOperand = '';
}

// Calculate the result
function compute() {
  // ... math logic here
  result = previousOperand + operation + currentOperand;
}
```

---

## 📱 Mobile Usage

The calculator is fully responsive!

### Phone/Tablet Tips
- 📱 Tap buttons to use
- 🔄 Rotate screen for best view
- ⌨️ Use on-screen keyboard
- 👆 Use two fingers to zoom if needed
- 🔌 Works offline once loaded

### Best Experience
- Portrait mode recommended
- Larger buttons for easy tapping
- Landscape mode shows larger display
- Works with all modern mobile browsers

---

## 🚀 Next Steps

After mastering the calculator:

1. ✅ Try keyboard shortcuts
2. ✅ Explore the source code
3. ✅ Customize colors and styles
4. ✅ Share with friends
5. ✅ Contribute improvements on GitHub

---

## 📚 See Also

- [Installation Guide](./INSTALLATION.md)
- [README](../README.md)
- [Contributing Guide](../CONTRIBUTING.md)

---

## 🎯 Quick Keyboard Reference

```
NUMBERS:     0 1 2 3 4 5 6 7 8 9 .
OPERATIONS:  + - * /
FUNCTIONS:   Enter(=) Backspace(DEL) Escape(AC)
```

---

Made with ❤️ by [Abdulrazaq Mehrwood](https://gettelelatino.com/)

*Last updated: 2026*
