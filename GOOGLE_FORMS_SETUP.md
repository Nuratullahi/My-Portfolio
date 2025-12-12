# Google Forms Integration Setup Guide

## 📋 Follow These Steps to Connect Your Contact Form

Your portfolio contact form is now ready to integrate with Google Forms. Follow these simple steps:

---

## Step 1: Create Your Google Form

1. **Go to Google Forms:** https://forms.google.com
2. **Sign in** with your account: `nuratullahi.ao@gmail.com`
3. **Click** the **"+ Blank"** button to create a new form
4. **Title your form:** "Portfolio Contact Form"

---

## Step 2: Add Form Questions (EXACT ORDER)

Add these questions in this EXACT order with these EXACT titles:

### Question 1: Name
- **Question type:** Short answer
- **Question text:** "Your Name"
- **Make it:** Required ✓

### Question 2: Email
- **Question type:** Short answer
- **Question text:** "Email Address"
- **Make it:** Required ✓

### Question 3: Company
- **Question type:** Short answer
- **Question text:** "Company/Organization"
- **Make it:** Optional (no checkmark)

### Question 4: Service
- **Question type:** Multiple choice
- **Question text:** "How Can I Help You?"
- **Options (add these exactly):**
  - Salesforce Implementation
  - Business Analysis
  - Process Optimization
  - Training
  - Other
- **Make it:** Required ✓

### Question 5: Project Details
- **Question type:** Paragraph
- **Question text:** "Project Details"
- **Make it:** Required ✓

### Question 6: Timeline
- **Question type:** Short answer
- **Question text:** "Timeline"
- **Make it:** Optional (no checkmark)

---

## Step 3: Configure Form Settings

1. **Click** the **⚙️ Settings** icon (top right)
2. **Under "Responses":**
   - ✓ Check "Collect email addresses"
   - ✓ Check "Send respondents a copy of their response"
3. **Under "Presentation":**
   - Set confirmation message: "Thank you for contacting me! I will review your message and get back to you shortly."
4. **Click "Save"**

---

## Step 4: Get Your Form IDs

1. **Click** the **Send** button (top right)
2. **Click** the **< >** (embed) icon
3. **You'll see HTML code** - DON'T use this yet
4. **Instead, click "Copy" on the iframe src URL**

The URL looks like:
```
https://docs.google.com/forms/d/e/1FAIpQLSc_XXXXX_FORM_ID_XXXXX/viewform
```

5. **Copy the FORM_ID** (the part after `/e/` and before `/viewform`)

Example: `1FAIpQLSc_abcdefghijklmnop1234567890`

---

## Step 5: Get Entry IDs for Each Field

This is the IMPORTANT part:

1. **Click "Preview"** (👁️ eye icon at top)
2. **Right-click** on the page → **View Page Source**
3. **Press Ctrl+F** (or Cmd+F) and search for: `entry.`

You'll find lines like:
```html
<input type="text" name="entry.123456789" ...>
<input type="email" name="entry.987654321" ...>
```

4. **Find and note down** the entry IDs for each field in order:
   - Name field: `entry.XXXXXXXX`
   - Email field: `entry.XXXXXXXX`
   - Company field: `entry.XXXXXXXX`
   - Service field: `entry.XXXXXXXX`
   - Details field: `entry.XXXXXXXX`
   - Timeline field: `entry.XXXXXXXX`

---

## Step 6: Update Your Portfolio Code

**Send me these values and I'll update your portfolio:**

```
FORM_ID: 1FAIpQLSc_YOUR_FORM_ID_HERE

NAME_ID: entry.123456789
EMAIL_ID: entry.987654321
COMPANY_ID: entry.111111111
SERVICE_ID: entry.222222222
DETAILS_ID: entry.333333333
TIMELINE_ID: entry.444444444
```

**Just paste these values here and I'll update your code automatically!**

---

## Step 7: Set Up Email Notifications

To receive emails when someone submits:

1. **In your Google Form**, click **Responses** tab
2. **Click** the three dots (⋮) menu
3. **Select** "Get email notifications for new responses"
4. **You're done!** You'll now receive emails at `nuratullahi.ao@gmail.com`

---

## Step 8: View Responses

All form submissions are saved in:
1. **Google Forms → Responses tab** (view individual responses)
2. **Click "View in Sheets"** to create a Google Spreadsheet with all responses

---

## 🎯 Quick Summary

**What you need to do:**
1. ✅ Create Google Form with 6 questions (in exact order above)
2. ✅ Enable email notifications
3. ✅ Get Form ID and Entry IDs
4. ✅ Send me those IDs (I'll update the code)
5. ✅ Test the form!

**What happens after setup:**
- ✅ All form submissions saved to Google Forms
- ✅ Email notification sent to you for each submission
- ✅ Respondent receives confirmation email
- ✅ All data organized in Google Sheets (optional)

---

## 🚨 Important Notes

- **Keep your Google Form public** (Anyone can respond)
- **Don't change question order** after getting entry IDs
- **Test your form** before announcing your portfolio
- **Check spam folder** if you don't receive notifications

---

## 📧 Need Help?

If you encounter any issues:
1. Double-check question order matches exactly
2. Ensure all entry IDs are correct
3. Verify email notifications are enabled
4. Test by submitting a form yourself

**Ready to integrate? Just send me your Form ID and Entry IDs!** 🚀
