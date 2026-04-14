# whatsapplockedchat
Bypassing whatsapp locked chats from WhatsappWeb. 

WhatsApp Web implements a "Locked Chats" feature that hides specific conversations behind a user-defined password. However, the "locked" status of these conversations is maintained via flags (isLocked/locked) within the browser's IndexedDB and localStorage.

The provided Proof-of-Concept script identifies these flags within the local database candidates (e.g., "wawc", "model-storage"), modifies them to 'false', and attempts an in-memory UI refresh. This allows an attacker with local access to an authenticated session to view and interact with locked chats without requiring the secondary password.
# Tested on: macOS / Windows / Linux - Chrome & Brave Browsers
