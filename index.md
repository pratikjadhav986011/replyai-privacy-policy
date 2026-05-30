# ReplyAI — Privacy Policy

_Last updated: May 30, 2026_

ReplyAI is a browser extension that provides AI-powered smart reply
suggestions for **WhatsApp Web** (`https://web.whatsapp.com`). This policy
explains exactly what data the extension handles, what is sent off your
device, and what is not.

ReplyAI operates **only on WhatsApp Web**. It does not run on, read, or
request permission for any other website or messaging platform.

## 1. What the extension accesses

When you have a WhatsApp Web conversation open and you ask ReplyAI to
generate or rewrite a reply, the extension reads, from the currently open
chat only:

- The text of the most recent incoming message.
- Up to the last 10 messages of the open conversation (text, sender label,
  and direction) to provide context for the suggestion.
- Any text you type into the reply box when you ask ReplyAI to rewrite it.

ReplyAI does **not** read your contact list, phone number, account
credentials, media files, or conversations you have not actively opened.
It does not run in the background when WhatsApp Web is closed.

## 2. What is sent off your device

To generate suggestions, the message text and conversation context described
above are sent over HTTPS to the ReplyAI backend service:

```
https://replyai-backend-production-3648.up.railway.app
```

Along with the message content, the request includes the reply settings you
choose in the extension (for example: tone, relationship type, personality,
and any custom instruction you enter). The backend forwards this context to a
third-party large language model provider to produce reply suggestions, then
returns the suggestions to your browser.

- All transmission uses HTTPS.
- Requests are made only when you actively trigger a suggestion or rewrite.
- The extension does not send your data anywhere other than the backend URL
  listed above.

## 3. What stays on your device

The following is stored **locally** in your browser via `chrome.storage` and
is **never** transmitted off your device by the extension:

- Your preferences and settings.
- Per-contact "memory" and writing-style fingerprint used to tailor
  suggestions.
- Local usage analytics (counts of actions taken). These are stored on-device
  only and are not sent to any server.
- Recent and favorited replies.

You can clear locally stored memory at any time from **Settings → Privacy**
inside the extension.

## 4. Permissions

ReplyAI requests the minimum permissions required to function:

- **`storage`** — to save your preferences and on-device data described above.
- **Host access to `https://web.whatsapp.com/*`** — so the extension can run
  on WhatsApp Web and read the open conversation.
- **Host access to the backend URL above** — so the extension can request
  reply suggestions.

ReplyAI requests **no** access to other sites, browser tabs, history,
cookies, downloads, or any sensitive browser API.

## 5. Data retention

Message content is used only to generate the requested suggestions and is not
used by the extension to build a persistent profile on our servers. Any
server-side handling of request content by the backend or the underlying
model provider is limited to producing the response. Locally stored data
remains on your device until you clear it or remove the extension.

## 6. Children

ReplyAI is not directed to children under 13 and should not be used by them.

## 7. Changes

If this policy changes, the "Last updated" date above will be revised and the
updated policy will be published alongside the extension listing.

## 8. Contact

For privacy questions or data requests, contact the developer through the
support channel listed on the Chrome Web Store listing for ReplyAI.
