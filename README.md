# Discord Voice 24/7

A Discord bot that joins a **permanent voice channel** and checks its connection every 45 seconds.

## Setup
1. Create a permanent voice channel in your Discord server (not a TempVoice-created channel).
2. Give the bot View Channel and Connect permissions.
3. Upload these files to a GitHub repository. Do not upload your bot token.
4. Create a Railway service from that repository. Railway will build the Dockerfile.
5. In Railway Variables, add `DISCORD_TOKEN` and `VOICE_CHANNEL_ID`.
6. Deploy and check Railway logs for `Voice connected to ...`.

Note: 24/7 uptime depends on your Railway plan, usage limits, Discord connectivity, and server/channel permissions. The bot cannot prevent third-party TempVoice managers from deleting temporary channels.
