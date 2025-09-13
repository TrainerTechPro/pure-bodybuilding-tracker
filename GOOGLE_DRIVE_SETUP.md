# Google Drive Cloud Sync Setup Guide

This guide will help you set up Google Drive integration for automatic cloud backup and cross-device sync.

## Prerequisites

- Google account
- 5 minutes of setup time

## Step 1: Create a Google Cloud Project

1. **Go to Google Cloud Console**: https://console.cloud.google.com/
2. **Create a new project** or select an existing one
3. **Enable the Drive API**:
   - Navigate to "APIs & Services" > "Library"
   - Search for "Google Drive API"
   - Click on it and press "Enable"

## Step 2: Create OAuth 2.0 Credentials

1. **Go to Credentials**:
   - Navigate to "APIs & Services" > "Credentials"
   - Click "Create Credentials" > "OAuth 2.0 Client IDs"

2. **Configure OAuth consent screen** (if not done):
   - Click "Configure Consent Screen"
   - Choose "External" for user type
   - Fill in required fields:
     - App name: "Pure Bodybuilding Tracker"
     - User support email: Your email
     - Developer contact: Your email
   - Add scopes: `https://www.googleapis.com/auth/drive.file`
   - Add test users (your email) if needed

3. **Create OAuth Client**:
   - Application type: "Web application"
   - Name: "Pure Bodybuilding Tracker"
   - Authorized JavaScript origins: Add your domain(s):
     - `http://localhost:8000` (for local testing)
     - `https://yourusername.github.io` (for GitHub Pages)
     - Add any other domains where you'll host the app

4. **Copy the Client ID**:
   - After creation, copy the "Client ID" (looks like: `123456789-abcdef.apps.googleusercontent.com`)

## Step 3: Configure the Workout Tracker

1. **Open the workout-tracker-cloud.html file**
2. **Find this line** (around line 8):
   ```javascript
   const GOOGLE_CLIENT_ID = 'YOUR_GOOGLE_CLIENT_ID_HERE';
   ```
3. **Replace with your actual Client ID**:
   ```javascript
   const GOOGLE_CLIENT_ID = '123456789-abcdef.apps.googleusercontent.com';
   ```

## Step 4: Test the Integration

1. **Open the workout tracker** in your browser
2. **Click "Connect Google Drive"**
3. **Sign in** with your Google account
4. **Grant permissions** for the app to access your Drive files
5. **Verify sync** by checking the cloud status indicator

## How It Works

### Automatic Sync
- **Real-time backup**: Your data syncs automatically every 2 seconds after changes
- **Cross-device sync**: Access your data from any device where you're signed in
- **Offline support**: Works offline, syncs when connection is restored

### Data Storage
- **Location**: Stored in your Google Drive's private app folder
- **File**: `workout-tracker-data.json` (hidden from regular Drive view)
- **Content**: All your workout logs, personal records, and notes
- **Privacy**: Only this app can access this file

### Sync Status Indicators
- ☁️ **Connected**: Successfully synced
- ⏳ **Syncing**: Currently uploading/downloading data  
- ❌ **Error**: Sync failed (will retry automatically)

## Troubleshooting

### "Client ID not configured" Error
- Make sure you replaced `YOUR_GOOGLE_CLIENT_ID_HERE` with your actual Client ID
- Check that the Client ID is correctly formatted (no extra quotes or spaces)

### "Redirect URI mismatch" Error
- Add your domain to "Authorized JavaScript origins" in Google Cloud Console
- For local testing, add `http://localhost:8000`
- For GitHub Pages, add `https://yourusername.github.io`

### "Access blocked" Error
- Make sure you've configured the OAuth consent screen
- Add your email as a test user if the app is in testing mode
- For production use, submit the app for verification

### Sync Not Working
- Check your internet connection
- Try signing out and back in
- Clear browser cache and try again

## Security & Privacy

### What data is stored?
- Your workout logs (sets, weights, reps, dates)
- Personal records and achievements  
- Workout notes
- No personal information beyond what's needed for the app

### How is it protected?
- Data stored in private app folder (not visible in your regular Drive)
- Uses OAuth 2.0 for secure authentication
- Data transmitted over HTTPS
- No data stored on external servers

### Can I delete my data?
- Yes, disconnect from Google Drive to stop syncing
- Delete the app from your Google Account permissions
- The data file will remain in your Drive but won't be accessed

## Advanced Configuration

### Multiple Domains
Add all domains where you'll host the app:
```
http://localhost:8000
http://localhost:3000  
https://yourusername.github.io
https://your-custom-domain.com
```

### Production Deployment
For public use:
1. Submit OAuth consent screen for verification
2. Remove test user restrictions
3. Add comprehensive privacy policy
4. Consider rate limiting for high-traffic usage

## Cost Information

### Free Usage Limits
- **Google Drive API**: 1 billion requests per day (free)
- **Storage**: Uses your Google Drive storage (15GB free)
- **Data size**: Workout tracker data is tiny (~1-50KB typically)

### Typical Usage
- **Personal use**: Completely free (well within all limits)
- **Family sharing**: Free for up to ~10 users
- **Public deployment**: Free for moderate usage

## Support

### Issues with Setup
1. Double-check the Client ID configuration
2. Verify domain authorization in Google Cloud Console  
3. Check browser console for error messages
4. Try incognito mode to rule out extension conflicts

### Need Help?
- Check the troubleshooting section above
- Open an issue in the GitHub repository
- Include error messages and browser console logs

---

## Quick Setup Checklist

- [ ] Create Google Cloud project
- [ ] Enable Google Drive API
- [ ] Configure OAuth consent screen
- [ ] Create OAuth 2.0 Client ID
- [ ] Add authorized domains
- [ ] Copy Client ID to workout tracker
- [ ] Test connection and sync
- [ ] Verify data backup is working

Once setup is complete, you'll have automatic cloud backup and cross-device sync! 🎉