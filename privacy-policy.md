# Privacy Policy — yt-autopilot

**Last updated: 2026-09-14**

## What this is

yt-autopilot is a personal, single-user desktop command-line tool. It runs locally on the author's own Windows PC and manages the author's own YouTube channel. It is not a service, it is not distributed, and it has no users other than the author.

This policy exists because the YouTube API Services Terms of Service require API clients to publish one.

## Who operates this tool

The author of this tool is a private individual in Japan operating their own YouTube channel. Contact: through the GitHub repository issues page where this policy is hosted.

## What data the tool accesses

The tool uses the YouTube Data API v3 and the YouTube Analytics API with these scopes:

- `https://www.googleapis.com/auth/youtube` — to set metadata and thumbnails on the author's own videos
- `https://www.googleapis.com/auth/youtube.upload` — to upload the author's own videos
- `https://www.googleapis.com/auth/yt-analytics.readonly` — to read the author's own channel performance data

The only account accessed is the author's own. The tool has no mechanism to authenticate any other user.

## What data is stored, and where

All data stays on the author's local disk. Nothing is transmitted to any server operated by the author, because no such server exists.

| Data | Where | Why | How long |
|---|---|---|---|
| OAuth access and refresh token | A local file on the author's PC, excluded from version control | To call the YouTube API without re-authenticating every time | Until revoked or replaced |
| The author's own channel analytics (views, watch time, average view percentage, subscriber changes) | Local CSV files | To decide what content to produce next | Indefinitely, at the author's discretion |
| Video IDs and publication timestamps of the author's own videos | A local CSV ledger | To avoid applying the same metadata twice | Indefinitely |

## What data is NOT collected

- No data about any other YouTube channel's private information
- No personal information about viewers, commenters, or subscribers
- No data about any person other than the author
- No payment information
- No location data, device identifiers, or advertising identifiers

## Sharing

No API data is shared with, sold to, or transferred to any third party. There are no analytics services, advertising networks, or data brokers involved.

The tool uses an AI model (Anthropic's Claude) to draft scripts and select topics. **No YouTube API data about other users is sent to it.** What is sent is limited to the author's own channel's aggregate performance numbers and the author's own draft content.

## Google user data and third-party access

This tool does not transfer Google user data to third parties. The author's own aggregate channel statistics may be included in prompts sent to the AI model used for content planning. This is the author's own data about the author's own channel.

## Revoking access

The author can revoke this tool's access at any time at https://myaccount.google.com/permissions. Doing so immediately stops all API access. Locally stored tokens can be deleted by removing the token file.

## Data deletion

Because all data is local, deleting it means deleting the files on the author's own PC. There is no server-side copy to request deletion of.

## Compliance

This tool is operated in accordance with the [YouTube Terms of Service](https://www.youtube.com/t/terms), the [YouTube API Services Terms of Service](https://developers.google.com/youtube/terms/api-services-terms-of-service), and the [Google Privacy Policy](https://policies.google.com/privacy).

The tool does not use automated means other than the official YouTube API to access YouTube. It performs no automated engagement (no comments, likes, subscriptions, or view manipulation).

## Changes

If this policy changes, the updated version will be published at the same URL with a new "Last updated" date.
