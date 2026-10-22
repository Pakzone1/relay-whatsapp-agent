# Relay

**A WhatsApp AI agent that handles messages and audio calls in one application.**

## The problem

I already had a WhatsApp messaging platform. This time, I wanted the call button to be useful too.

An assistant that handles the chat but has nothing to say when the phone rings has a fairly obvious gap. The goal was to extend the single-tenant workflow to actual WhatsApp audio calls, with the conversation continuing across both modes.

## The solution

A fresh Go application with an embedded React dashboard, local storage, WhatsApp messaging, and a calling bridge connected to OpenAI Realtime.

## What it does

- WhatsApp account pairing and session management.
- Text messages, voice notes, photos, and direct audio calls.
- OpenAI Responses for message handling and Realtime for calls.
- Per-contact context shared across messages and call transcripts.
- Editable persona/settings and dashboard conversation history.
- Local application data stored in SQLite.

## Engineering highlights

Bridges WhatsApp call negotiation and audio transport with realtime model events, durable transcripts, and shared per-contact context. The Go backend serves an embedded React dashboard, bringing pairing, messaging, calling, and configuration into one deployable application.

## Technology

Go, Echo, Whatsmeow, meowcaller, React, TypeScript, Vite, SQLite, OpenAI Responses and Realtime.

## Source code

This repository documents the project, its capabilities, and the engineering behind it. The application source code is maintained privately.
