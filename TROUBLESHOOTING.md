# Troubleshooting

## Common Issues

### Jokes Not Loading

**Problem:** Clicking "Get Joke" doesn't display jokes

**Solutions:**
- Check internet connection
- Open browser console (F12) and check for errors
- Try a different API from the dropdown
- Disable browser extensions that might block requests
- Check if API services are down (visit their websites)

### Copy Button Not Working

**Problem:** Copy button doesn't copy to clipboard

**Solutions:**
- Ensure site is served over HTTPS (clipboard API requirement)
- Check browser permissions for clipboard access
- Try a different browser

### Auto Mode Not Stopping

**Problem:** Auto-fetch continues after clicking stop

**Solutions:**
- Refresh the page
- Check browser console for JavaScript errors

### Keyboard Shortcut Not Working

**Problem:** Space bar doesn't fetch jokes

**Solutions:**
- Click somewhere on the page (not in an input field)
- Check if another extension is using the Space key
- Try clicking the page background first

## Browser Issues

### Firefox
If security warnings appear, add exception for the APIs in Settings → Privacy & Security

### Safari
Enable "Allow cross-origin requests" in Develop menu for local testing

## Still Having Issues?

Open an issue on GitHub with:
- Browser and version
- Operating system
- Console error messages
- Steps to reproduce