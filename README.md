# Chrome Tabs Recovery

A browser-based tool to recover lost Chrome tabs from Chrome's internal tabs file. Perfect for when Chrome crashes, Windows updates force-close your browser, or you accidentally close important tabs.

## 🚀 Live Demo

**[Try it now](https://your-username.github.io/chrome-tabs-recovery/)**

No installation required - works entirely in your browser!

## ✨ Features

- **🌐 Browser-based processing** - No downloads or installations needed
- **🔒 Privacy-focused** - All processing happens locally in your browser
- **📁 Drag & drop support** - Simply drop your tabs file to start
- **🧹 Smart cleanup** - Automatically removes duplicates and invalid URLs
- **🔍 Real-time search** - Filter through recovered URLs instantly
- **📊 Export options** - Save as HTML, browser bookmarks, or JSON
- **📱 Mobile-friendly** - Works on all devices
- **🎯 Intelligent deduplication** - Handles incomplete domains and fragments

## 🎯 When to Use This Tool

- Chrome crashed and you lost all your tabs
- Windows/Mac updates forced Chrome to close
- Accidentally closed important browser windows
- Need to recover tabs from a previous browsing session
- Want to extract URLs from Chrome's internal files

## 📁 Finding Your Tabs File

The Chrome tabs file is located in different places depending on your operating system:

### Windows
```
C:\Users\[Your Username]\AppData\Local\Google\Chrome\User Data\Default\tabs
```

**Alternative location (Sessions folder):**
```
C:\Users\[Your Username]\AppData\Local\Google\Chrome\User Data\Default\Sessions\tabs_*
```

### macOS
```
~/Library/Application Support/Google/Chrome/Default/tabs
```

### Linux
```
~/.config/google-chrome/Default/tabs
```

### Tips for Finding the File

1. **Show hidden files** - The AppData folder is hidden by default on Windows
2. **Multiple profiles** - If you use multiple Chrome profiles, check each `Profile X` folder
3. **Recent files** - Look for the most recently modified tabs file
4. **Sessions folder** - Check the Sessions subfolder for additional tab files

## 🔧 How It Works

1. **Upload** your Chrome tabs file using drag & drop or file selection
2. **Processing** - The tool extracts URLs from Chrome's binary format
3. **Cleanup** - Removes duplicates, invalid URLs, and incomplete fragments
4. **Results** - Browse, search, and export your recovered tabs

### Advanced Filtering

The tool automatically removes:
- Duplicate URLs across domains
- Invalid or corrupted URL fragments  
- Base64-encoded session data
- Incomplete domain names
- JWT tokens and authentication fragments

## 📊 What You'll Recover

- **Website URLs** - All your open tabs and their addresses
- **Domain grouping** - Multiple URLs from the same site are intelligently merged
- **Quality filtering** - Only valid, working URLs are included
- **Smart deduplication** - Removes partial duplicates (e.g., `site.com` vs `site.com/page`)

## 💾 Export Options

- **HTML Report** - Standalone file you can save and view later
- **Browser Bookmarks** - Import directly into any browser
- **JSON Data** - Machine-readable format for further processing
- **Open All** - Restore all tabs directly in your browser

## 🛠️ Technical Details

- **Pure JavaScript** - No server required, works offline
- **Binary parsing** - Reads Chrome's internal binary format
- **UTF-8 decoding** - Handles international characters correctly
- **Regex extraction** - Multiple patterns to catch different URL formats
- **Responsive design** - Works on desktop and mobile devices

## 🚨 Troubleshooting

### "No URLs found in file"
- Ensure you're using the correct tabs file
- Check file size - it should be larger than 1KB
- Try files from the Sessions folder
- Make sure Chrome was properly closed (not force-killed)

### "File not found"
- Enable viewing hidden files/folders
- Check all Chrome profile folders
- Look in both Default and numbered Profile folders
- Try the most recently modified tabs file

### Too many invalid URLs
- The file might be corrupted
- Try an older tabs file from the Sessions folder
- Check if Chrome was running when the file was copied

## 🤝 Contributing

Contributions are welcome! Here are ways you can help:

- **Report bugs** - Open an issue with details about the problem
- **Suggest features** - Ideas for improving the tool
- **Submit pull requests** - Code improvements and new features
- **Share feedback** - Let us know how the tool worked for you

### Development Setup

1. Fork the repository
2. Make your changes to `index.html`
3. Test locally by opening the file in a browser
4. Submit a pull request

## 📄 Browser Compatibility

- **Chrome/Edge** - Full support (recommended)
- **Firefox** - Full support
- **Safari** - Full support
- **Mobile browsers** - Basic support

## 🔐 Privacy & Security

- **No data transmission** - Everything happens locally in your browser
- **No tracking** - No analytics or tracking scripts
- **No storage** - Files are not saved or cached
- **Open source** - All code is visible and auditable

## 📜 License

MIT License - feel free to use, modify, and distribute.

## ⚠️ Disclaimer

This tool is designed to help recover lost tabs but cannot guarantee 100% recovery. The effectiveness depends on:
- How Chrome was closed (graceful vs force-kill)
- File corruption levels
- Time since the tabs were lost

Always keep important bookmarks saved separately as a backup.

## 🙏 Acknowledgments

- Inspired by the need to recover tabs after Windows updates
- Built with modern web technologies for maximum compatibility
- Community feedback helped improve the filtering algorithms

## 📧 Support

If you encounter issues or have questions:

1. Check the troubleshooting section above
2. Open an issue on GitHub with details
3. Include your browser version and file size information

---

**Star this repository if it helped you recover your tabs!** ⭐
