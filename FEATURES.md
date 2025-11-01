# Features Guide - ডিজিটাল হিসাব খাতা

Complete guide to all features in the Digital Accounting Ledger.

## 📱 Quick Access Panel

Located on the left side of the screen, this panel provides instant access to key features:

### 💾 ব্যাকআপ (Backup)
**Purpose**: Export all your data for safekeeping

**How to use**:
1. Click the "💾 ব্যাকআপ" button
2. A JSON file will automatically download
3. File name format: `hishabkhata-backup-YYYY-MM-DD.json`
4. Save this file in a safe location

**What's included**:
- All cash sources and amounts
- All due/receivable entries
- All loan entries
- Complete transaction history
- Export timestamp

### 📥 রিস্টোর (Restore)
**Purpose**: Import previously backed up data

**How to use**:
1. Click the "📥 রিস্টোর" button
2. Select your backup JSON file
3. Confirm the restoration (warning: replaces current data)
4. Page will reload with restored data

**Important**: This will replace ALL current data. Make sure to backup first!

### 📊 CSV
**Purpose**: Export data in spreadsheet-compatible format

**How to use**:
1. Click the "📊 CSV" button
2. CSV file downloads automatically
3. Open in Excel, Google Sheets, or any spreadsheet software

**What's included**:
- Cash table with sources and amounts
- Dues table with names, amounts, and dates
- Loans table with names, amounts, and dates
- Summary section with totals

**Note**: File uses UTF-8 encoding to properly display Bengali text.

### 📈 চার্ট (Charts)
**Purpose**: Visualize your financial data

**How to use**:
1. Click the "📈 চার্ট" button
2. View interactive charts in popup

**Charts displayed**:

**Summary Distribution (Pie Chart)**:
- Blue: Current Cash (বর্তমান ক্যাশ)
- Yellow: Receivables (পাওনা বাকি)
- Red: Loans (লোন)

**Cash Sources Breakdown (Bar Chart)**:
- Shows each cash source
- Height represents amount
- Easy comparison of sources

### 📜 হিস্ট্রি (History)
**Purpose**: View transaction audit trail

**How to use**:
1. Click the "📜 হিস্ট্রি" button
2. View last 20 transactions in popup

**What's tracked**:
- Cash additions and deletions
- Deposits to cash sources
- Due entries added/removed
- Loan entries added/removed
- Data exports (backup, CSV)
- Data restores
- Each action includes timestamp and details

**Note**: System stores last 100 transactions.

### 🗑️ ক্লিয়ার (Clear All)
**Purpose**: Delete all data and start fresh

**How to use**:
1. Click the "🗑️ ক্লিয়ার" button
2. Confirm deletion (warning shown)
3. All data permanently removed
4. Page reloads with clean slate

**⚠️ Warning**: This cannot be undone! Always backup first.

---

## 🔍 Search Functionality

### Real-time Search
Located at the top of the page, below the title.

**How to use**:
1. Type in the search box
2. Results filter instantly as you type
3. Searches across all three tables simultaneously

**What it searches**:
- Cash source names
- Due person names
- Loan person names
- Amounts (if you type numbers)
- Dates

**Tips**:
- Search is case-insensitive
- Partial matches work (e.g., "রহ" finds "রহমান")
- Clear search box to show all entries

---

## 💰 Cash Management (ক্যাশ টাকা)

### Adding Cash Source
1. Click "উৎস যোগ করুন" button
2. Edit the source name (default: "সোর্স")
3. Enter amount
4. Changes auto-save

### Depositing Money
1. Click "ডিপোজিট" button on any cash row
2. Enter deposit amount in popup
3. Amount adds to existing balance
4. Transaction logged in history

### Editing Cash
- Click in any field to edit
- Changes save automatically
- Toast notification confirms save

### Deleting Cash Source
1. Click "ডিলিট" button
2. Source removed immediately
3. Deletion logged in history

---

## 📋 Dues/Receivables (বাকি হিসাব)

### Adding Due Entry
1. Click "ব্যক্তি যুক্ত করুন" button
2. Edit person name
3. Enter amount owed
4. Date/time automatically added

### Managing Dues
- Edit name or amount directly in table
- Delete when payment received
- All changes tracked in history

**Use case**: Track money others owe you (receivables)

---

## 💳 Loan Management (লোন এর হিসাব)

### Adding Loan
1. Click "লোন যুক্ত করুন" button
2. Edit lender name
3. Enter loan amount
4. Date/time automatically added

### Managing Loans
- Edit name or amount directly
- Delete when loan repaid
- All changes tracked in history

**Use case**: Track money you owe to others (payables)

---

## 📊 Summary Cards

Located at the bottom, shows real-time calculations:

### বর্তমান ক্যাশ (Current Cash)
- **Color**: Blue
- **Shows**: Sum of all cash sources
- **Formula**: Total of all amounts in Cash table

### পাওনা বাকি (Receivables)
- **Color**: Yellow
- **Shows**: Total money owed to you
- **Formula**: Sum of all due amounts

### লোন (Loans)
- **Color**: Red
- **Shows**: Total money you owe
- **Formula**: Sum of all loan amounts

### সর্বমোট (Grand Total)
- **Color**: Green
- **Shows**: Net worth
- **Formula**: Cash + Receivables - Loans

**Example**:
- Cash: ৳10,000
- Receivables: ৳5,000
- Loans: ৳3,000
- **Grand Total**: ৳12,000 (10,000 + 5,000 - 3,000)

---

## 🌓 Theme Switching

### Toggle Theme
Click the moon (🌙) or sun (☀️) icon in top-left corner.

**Light Theme**:
- Default pink background (#fff9f9)
- Dark text
- Standard table colors

**Dark Theme**:
- Dark background (#1a1a1a)
- Light text (#e0e0e0)
- Adjusted table and card colors

**Preference**: Your theme choice is saved and persists across sessions.

---

## 💡 Pro Tips

### Data Safety
1. **Regular Backups**: Export backup weekly
2. **Before Major Changes**: Always backup first
3. **Test Restore**: Try restoring on a test device

### Organization
1. **Descriptive Names**: Use clear source/person names
2. **Regular Updates**: Update amounts as transactions occur
3. **Clean Old Entries**: Delete completed dues/loans

### Performance
1. **Limit History**: System auto-limits to 100 entries
2. **Clear Old Data**: Periodically export and clear
3. **Use Search**: Find entries quickly instead of scrolling

### Analysis
1. **Check Charts**: Visualize your financial distribution
2. **Review History**: Track your financial activities
3. **Monitor Grand Total**: Watch your net worth trend

---

## 🔐 Privacy & Security

### Data Storage
- All data stored locally in browser
- No server uploads
- No internet required (except initial load)
- Data never leaves your device

### Backup Security
- JSON backups are plain text
- Store backups securely
- Don't share backup files publicly
- Consider encrypting sensitive backups

### Browser Data
- Data tied to specific browser
- Clearing browser data deletes everything
- Use backup/restore to move between browsers
- Private browsing won't save data

---

## 🐛 Troubleshooting

### Data Not Saving
- Check browser allows localStorage
- Disable private/incognito mode
- Check browser storage quota

### Theme Not Persisting
- Same as above (uses localStorage)
- Check cookies/storage settings

### Charts Not Showing
- Ensure internet connection (loads Chart.js)
- Check browser JavaScript enabled
- Try different browser

### CSV Not Opening Correctly
- Open with UTF-8 encoding
- Use "Import" feature in Excel (not double-click)
- Try Google Sheets for better Bengali support

---

## 📱 Mobile Usage

### Touch Gestures
- Tap to edit fields
- Scroll tables horizontally if needed
- Action buttons accessible from menu

### Responsive Design
- Tables stack on small screens
- Buttons adjust size
- Charts resize automatically

### Best Practices
- Use in portrait mode for best experience
- Backup regularly (export to cloud storage)
- Consider bookmark for easy access

---

## 🎓 Tutorial Walkthrough

### First Time Setup
1. Open index.html in browser
2. Click theme toggle to choose preferred theme
3. Add your first cash source
4. Add any dues/loans
5. Create your first backup

### Daily Usage
1. Open the app
2. Add/update transactions
3. Use search to find entries
4. Check summary cards for totals
5. Review history periodically

### Weekly Maintenance
1. Export CSV for records
2. Create JSON backup
3. Delete completed dues/loans
4. Review charts for insights

---

**Need Help?** Check the main [README.md](README.md) or create an issue on GitHub.
