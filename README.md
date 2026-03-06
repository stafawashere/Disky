# Disky

> A Discord API wrapper, built from scratch in Python only utilizing Discord's Gateway and REST API.

## What it does
- Connects directly to Discord's Gateway (v9) over WebSocket
- Handles heartbeat, reconnection, and invalid session recovery automatically
- Supports both token and email/password authentication
- Spoofs real browser fingerprints, build numbers, and X-Super-Properties to look like an actual Discord client
- Covers 50+ gateway events (messages, guilds, members, reactions, threads, voice, moderation, polls, etc.)
- REST API methods for sending, editing, deleting, pinning, reacting to messages

## Structure
- `client.py` — WebSocket session, gateway connection, heartbeat loop, REST methods
- `objects.py` — Event parsing, gateway event types, User object
- `utility.py` — Browser spoofing, build number scraping, fingerprint fetching, X-Super-Properties encoding
- `logger.py` — Colored console logging
- `errors.py` — Custom exceptions for auth failures
