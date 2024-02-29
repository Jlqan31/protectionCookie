# protectionCookie
{
  "manifest_version": 2,
  "name": "Çerez sikici",
  "version": "1.0",
  "description": "Bu eklenti çerezleri otomatik olarak gizler.",
  "permissions": [
    "storage",
    "cookies"
  ],
  "background": {
    "scripts": ["background.js"],
    "persistent": false
  },
  "browser_action": {
    "default_popup": "popup.html",
    "default_icon": "icon.png"
  },
  "icons": {
    "16": "icon.png",
    "48": "icon.png",
    "128": "icon.png"
  },
  "content_scripts": [
    {
      "matches": ["<all_urls>"],
      "js": ["content.js"]
    }
  ]
}
